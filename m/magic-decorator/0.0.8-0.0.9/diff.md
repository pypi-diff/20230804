# Comparing `tmp/magic_decorator-0.0.8.tar.gz` & `tmp/magic_decorator-0.0.9.tar.gz`

## Comparing `magic_decorator-0.0.8.tar` & `magic_decorator-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/LICENSE
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 magic_decorator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 magic_decorator-0.0.9/PKG-INFO
```

### Comparing `magic_decorator-0.0.8/magic_decorator.py` & `magic_decorator-0.0.9/magic_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,21 @@
     )
 
     return chain
 
 
 def magic(llm: BaseLanguageModel, return_all=False):
     def decorator(func: Callable):
+        chain = _get_func_chain(llm=llm, func=func, return_all=return_all)
+        signature = inspect.signature(func)
+
         @wraps(func)
         def wrapper(*args, **kwargs):
-            arguments = inspect.signature(func).bind(*args, **kwargs).arguments
-            return _get_func_chain(llm=llm, func=func, return_all=return_all).predict(
-                **arguments
-            )
+            arguments = signature.bind(*args, **kwargs).arguments
+            return chain.predict(**arguments)
 
         return wrapper
 
     return decorator
 
 
 def magic_langchain(llm: BaseLanguageModel, return_all=False):
```

### Comparing `magic_decorator-0.0.8/.gitignore` & `magic_decorator-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.8/LICENSE` & `magic_decorator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.8/README.md` & `magic_decorator-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,57 @@
-# Simple demo function using OpenAI's ChatComplete
+# Simple demo function using LangChain
 
 The only function implemented in this module is magic.
 
-`magic` works as a decorator. It simply sends the function's signature and docstring to the GPT and expects to get a result.
+`magic` works as a decorator. It simply sends the function's signature and docstring to the LLM and expects to get a result.
 
 It can be installed with `pip install magic-decorator` and used with `from magic_decorator import magic`.
 
 ```python
+from langchain import SomeLLMModels
+llm = SomeLLMModels()
+
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def transpose(matrix: list[list[int]]) -> list[list[int]]:
     """
     This function finds the transpose of the given matrix.
     """
 transpose([[1,2,3],[4,5,6]])
 ```
 ```
 [[1, 4], [2, 5], [3, 6]]
 ```
 
 ```python
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def add(a: float, b: float) -> float:
     """
     This function adds a and b.
     """
 add(1., 10.)
 ```
 ```
 11.0
 ```
 
 ```python
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def friend(message: str) -> str:
     """
     This function responds like a friend.
     """
 friend("Hi, how are you today?")
 ```
 ```
 'Hey! I am doing great, thank you. How about you?'
 ```
 
-Since the magic decorator works with OpenAI's API, you need to put the API_KEY in an environment variable or directly in the decorator.
-```python
-import os
-from magic_decorator import magic
-
-os.environ["OPENAI_API_KEY"] = ...
-# or
-@magic(model="gpt-4", api_key=...)
-def func():
-    ...
-```
-Alternatively, you can pre-declare decorators that will be used repeatedly.
-```python
-cold_magic = magic(model="gpt-4", temperature=0)
-@cold_magic
-def func():
-    ...
-```
-
 Added a decorator for langchain. In this case, it becomes LLMChain.
 ```python
 llm = SomeLLMModels()
 @magic_langchain(llm=llm)
 def mychain(arg1: int, arg2: str):
     ...
```

### Comparing `magic_decorator-0.0.8/pyproject.toml` & `magic_decorator-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magic-decorator"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name="Kim Minjong", email="make.dirty.code@gmail.com"},
 ]
 description = "A magic function decorator using OpenAI ChatCompletion"
 readme = "README.md"
 requires-python = ">=3.7.1"
 dependencies = ["openai>0.27", "sick-json", "langchain"]
```

### Comparing `magic_decorator-0.0.8/PKG-INFO` & `magic_decorator-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,72 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.8
+Version: 0.0.9
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
 Requires-Dist: langchain
 Requires-Dist: openai>0.27
 Requires-Dist: sick-json
 Description-Content-Type: text/markdown
 
-# Simple demo function using OpenAI's ChatComplete
+# Simple demo function using LangChain
 
 The only function implemented in this module is magic.
 
-`magic` works as a decorator. It simply sends the function's signature and docstring to the GPT and expects to get a result.
+`magic` works as a decorator. It simply sends the function's signature and docstring to the LLM and expects to get a result.
 
 It can be installed with `pip install magic-decorator` and used with `from magic_decorator import magic`.
 
 ```python
+from langchain import SomeLLMModels
+llm = SomeLLMModels()
+
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def transpose(matrix: list[list[int]]) -> list[list[int]]:
     """
     This function finds the transpose of the given matrix.
     """
 transpose([[1,2,3],[4,5,6]])
 ```
 ```
 [[1, 4], [2, 5], [3, 6]]
 ```
 
 ```python
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def add(a: float, b: float) -> float:
     """
     This function adds a and b.
     """
 add(1., 10.)
 ```
 ```
 11.0
 ```
 
 ```python
 from magic_decorator import magic
-@magic(model="gpt-4")
+@magic(llm=llm)
 def friend(message: str) -> str:
     """
     This function responds like a friend.
     """
 friend("Hi, how are you today?")
 ```
 ```
 'Hey! I am doing great, thank you. How about you?'
 ```
 
-Since the magic decorator works with OpenAI's API, you need to put the API_KEY in an environment variable or directly in the decorator.
-```python
-import os
-from magic_decorator import magic
-
-os.environ["OPENAI_API_KEY"] = ...
-# or
-@magic(model="gpt-4", api_key=...)
-def func():
-    ...
-```
-Alternatively, you can pre-declare decorators that will be used repeatedly.
-```python
-cold_magic = magic(model="gpt-4", temperature=0)
-@cold_magic
-def func():
-    ...
-```
-
 Added a decorator for langchain. In this case, it becomes LLMChain.
 ```python
 llm = SomeLLMModels()
 @magic_langchain(llm=llm)
 def mychain(arg1: int, arg2: str):
     ...
```

