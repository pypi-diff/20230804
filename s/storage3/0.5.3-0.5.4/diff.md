# Comparing `tmp/storage3-0.5.3.tar.gz` & `tmp/storage3-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage3-0.5.3.tar", max compression
+gzip compressed data, was "storage3-0.5.4.tar", max compression
```

## Comparing `storage3-0.5.3.tar` & `storage3-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1147 2023-07-24 20:22:34.982546 storage3-0.5.3/LICENSE
--rw-r--r--   0        0        0      909 2023-07-24 20:22:34.982777 storage3-0.5.3/README.md
--rw-r--r--   0        0        0     1859 2023-07-24 20:23:13.116881 storage3-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      894 2023-07-24 20:22:34.984482 storage3-0.5.3/storage3/__init__.py
--rw-r--r--   0        0        0       61 2023-07-24 20:22:34.984598 storage3-0.5.3/storage3/_async/__init__.py
--rw-r--r--   0        0        0     3984 2023-07-24 20:22:34.984701 storage3-0.5.3/storage3/_async/bucket.py
--rw-r--r--   0        0        0     1367 2023-07-24 20:22:34.984776 storage3-0.5.3/storage3/_async/client.py
--rw-r--r--   0        0        0    12745 2023-07-24 20:22:34.984896 storage3-0.5.3/storage3/_async/file_api.py
--rw-r--r--   0        0        0       59 2023-07-24 20:22:34.985012 storage3-0.5.3/storage3/_sync/__init__.py
--rw-r--r--   0        0        0     3891 2023-07-24 20:22:34.985100 storage3-0.5.3/storage3/_sync/bucket.py
--rw-r--r--   0        0        0     1324 2023-07-24 20:22:34.985173 storage3-0.5.3/storage3/_sync/client.py
--rw-r--r--   0        0        0    12597 2023-07-24 20:22:34.985259 storage3-0.5.3/storage3/_sync/file_api.py
--rw-r--r--   0        0        0      288 2023-07-24 20:22:34.985338 storage3-0.5.3/storage3/constants.py
--rw-r--r--   0        0        0     1828 2023-07-24 20:22:34.985412 storage3-0.5.3/storage3/types.py
--rw-r--r--   0        0        0      308 2023-07-24 20:23:28.507758 storage3-0.5.3/storage3/utils.py
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 storage3-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-08-04 08:19:42.981076 storage3-0.5.4/LICENSE
+-rw-r--r--   0        0        0      909 2023-08-04 08:19:42.981275 storage3-0.5.4/README.md
+-rw-r--r--   0        0        0     1851 2023-08-04 08:20:17.569712 storage3-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      894 2023-08-04 08:19:42.982607 storage3-0.5.4/storage3/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-04 08:19:42.982696 storage3-0.5.4/storage3/_async/__init__.py
+-rw-r--r--   0        0        0     3984 2023-08-04 08:19:42.982789 storage3-0.5.4/storage3/_async/bucket.py
+-rw-r--r--   0        0        0     1367 2023-08-04 08:19:42.982856 storage3-0.5.4/storage3/_async/client.py
+-rw-r--r--   0        0        0    12745 2023-08-04 08:19:42.982957 storage3-0.5.4/storage3/_async/file_api.py
+-rw-r--r--   0        0        0       59 2023-08-04 08:19:42.983058 storage3-0.5.4/storage3/_sync/__init__.py
+-rw-r--r--   0        0        0     3891 2023-08-04 08:19:42.983124 storage3-0.5.4/storage3/_sync/bucket.py
+-rw-r--r--   0        0        0     1324 2023-08-04 08:19:42.983184 storage3-0.5.4/storage3/_sync/client.py
+-rw-r--r--   0        0        0    12597 2023-08-04 08:19:42.983269 storage3-0.5.4/storage3/_sync/file_api.py
+-rw-r--r--   0        0        0      288 2023-08-04 08:19:42.983329 storage3-0.5.4/storage3/constants.py
+-rw-r--r--   0        0        0     1828 2023-08-04 08:19:42.983410 storage3-0.5.4/storage3/types.py
+-rw-r--r--   0        0        0      308 2023-08-04 08:20:08.839568 storage3-0.5.4/storage3/utils.py
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 storage3-0.5.4/PKG-INFO
```

### Comparing `storage3-0.5.3/LICENSE` & `storage3-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/README.md` & `storage3-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/pyproject.toml` & `storage3-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 description = "Supabase Storage client for Python."
 documentation = "https://supabase-community.github.io/storage-py"
 homepage = "https://supabase-community.github.io/storage-py"
 license = "MIT"
 name = "storage3"
 readme = "README.md"
 repository = "https://github.com/supabase-community/storage-py"
-version = "0.5.3"
+version = "0.5.4"
 
 [tool.poetry.dependencies]
-httpx = ">=0.23,<0.25"
+httpx = "^0.24"
 python = "^3.8"
 typing-extensions = "^4.2.0"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
-python-semantic-release = "^7.33.2"
+python-semantic-release = "^8.0.4"
 black = "^23.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
 python-dotenv = "^1.0.0"
-Sphinx = "^7.0.1"
+Sphinx = "^7.1.2"
 sphinx-press-theme = "^0.8.0"
 unasync-cli = "^0.0.9"
 
 [tool.poetry.group.dev.dependencies]
 sphinx-toolbox = "^3.4.0"
 
 [tool.semantic_release]
```

### Comparing `storage3-0.5.3/storage3/__init__.py` & `storage3-0.5.4/storage3/__init__.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_async/bucket.py` & `storage3-0.5.4/storage3/_async/bucket.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_async/client.py` & `storage3-0.5.4/storage3/_async/client.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_async/file_api.py` & `storage3-0.5.4/storage3/_async/file_api.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_sync/bucket.py` & `storage3-0.5.4/storage3/_sync/bucket.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_sync/client.py` & `storage3-0.5.4/storage3/_sync/client.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/_sync/file_api.py` & `storage3-0.5.4/storage3/_sync/file_api.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/storage3/types.py` & `storage3-0.5.4/storage3/types.py`

 * *Files identical despite different names*

### Comparing `storage3-0.5.3/PKG-INFO` & `storage3-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: storage3
-Version: 0.5.3
+Version: 0.5.4
 Summary: Supabase Storage client for Python.
 Home-page: https://supabase-community.github.io/storage-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23,<0.25)
+Requires-Dist: httpx (>=0.24,<0.25)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Project-URL: Documentation, https://supabase-community.github.io/storage-py
 Project-URL: Repository, https://github.com/supabase-community/storage-py
 Description-Content-Type: text/markdown
 
 # Storage-py
```

