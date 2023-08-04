# Comparing `tmp/mamon_utils-0.0.4.tar.gz` & `tmp/mamon_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamon_utils-0.0.4.tar", max compression
+gzip compressed data, was "mamon_utils-0.1.0.tar", max compression
```

## Comparing `mamon_utils-0.0.4.tar` & `mamon_utils-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1568 2023-08-03 22:55:55.001531 mamon_utils-0.0.4/README_PYPI.md
--rw-r--r--   0        0        0      111 2023-08-03 22:07:36.994336 mamon_utils-0.0.4/mamonutils/__init__.py
--rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.4/mamonutils/db.py
--rw-r--r--   0        0        0      828 2023-08-03 22:35:15.239076 mamon_utils-0.0.4/mamonutils/image_dimensions.py
--rw-r--r--   0        0        0      488 2023-08-03 22:56:14.781171 mamon_utils-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 mamon_utils-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1568 2023-08-04 09:30:29.837069 mamon_utils-0.1.0/README_PYPI.md
+-rw-r--r--   0        0        0      111 2023-08-04 09:30:29.837069 mamon_utils-0.1.0/mamonutils/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.1.0/mamonutils/db.py
+-rw-r--r--   0        0        0      828 2023-08-04 09:30:29.837069 mamon_utils-0.1.0/mamonutils/image_dimensions.py
+-rw-r--r--   0        0        0      488 2023-08-04 16:46:35.929055 mamon_utils-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 mamon_utils-0.1.0/PKG-INFO
```

### Comparing `mamon_utils-0.0.4/README_PYPI.md` & `mamon_utils-0.1.0/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.4/mamonutils/db.py` & `mamon_utils-0.1.0/mamonutils/db.py`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.4/mamonutils/image_dimensions.py` & `mamon_utils-0.1.0/mamonutils/image_dimensions.py`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.4/PKG-INFO` & `mamon_utils-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mamon-utils
-Version: 0.0.4
+Version: 0.1.0
 Summary: Common Mamon11 tools and utilities
 Author: WessCoby
 Author-email: wc@wesscoby.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: psycopg2-binary (==2.9.5)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

