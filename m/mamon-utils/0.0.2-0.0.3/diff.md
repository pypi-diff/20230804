# Comparing `tmp/mamon_utils-0.0.2.tar.gz` & `tmp/mamon_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamon_utils-0.0.2.tar", max compression
+gzip compressed data, was "mamon_utils-0.0.3.tar", max compression
```

## Comparing `mamon_utils-0.0.2.tar` & `mamon_utils-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      736 2023-07-18 23:03:34.398485 mamon_utils-0.0.2/README_PYPI.md
--rw-r--r--   0        0        0       66 2023-07-18 22:35:53.627917 mamon_utils-0.0.2/mamonutils/__init__.py
--rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.2/mamonutils/db.py
--rw-r--r--   0        0        0      392 2023-07-21 19:02:08.220996 mamon_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 mamon_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      736 2023-07-18 23:03:34.398485 mamon_utils-0.0.3/README_PYPI.md
+-rw-r--r--   0        0        0      111 2023-08-03 22:07:36.994336 mamon_utils-0.0.3/mamonutils/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.3/mamonutils/db.py
+-rw-r--r--   0        0        0      828 2023-08-03 22:35:15.239076 mamon_utils-0.0.3/mamonutils/image_dimensions.py
+-rw-r--r--   0        0        0      488 2023-08-03 22:36:03.665519 mamon_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 mamon_utils-0.0.3/PKG-INFO
```

### Comparing `mamon_utils-0.0.2/README_PYPI.md` & `mamon_utils-0.0.3/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.2/mamonutils/db.py` & `mamon_utils-0.0.3/mamonutils/db.py`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.2/PKG-INFO` & `mamon_utils-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: mamon-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Common Mamon11 tools and utilities
 Author: WessCoby
 Author-email: wc@wesscoby.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: psycopg2-binary (==2.9.5)
 Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Mamon Utilities
 
 A set of tools and utilities for Python Development
 
 ## Installation
```

