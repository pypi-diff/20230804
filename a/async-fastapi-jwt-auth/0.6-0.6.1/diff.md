# Comparing `tmp/async_fastapi_jwt_auth-0.6.tar.gz` & `tmp/async_fastapi_jwt_auth-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_fastapi_jwt_auth-0.6.tar", max compression
+gzip compressed data, was "async_fastapi_jwt_auth-0.6.1.tar", max compression
```

## Comparing `async_fastapi_jwt_auth-0.6.tar` & `async_fastapi_jwt_auth-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-01-27 22:05:26.408303 async_fastapi_jwt_auth-0.6/LICENSE
--rw-r--r--   0        0        0     2223 2023-01-27 22:05:26.408393 async_fastapi_jwt_auth-0.6/README.md
--rw-r--r--   0        0        0      161 2023-01-27 22:58:05.789093 async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/__init__.py
--rw-r--r--   0        0        0     4931 2023-08-04 00:00:49.762017 async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/auth_config.py
--rw-r--r--   0        0        0    37133 2023-08-04 00:00:49.762295 async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/auth_jwt.py
--rw-r--r--   0        0        0     4672 2023-08-04 00:00:49.762619 async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/config.py
--rw-r--r--   0        0        0     2292 2023-08-04 00:00:49.762770 async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/exceptions.py
--rw-r--r--   0        0        0     1616 2023-08-04 00:00:55.042672 async_fastapi_jwt_auth-0.6/pyproject.toml
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 async_fastapi_jwt_auth-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2223 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/README.md
+-rw-r--r--   0        0        0      161 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/__init__.py
+-rw-r--r--   0        0        0     4931 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/auth_config.py
+-rw-r--r--   0        0        0    37133 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/auth_jwt.py
+-rw-r--r--   0        0        0     4672 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/config.py
+-rw-r--r--   0        0        0     2292 2023-08-04 00:25:12.865012 async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/exceptions.py
+-rw-r--r--   0        0        0     1618 2023-08-04 00:25:12.869012 async_fastapi_jwt_auth-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 async_fastapi_jwt_auth-0.6.1/PKG-INFO
```

### Comparing `async_fastapi_jwt_auth-0.6/LICENSE` & `async_fastapi_jwt_auth-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/README.md` & `async_fastapi_jwt_auth-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/auth_config.py` & `async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/auth_jwt.py` & `async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/config.py` & `async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/config.py`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/async_fastapi_jwt_auth/exceptions.py` & `async_fastapi_jwt_auth-0.6.1/async_fastapi_jwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_fastapi_jwt_auth-0.6/pyproject.toml` & `async_fastapi_jwt_auth-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_fastapi_jwt_auth"
-version = "0.6"
+version = "0.6.1"
 description = "Async fork of FastAPI extension that provides JWT Auth support (secure, easy to use and lightweight)"
 authors = ["Yan Khachko <a@slnk.icu>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
```

### Comparing `async_fastapi_jwt_auth-0.6/PKG-INFO` & `async_fastapi_jwt_auth-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-fastapi-jwt-auth
-Version: 0.6
+Version: 0.6.1
 Summary: Async fork of FastAPI extension that provides JWT Auth support (secure, easy to use and lightweight)
 License: MIT
 Author: Yan Khachko
 Author-email: a@slnk.icu
 Requires-Python: >=3.8
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: async-fastapi-jwt-auth Version: 0.6 Summary: Async
-fork of FastAPI extension that provides JWT Auth support (secure, easy to use
-and lightweight) License: MIT Author: Yan Khachko Author-email: a@slnk.icu
+Metadata-Version: 2.1 Name: async-fastapi-jwt-auth Version: 0.6.1 Summary:
+Async fork of FastAPI extension that provides JWT Auth support (secure, easy to
+use and lightweight) License: MIT Author: Yan Khachko Author-email: a@slnk.icu
 Requires-Python: >=3.8 Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

