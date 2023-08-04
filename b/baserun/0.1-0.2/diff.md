# Comparing `tmp/baserun-0.1.tar.gz` & `tmp/baserun-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-0.1.tar", last modified: Tue Aug  1 17:48:07 2023, max compression
+gzip compressed data, was "baserun-0.2.tar", last modified: Wed Aug  2 17:28:27 2023, max compression
```

## Comparing `baserun-0.1.tar` & `baserun-0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-01 17:48:07.458694 baserun-0.1/
--rw-r--r--   0 adam       (501) staff       (20)     1073 2023-08-01 17:47:59.000000 baserun-0.1/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)     3303 2023-08-01 17:48:07.458743 baserun-0.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1717 2023-08-01 16:58:40.000000 baserun-0.1/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-01 17:48:07.456848 baserun-0.1/baserun/
--rw-r--r--   0 adam       (501) staff       (20)      239 2023-07-26 19:18:57.000000 baserun-0.1/baserun/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7959 2023-08-01 16:35:53.000000 baserun-0.1/baserun/baserun.py
--rw-r--r--   0 adam       (501) staff       (20)      523 2023-07-27 15:16:20.000000 baserun-0.1/baserun/cli.py
--rw-r--r--   0 adam       (501) staff       (20)     1051 2023-07-30 18:03:35.000000 baserun-0.1/baserun/helpers.py
--rw-r--r--   0 adam       (501) staff       (20)     2535 2023-07-31 17:37:43.000000 baserun-0.1/baserun/openai.py
--rw-r--r--   0 adam       (501) staff       (20)     1327 2023-07-31 18:15:20.000000 baserun-0.1/baserun/pytest_plugin.py
--rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-27 22:26:42.000000 baserun-0.1/baserun/unittests_class.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-01 17:48:07.457681 baserun-0.1/baserun.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3303 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      459 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       90 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/entry_points.txt
--rw-r--r--   0 adam       (501) staff       (20)       17 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2023-08-01 17:48:07.000000 baserun-0.1/baserun.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      589 2023-08-01 17:47:59.000000 baserun-0.1/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       81 2023-08-01 17:48:07.458912 baserun-0.1/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-01 17:48:07.458487 baserun-0.1/tests/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-24 16:20:33.000000 baserun-0.1/tests/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     4484 2023-08-01 16:35:53.000000 baserun-0.1/tests/explicit_init.py
--rw-r--r--   0 adam       (501) staff       (20)     3311 2023-08-01 16:35:53.000000 baserun-0.1/tests/pytest_test.py
--rw-r--r--   0 adam       (501) staff       (20)     4520 2023-08-01 16:35:53.000000 baserun-0.1/tests/unittests_test.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-02 17:28:27.132110 baserun-0.2/
+-rw-r--r--   0 adam       (501) staff       (20)     1073 2023-08-01 17:47:59.000000 baserun-0.2/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)     3328 2023-08-02 17:28:27.132153 baserun-0.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1717 2023-08-02 16:52:01.000000 baserun-0.2/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-02 17:28:27.130936 baserun-0.2/baserun/
+-rw-r--r--   0 adam       (501) staff       (20)      239 2023-07-26 19:18:57.000000 baserun-0.2/baserun/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7971 2023-08-02 16:51:41.000000 baserun-0.2/baserun/baserun.py
+-rw-r--r--   0 adam       (501) staff       (20)      523 2023-07-27 15:16:20.000000 baserun-0.2/baserun/cli.py
+-rw-r--r--   0 adam       (501) staff       (20)     1051 2023-07-30 18:03:35.000000 baserun-0.2/baserun/helpers.py
+-rw-r--r--   0 adam       (501) staff       (20)     2535 2023-07-31 17:37:43.000000 baserun-0.2/baserun/openai.py
+-rw-r--r--   0 adam       (501) staff       (20)     1327 2023-07-31 18:15:20.000000 baserun-0.2/baserun/pytest_plugin.py
+-rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-27 22:26:42.000000 baserun-0.2/baserun/unittests_class.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-02 17:28:27.131559 baserun-0.2/baserun.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3328 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      459 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)       90 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 adam       (501) staff       (20)       17 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-08-02 17:28:27.000000 baserun-0.2/baserun.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      617 2023-08-02 17:27:32.000000 baserun-0.2/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       81 2023-08-02 17:28:27.132300 baserun-0.2/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-02 17:28:27.132014 baserun-0.2/tests/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-24 16:20:33.000000 baserun-0.2/tests/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     4484 2023-08-01 16:35:53.000000 baserun-0.2/tests/explicit_init.py
+-rw-r--r--   0 adam       (501) staff       (20)     3311 2023-08-01 16:35:53.000000 baserun-0.2/tests/pytest_test.py
+-rw-r--r--   0 adam       (501) staff       (20)     4520 2023-08-01 16:35:53.000000 baserun-0.2/tests/unittests_test.py
```

### Comparing `baserun-0.1/LICENSE` & `baserun-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-0.1/PKG-INFO` & `baserun-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.1
+Version: 0.2
 Summary: Tools for testing, debugging, and evaluating LLM features.
 Author-email: Adam Ginzberg <adam@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baserun
 
 **[Baserun](https://baserun.ai)** is the collaborative workspace for AI teams. Our mission is to simplify the testing, debugging, and evaluation of LLM features to help you get your app production-ready.
 
@@ -83,15 +84,15 @@
 ## Custom logs
 
 ### log
 Logs a custom message to Baserun. If Baserun is not initialized, this function will have no effect.
 
 #### Parameters
 * message (str): The custom log message to be recorded.
-* payload (Union[str, dict]): The log's additional data, which can be either a string or a dictionary.
+* payload (Union[str, Dict]): The log's additional data, which can be either a string or a dictionary.
 
 ```python
 import baserun
 
 def test_custom_log():
     ...
     baserun.log("CustomEvent", payload={"key": "value"})
```

### Comparing `baserun-0.1/README.md` & `baserun-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ## Custom logs
 
 ### log
 Logs a custom message to Baserun. If Baserun is not initialized, this function will have no effect.
 
 #### Parameters
 * message (str): The custom log message to be recorded.
-* payload (Union[str, dict]): The log's additional data, which can be either a string or a dictionary.
+* payload (Union[str, Dict]): The log's additional data, which can be either a string or a dictionary.
 
 ```python
 import baserun
 
 def test_custom_log():
     ...
     baserun.log("CustomEvent", payload={"key": "value"})
```

### Comparing `baserun-0.1/baserun/baserun.py` & `baserun-0.2/baserun/baserun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import uuid
 import os
 import requests
 import time
 import threading
-from typing import Union
+from typing import List, Dict, Union
 from urllib.parse import urlparse
 import warnings
 from .helpers import BaserunProvider, BaserunStepType, BaserunType, get_provider_for_model
 from .openai import monkey_patch_openai
 
 _thread_local = threading.local()
 
@@ -79,15 +79,15 @@
             _thread_local.buffer = []
             del _thread_local.baserun_test_execution_id
             return result
 
         return wrapper
 
     @staticmethod
-    def log(name: str, payload: Union[str, dict]):
+    def log(name: str, payload: Union[str, Dict]):
         if not Baserun._initialized:
             return
 
         baserun_test_execution_id = getattr(_thread_local, "baserun_test_execution_id", None)
         if not baserun_test_execution_id:
             warnings.warn("baserun.log was called outside of a Baserun decorated test. The log will be ignored.")
             return
@@ -98,15 +98,15 @@
             "payload": payload,
             "timestamp": time.time(),
         }
 
         Baserun._append_to_buffer(log_entry)
 
     @staticmethod
