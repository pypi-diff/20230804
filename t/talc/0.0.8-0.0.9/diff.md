# Comparing `tmp/talc-0.0.8.tar.gz` & `tmp/talc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.0.8.tar", last modified: Tue Jul 25 05:00:16 2023, max compression
+gzip compressed data, was "talc-0.0.9.tar", last modified: Fri Aug  4 06:03:37 2023, max compression
```

## Comparing `talc-0.0.8.tar` & `talc-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.529008 talc-0.0.8/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.8/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-25 05:00:16.528892 talc-0.0.8/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.8/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-25 04:59:13.000000 talc-0.0.8/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-25 05:00:16.529043 talc-0.0.8/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.527366 talc-0.0.8/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.527883 talc-0.0.8/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.8/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)    15270 2023-07-25 04:53:42.000000 talc-0.0.8/src/talc/talc.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.528736 talc-0.0.8/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-08-04 06:03:37.576057 talc-0.0.9/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.9/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)     2307 2023-08-04 06:03:37.575918 talc-0.0.9/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)     1884 2023-08-04 06:02:45.000000 talc-0.0.9/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-08-04 06:01:06.000000 talc-0.0.9/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-08-04 06:03:37.576096 talc-0.0.9/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-08-04 06:03:37.574304 talc-0.0.9/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-08-04 06:03:37.574787 talc-0.0.9/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.9/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)    15691 2023-08-04 05:59:09.000000 talc-0.0.9/src/talc/talc.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-08-04 06:03:37.575769 talc-0.0.9/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)     2307 2023-08-04 06:03:37.000000 talc-0.0.9/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-08-04 06:03:37.000000 talc-0.0.9/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-08-04 06:03:37.000000 talc-0.0.9/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-08-04 06:03:37.000000 talc-0.0.9/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-08-04 06:03:37.000000 talc-0.0.9/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.0.8/PKG-INFO` & `talc-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -57,26 +57,33 @@
 ```python
 sessionId = talc.createSession()
 ```
 
 ### Step 3: Log calls
 
 
-Talc automatically integrates with the OpenAI chat API, so all you need to do is pass an additional parameter to your calls. 
+Talc automatically integrates with the OpenAI chat completion API, so all you need to do is pass an additional parameter to your calls. 
 
 Add the `session=sessionId` parameter to your chat completion calls:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
 )
 ```
 
+If you are using a wrapper library like SemanticKernel and don't have access to the direct chat completion call, you can set the session globally:
+
+```python
+session_id = talc.createSession()
+talc.setGlobalSession(session_id)
+```
+
 If your application uses agents or multistep chains, you can add the optional `agent` parameter to identify the current agent or step of the chain:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
```

### Comparing `talc-0.0.8/README.md` & `talc-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,26 +44,33 @@
 ```python
 sessionId = talc.createSession()
 ```
 
 ### Step 3: Log calls
 
 
-Talc automatically integrates with the OpenAI chat API, so all you need to do is pass an additional parameter to your calls. 
+Talc automatically integrates with the OpenAI chat completion API, so all you need to do is pass an additional parameter to your calls. 
 
 Add the `session=sessionId` parameter to your chat completion calls:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
 )
 ```
 
+If you are using a wrapper library like SemanticKernel and don't have access to the direct chat completion call, you can set the session globally:
+
+```python
+session_id = talc.createSession()
+talc.setGlobalSession(session_id)
+```
+
 If your application uses agents or multistep chains, you can add the optional `agent` parameter to identify the current agent or step of the chain:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
```

