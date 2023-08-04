# Comparing `tmp/xata-1.0.0a5.tar.gz` & `tmp/xata-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.0.0a5.tar", max compression
+gzip compressed data, was "xata-1.0.0a6.tar", max compression
```

## Comparing `xata-1.0.0a5.tar` & `xata-1.0.0a6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-08-03 12:30:56.384654 xata-1.0.0a5/LICENSE
--rw-r--r--   0        0        0     1083 2023-08-03 12:30:56.384654 xata-1.0.0a5/README.md
--rw-r--r--   0        0        0      818 2023-08-03 12:30:56.416654 xata-1.0.0a5/pyproject.toml
--rw-r--r--   0        0        0      873 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/__init__.py
--rw-r--r--   0        0        0      769 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/__init__.py
--rw-r--r--   0        0        0     2995 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/authentication.py
--rw-r--r--   0        0        0    13898 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/branch.py
--rw-r--r--   0        0        0     8389 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/databases.py
--rw-r--r--   0        0        0     8962 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/files.py
--rw-r--r--   0        0        0     6742 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/invites.py
--rw-r--r--   0        0        0    13228 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/migrations.py
--rw-r--r--   0        0        0    13684 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/records.py
--rw-r--r--   0        0        0    33149 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/search_and_filter.py
--rw-r--r--   0        0        0    13796 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/table.py
--rw-r--r--   0        0        0     2771 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/users.py
--rw-r--r--   0        0        0     8262 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api/workspaces.py
--rw-r--r--   0        0        0     3080 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api_request.py
--rw-r--r--   0        0        0     3186 2023-08-03 12:30:56.448654 xata-1.0.0a5/xata/api_response.py
--rw-r--r--   0        0        0    13444 2023-08-03 12:30:56.452654 xata-1.0.0a5/xata/client.py
--rw-r--r--   0        0        0     1188 2023-08-03 12:30:56.452654 xata-1.0.0a5/xata/errors.py
--rw-r--r--   0        0        0    15894 2023-08-03 12:30:56.452654 xata-1.0.0a5/xata/helpers.py
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 xata-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 14:00:46.126982 xata-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0     1083 2023-08-03 14:00:46.126982 xata-1.0.0a6/README.md
+-rw-r--r--   0        0        0      822 2023-08-03 14:00:46.154984 xata-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/__init__.py
+-rw-r--r--   0        0        0     2995 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/authentication.py
+-rw-r--r--   0        0        0    13898 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/branch.py
+-rw-r--r--   0        0        0     8389 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/databases.py
+-rw-r--r--   0        0        0     8962 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/files.py
+-rw-r--r--   0        0        0     6742 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/invites.py
+-rw-r--r--   0        0        0    13228 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/migrations.py
+-rw-r--r--   0        0        0    13684 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/records.py
+-rw-r--r--   0        0        0    33149 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    13796 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/table.py
+-rw-r--r--   0        0        0     2771 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/users.py
+-rw-r--r--   0        0        0     8262 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/workspaces.py
+-rw-r--r--   0        0        0     3080 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api_request.py
+-rw-r--r--   0        0        0     3186 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api_response.py
+-rw-r--r--   0        0        0    13444 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/errors.py
+-rw-r--r--   0        0        0    15894 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/helpers.py
+-rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 xata-1.0.0a6/PKG-INFO
```

### Comparing `xata-1.0.0a5/LICENSE` & `xata-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/README.md` & `xata-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/pyproject.toml` & `xata-1.0.0a6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "xata"
-version = "1.0.0a5"
+version = "1.0.0a6"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
-python-dotenv = "^0.21.0"
+python-dotenv = ">=0.21,<2.0"
 orjson = "^3.8.1"
 deprecation = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 black = "^22.12.0"
```

### Comparing `xata-1.0.0a5/xata/__init__.py` & `xata-1.0.0a6/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/__init__.py` & `xata-1.0.0a6/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/authentication.py` & `xata-1.0.0a6/xata/api/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/branch.py` & `xata-1.0.0a6/xata/api/branch.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/databases.py` & `xata-1.0.0a6/xata/api/databases.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/files.py` & `xata-1.0.0a6/xata/api/files.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/invites.py` & `xata-1.0.0a6/xata/api/invites.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/migrations.py` & `xata-1.0.0a6/xata/api/migrations.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/records.py` & `xata-1.0.0a6/xata/api/records.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/search_and_filter.py` & `xata-1.0.0a6/xata/api/search_and_filter.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/table.py` & `xata-1.0.0a6/xata/api/table.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/users.py` & `xata-1.0.0a6/xata/api/users.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api/workspaces.py` & `xata-1.0.0a6/xata/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api_request.py` & `xata-1.0.0a6/xata/api_request.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/api_response.py` & `xata-1.0.0a6/xata/api_response.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/client.py` & `xata-1.0.0a6/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .api.search_and_filter import SearchAndFilter
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.0.0a5"
+__version__ = "1.0.0a6"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
```

### Comparing `xata-1.0.0a5/xata/errors.py` & `xata-1.0.0a6/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/xata/helpers.py` & `xata-1.0.0a6/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a5/PKG-INFO` & `xata-1.0.0a6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: orjson (>=3.8.1,<4.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=0.21,<2.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://xata-py.readthedocs.io
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="./assets/logo_dark.svg">
```