-    def log_llm_chat(config: dict, messages: list[dict], output: str, variables: dict[str, str] = None):
+    def log_llm_chat(config: Dict, messages: List[Dict], output: str, variables: Dict[str, str] = None):
         if not Baserun._initialized:
             return
 
         baserun_test_execution_id = getattr(_thread_local, "baserun_test_execution_id", None)
         if not baserun_test_execution_id:
             warnings.warn(
                 "baserun.log_llm_chat was called outside of a Baserun decorated test. The log will be ignored.")
@@ -140,15 +140,15 @@
             "variables": variables if variables else {},
             "timestamp": time.time(),
         }
 
         Baserun._append_to_buffer(log_entry)
 
     @staticmethod
-    def log_llm_completion(config: dict[str, any], prompt: str, output: str, variables: dict[str, str] = None):
+    def log_llm_completion(config: Dict[str, any], prompt: str, output: str, variables: Dict[str, str] = None):
         if not Baserun._initialized:
             return
 
         baserun_test_execution_id = getattr(_thread_local, "baserun_test_execution_id", None)
         if not baserun_test_execution_id:
             warnings.warn("baserun.log_llm_completion was called outside of a Baserun decorated test. The log will be ignored.")
             return
@@ -175,15 +175,15 @@
             "variables": variables if variables else {},
             "timestamp": time.time(),
         }
 
         Baserun._append_to_buffer(log_entry)
 
     @staticmethod