### Comparing `talc-0.0.8/pyproject.toml` & `talc-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talc"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Max Kerr", email="max@talc.ai" },
   { name="Matt Lee", email="matt@talc.ai" },
 ]
 description = "Logging client for Talc Debugger."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `talc-0.0.8/src/talc/talc.py` & `talc-0.0.9/src/talc/talc.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,25 +45,28 @@
                     "organization": self.__organization,
                 }
             )
             .execute()
         )
         return response.data[0]["id"]
 
-    def __createInput(self, sessionId, generationId, role, content, name, index):
+    def __createInput(
+        self, sessionId, generationId, role, content, name, function_call, index
+    ):
         response = (
             self.supabase.table("inputs")
             .insert(
                 {
                     "session": sessionId,
                     "generation": generationId,
                     "role": role,
                     "content": content,
                     "index": index,
                     "name": name,
+                    "function_call": function_call,
                 }
             )
             .execute()
         )
         return response.data[0]["id"]
 
     def __createGeneration(
@@ -91,20 +94,25 @@
             )
             .execute()
         )
         return response.data[0]["id"]
 
     def __historyArrayToInputs(self, history, generationId, sessionId):
         for index, chat in enumerate(history):
+            encoded_function_call = None
+            if "function_call" in chat:
+                encoded_function_call = json.dumps(chat["function_call"])
+
             self.__createInput(
                 sessionId,
                 generationId,
                 chat["role"],
                 chat["content"],
                 chat.get("name", None),  # Name is optional
+                encoded_function_call,
                 # Index is reversed because we want the most recent message to have the lowest index
                 len(history) - index,
             )
 
     def log(
         self,
         sessionId,
@@ -135,20 +143,28 @@
 
 
 def init():
     global client
     client = _SupabaseClient()
 
 
+globalSession = None
+
+
+def setGlobalSession(session):
+    global globalSession
+    globalSession = session
+
+
 class __alternateCompletion(openai.ChatCompletion):
     @classmethod
     def create(cls, *args, **kwargs):
         # Pop arguments that are not supported by the original create method
         agent = kwargs.pop("agent", "Default")
-        session = kwargs.pop("session", None)
+        session = kwargs.pop("session", globalSession)
         stream = "stream" in kwargs and kwargs["stream"]
 
         # Handle case where we have received the full response at once.
         if not stream:
             result = super().create(*args, **kwargs)
             try:
                 functions_available, parameters = cls.__getFunctionsAndParameters(
@@ -174,15 +190,15 @@
             return cls.__streamContent(session=session, agent=agent, *args, **kwargs)
 
     # Handles the case where we are streaming the response
     # This is really complicated. Godspeed.
     @classmethod
     def __streamContent(cls, *args, **kwargs):
         agent = kwargs.pop("agent", "Default")
-        session = kwargs.pop("session", None)
+        session = kwargs.pop("session", globalSession)
 
         generator = super().create(*args, **kwargs)
 
         choices = {}
         final_choice = None
 
         for result in generator:
@@ -261,15 +277,15 @@
             logging.warning("Error logging to talc: ", e)
 
         return final_choice
 
     @classmethod
     async def __streamContentAsync(cls, *args, **kwargs):
         agent = kwargs.pop("agent", "Default")
-        session = kwargs.pop("session", None)
+        session = kwargs.pop("session", globalSession)
 
         generator = super().acreate(*args, **kwargs)
 
         choices = {}
         final_choice = None
 
         async for result in await generator:
@@ -355,15 +371,15 @@
         # print("Arguments ", option, ":", "".join(arguments_accumulator))
         # print("=====================================")
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         # Pop arguments that are not supported by the original create method
         agent = kwargs.pop("agent", "Default")
-        session = kwargs.pop("session", None)
+        session = kwargs.pop("session", globalSession)
         stream = "stream" in kwargs and kwargs["stream"]
 
         # Handle case where we have received the full response at once.
         if not stream:
             result = await super().acreate(*args, **kwargs)
             try:
                 functions_available, parameters = cls.__getFunctionsAndParameters(
```

### Comparing `talc-0.0.8/src/talc.egg-info/PKG-INFO` & `talc-0.0.9/src/talc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -57,26 +57,33 @@
 ```python
 sessionId = talc.createSession()
 ```
 
 ### Step 3: Log calls
 
 
-Talc automatically integrates with the OpenAI chat API, so all you need to do is pass an additional parameter to your calls. 
+Talc automatically integrates with the OpenAI chat completion API, so all you need to do is pass an additional parameter to your calls. 
 
 Add the `session=sessionId` parameter to your chat completion calls:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
 )
 ```
 
+If you are using a wrapper library like SemanticKernel and don't have access to the direct chat completion call, you can set the session globally:
+
+```python
+session_id = talc.createSession()
+talc.setGlobalSession(session_id)
+```
+
 If your application uses agents or multistep chains, you can add the optional `agent` parameter to identify the current agent or step of the chain:
 
 ```python
 response = openai.ChatCompletion.create(
     model="gpt-3.5-turbo-0613",
     messages=messages,
     session=sessionId,
```

