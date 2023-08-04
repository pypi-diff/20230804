# Comparing `tmp/supafunc-0.2.2.tar.gz` & `tmp/supafunc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supafunc-0.2.2.tar", max compression
+gzip compressed data, was "supafunc-0.2.3.tar", max compression
```

## Comparing `supafunc-0.2.2.tar` & `supafunc-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2022-06-13 01:43:38.321427 supafunc-0.2.2/LICENSE
--rw-r--r--   0        0        0      341 2022-10-10 15:45:49.718730 supafunc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       68 2022-10-10 15:45:59.217059 supafunc-0.2.2/supafunc/__init__.py
--rw-r--r--   0        0        0     1902 2022-10-10 03:28:36.516188 supafunc-0.2.2/supafunc/functions_client.py
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 supafunc-0.2.2/setup.py
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 supafunc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-04 08:08:21.383712 supafunc-0.2.3/LICENSE
+-rw-r--r--   0        0        0      341 2023-08-04 08:09:00.495259 supafunc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-08-04 08:09:09.917494 supafunc-0.2.3/supafunc/__init__.py
+-rw-r--r--   0        0        0     1902 2023-08-04 08:08:21.384347 supafunc-0.2.3/supafunc/functions_client.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 supafunc-0.2.3/PKG-INFO
```

### Comparing `supafunc-0.2.2/LICENSE` & `supafunc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supafunc-0.2.2/supafunc/functions_client.py` & `supafunc-0.2.3/supafunc/functions_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def set_auth(self, token: str) -> None:
         """Updates the authorization header
 
         Parameters
         ----------
         token : str
-            the new jwt token sent in the authorisation header
+            the new jwt token sent in the authorization header
         """
 
         self.headers["Authorization"] = f"Bearer {token}"
 
     async def invoke(self, function_name: str, invoke_options: Dict) -> Dict:
         """Invokes a function
```

### Comparing `supafunc-0.2.2/PKG-INFO` & `supafunc-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: supafunc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Library for Supabase Functions
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
```