-    def store_test(test_data: dict):
+    def store_test(test_data: Dict):
         Baserun._testExecutions.append(test_data)
 
     @staticmethod
     def flush():
         if not Baserun._initialized:
             warnings.warn("Baserun has not been initialized. No data will be flushed.")
             return
@@ -204,12 +204,12 @@
 
         except requests.RequestException as e:
             warnings.warn(f"Failed to upload results to Baserun: {str(e)}")
 
         Baserun._testExecutions = []
 
     @staticmethod
-    def _append_to_buffer(log_entry: dict):
+    def _append_to_buffer(log_entry: Dict):
         if not hasattr(_thread_local, 'buffer'):
             _thread_local.buffer = []
 
         _thread_local.buffer.append(log_entry)
```

### Comparing `baserun-0.1/baserun/cli.py` & `baserun-0.2/baserun/cli.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/baserun/helpers.py` & `baserun-0.2/baserun/helpers.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/baserun/openai.py` & `baserun-0.2/baserun/openai.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/baserun/pytest_plugin.py` & `baserun-0.2/baserun/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/baserun/unittests_class.py` & `baserun-0.2/baserun/unittests_class.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/baserun.egg-info/PKG-INFO` & `baserun-0.2/baserun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.1
+Version: 0.2
 Summary: Tools for testing, debugging, and evaluating LLM features.
 Author-email: Adam Ginzberg <adam@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,14 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baserun
 
 **[Baserun](https://baserun.ai)** is the collaborative workspace for AI teams. Our mission is to simplify the testing, debugging, and evaluation of LLM features to help you get your app production-ready.
 
@@ -83,15 +84,15 @@
 ## Custom logs
 
 ### log
 Logs a custom message to Baserun. If Baserun is not initialized, this function will have no effect.
 
 #### Parameters
 * message (str): The custom log message to be recorded.
-* payload (Union[str, dict]): The log's additional data, which can be either a string or a dictionary.
+* payload (Union[str, Dict]): The log's additional data, which can be either a string or a dictionary.
 
 ```python
 import baserun
 
 def test_custom_log():
     ...
     baserun.log("CustomEvent", payload={"key": "value"})
```

### Comparing `baserun-0.1/pyproject.toml` & `baserun-0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "0.1"
+version = "0.2"
 description = "Tools for testing, debugging, and evaluating LLM features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     {name = "Adam Ginzberg", email = "adam@baserun.ai"}
 ]
+requires-python = ">=3.7.1"
 dependencies = [
     "requests>=2.31.0"
 ]
 
 [project.urls]
 Homepage="https://baserun.ai"
 Repository="https://github.com/baserun-ai/baserun-py"
```

### Comparing `baserun-0.1/tests/explicit_init.py` & `baserun-0.2/tests/explicit_init.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/tests/pytest_test.py` & `baserun-0.2/tests/pytest_test.py`

 * *Files identical despite different names*

### Comparing `baserun-0.1/tests/unittests_test.py` & `baserun-0.2/tests/unittests_test.py`

 * *Files identical despite different names*

