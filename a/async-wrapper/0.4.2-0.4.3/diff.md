# Comparing `tmp/async_wrapper-0.4.2.tar.gz` & `tmp/async_wrapper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.2.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.3.tar", max compression
```

## Comparing `async_wrapper-0.4.2.tar` & `async_wrapper-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1070 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/LICENSE
--rw-r--r--   0        0        0     1681 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/README.md
--rw-r--r--   0        0        0     3416 2023-08-02 14:36:42.939421 async_wrapper-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-02 14:36:42.975421 async_wrapper-0.4.2/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      595 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     1186 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1261 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0        0 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      151 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0      104 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/exception.py
--rw-r--r--   0        0        0     5976 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      793 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 async_wrapper-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1681 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/README.md
+-rw-r--r--   0        0        0     3493 2023-08-04 00:24:16.449975 async_wrapper-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-04 00:24:16.489975 async_wrapper-0.4.3/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     1186 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1261 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      551 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      151 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     5976 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      806 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0      101 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/utils/__init__.py
+-rw-r--r--   0        0        0     7701 2023-08-04 00:23:53.557851 async_wrapper-0.4.3/src/async_wrapper/utils/queue.py
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 async_wrapper-0.4.3/PKG-INFO
```

### Comparing `async_wrapper-0.4.2/LICENSE` & `async_wrapper-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/README.md` & `async_wrapper-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/pyproject.toml` & `async_wrapper-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.2"
+version = "0.4.3"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = "^3.7.0"
 uvloop = { version = "^0.17.0", optional = true, markers = "platform_system != 'Windows'" }
+exceptiongroup = { version = "^1.1.2", markers = "python_version < '3.11'" }
 
 [tool.poetry.extras]
 uvloop = ['uvloop']
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.282"
 black = "23.3.0"
```

### Comparing `async_wrapper-0.4.2/src/async_wrapper/convert/_async.py` & `async_wrapper-0.4.3/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.3/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/src/async_wrapper/convert/abc.py` & `async_wrapper-0.4.3/src/async_wrapper/convert/abc.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/src/async_wrapper/convert/main.py` & `async_wrapper-0.4.3/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.3/src/async_wrapper/task_group/task_group.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.2/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.3/src/async_wrapper/task_group/value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from threading import local
 from typing import Generic, TypeVar
 
-from .exception import PendingError
+from async_wrapper.exception import PendingError
 
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 Pending = local()
 
 __all__ = ["SoonValue"]
```

### Comparing `async_wrapper-0.4.2/PKG-INFO` & `async_wrapper-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.2
+Version: 0.4.3
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: uvloop
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
+Requires-Dist: exceptiongroup (>=1.1.2,<2.0.0) ; python_version < "3.11"
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
```

