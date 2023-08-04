# Comparing `tmp/open_interpreter-0.0.245.tar.gz` & `tmp/open_interpreter-0.0.246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.245.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.246.tar", max compression
```

## Comparing `open_interpreter-0.0.245.tar` & `open_interpreter-0.0.246.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.245/LICENSE
--rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.245/README.md
--rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.245/cli/__init__.py
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.245/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.245/interpreter/exec.py
--rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.245/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.245/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.245/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3090 2023-08-02 00:14:15.256798 open_interpreter-0.0.245/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.245/interpreter/view.py
--rw-r--r--   0        0        0      578 2023-08-02 00:14:33.072959 open_interpreter-0.0.245/pyproject.toml
--rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 open_interpreter-0.0.245/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.246/LICENSE
+-rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.246/README.md
+-rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.246/cli/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.246/interpreter/__init__.py
+-rw-r--r--   0        0        0     7256 2023-08-04 06:16:21.710559 open_interpreter-0.0.246/interpreter/exec.py
+-rw-r--r--   0        0        0     9066 2023-08-03 19:47:19.678943 open_interpreter-0.0.246/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.246/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3090 2023-08-02 00:25:57.099108 open_interpreter-0.0.246/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.246/interpreter/view.py
+-rw-r--r--   0        0        0      599 2023-08-04 06:27:49.719302 open_interpreter-0.0.246/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 open_interpreter-0.0.246/PKG-INFO
```

### Comparing `open_interpreter-0.0.245/LICENSE` & `open_interpreter-0.0.246/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/README.md` & `open_interpreter-0.0.246/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/cli/__init__.py` & `open_interpreter-0.0.246/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/interpreter/exec.py` & `open_interpreter-0.0.246/interpreter/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     # If data exceeds max length, truncate it and add message
     if len(data) > max_output_chars:
         data = message + data[-max_output_chars:]
     return data
 
 class RichOutStream:
 
-    def __init__(self, live, max_output_chars):
+    def __init__(self, live, max_output_chars, sysout):
         self.live = live
         self.data = ""
         self.max_output_chars = max_output_chars
+        self.sysout = sysout
 
     def write(self, data):
         self.data += data
 
         # Clean ANSI color codes
         self.data = re.sub(r'\x1b\[[0-9;]*m', '', self.data)
       
@@ -61,15 +62,15 @@
             self.data = ""
             self.live.update("")
         else:
             panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
             self.live.update(panel)
 
     def flush(self):
-        pass
+        self.sysout.flush()
 
     # Some things (like youtube-dl) will check if this is "isatty()"
     # then fail if it isn't present, so. If this is True it breaks the CLI, so we set it to False (I don't know what it means).
     def isatty(self):
         return False
 
 def exec_and_capture_output(code, max_output_chars, forbidden_commands):
@@ -97,15 +98,15 @@
     shell.showtraceback = custom_showtraceback
 
     code = jupyterify_code(code)
 
     live = Live(console=Console())
     try:
         live.start()
-        rich_stdout = RichOutStream(live, max_output_chars)
+        rich_stdout = RichOutStream(live, max_output_chars, old_stdout)
 
         # Check syntax before attempting to execute
         try:
             check_for_syntax_errors(code)
         except SyntaxError:
             # Do the same thing you do in custom_showtraceback
             etype, value, tb = sys.exc_info()
```

### Comparing `open_interpreter-0.0.245/interpreter/interpreter.py` & `open_interpreter-0.0.246/interpreter/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from .exec import exec_and_capture_output
 from .view import View
 from .json_utils import JsonDeltaCalculator
-from .openai_utils import openai_streaming_response
+import openai
+import tokentrim as tt
 import os
 import readline
 
 
 functions = [{
   "name": "run_code",
   "description":
@@ -160,17 +161,22 @@
     try:
 
       # make openai call
       gpt_functions = [{k: v
                         for k, v in d.items() if k != 'function'}
                        for d in functions]
 
-      response = openai_streaming_response(self.messages, gpt_functions,
-                                           self.system_message, "gpt-4-0613",
-                                           self.temperature, self.api_key)
+      model = "gpt-4-0613"
+      response = openai.ChatCompletion.create(
+          model=model,
+          messages=tt.trim(self.messages, model, system_message=self.system_message),
+          functions=gpt_functions,
+          stream=True,
+          temperature=self.temperature,
+      )
 
       base_event = {"role": "assistant", "content": ""}
       event = base_event
 
       func_call = {
         "name": None,
         "arguments": "",
```

### Comparing `open_interpreter-0.0.245/interpreter/json_utils.py` & `open_interpreter-0.0.246/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/interpreter/system_message.txt` & `open_interpreter-0.0.246/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/interpreter/view.py` & `open_interpreter-0.0.246/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.245/pyproject.toml` & `open_interpreter-0.0.246/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
     {include = "cli"}
 ]
-version = "0.0.245"
+version = "0.0.246"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
 ipython = "^8.14.0"
 astor = "^0.8.1"
 git-python = "^1.0.3"
+tokentrim = "^0.1.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `open_interpreter-0.0.245/PKG-INFO` & `open_interpreter-0.0.246/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.245
+Version: 0.0.246
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: git-python (>=1.0.3,<2.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: tokentrim (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Open Interpreter
 
 A minimal, open-source implementation of OpenAI's code interpreter.
 
 ![Interpreter Demo](https://github.com/KillianLucas/open-interpreter/assets/63927363/a1597f66-d298-4172-bc0b-35b36e1479eb)
```

