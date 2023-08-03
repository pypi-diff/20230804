# Comparing `tmp/mamon_utils-0.0.3.tar.gz` & `tmp/mamon_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamon_utils-0.0.3.tar", max compression
+gzip compressed data, was "mamon_utils-0.0.4.tar", max compression
```

## Comparing `mamon_utils-0.0.3.tar` & `mamon_utils-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      736 2023-07-18 23:03:34.398485 mamon_utils-0.0.3/README_PYPI.md
--rw-r--r--   0        0        0      111 2023-08-03 22:07:36.994336 mamon_utils-0.0.3/mamonutils/__init__.py
--rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.3/mamonutils/db.py
--rw-r--r--   0        0        0      828 2023-08-03 22:35:15.239076 mamon_utils-0.0.3/mamonutils/image_dimensions.py
--rw-r--r--   0        0        0      488 2023-08-03 22:36:03.665519 mamon_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 mamon_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1568 2023-08-03 22:55:55.001531 mamon_utils-0.0.4/README_PYPI.md
+-rw-r--r--   0        0        0      111 2023-08-03 22:07:36.994336 mamon_utils-0.0.4/mamonutils/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-18 22:46:42.155559 mamon_utils-0.0.4/mamonutils/db.py
+-rw-r--r--   0        0        0      828 2023-08-03 22:35:15.239076 mamon_utils-0.0.4/mamonutils/image_dimensions.py
+-rw-r--r--   0        0        0      488 2023-08-03 22:56:14.781171 mamon_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 mamon_utils-0.0.4/PKG-INFO
```

### Comparing `mamon_utils-0.0.3/mamonutils/db.py` & `mamon_utils-0.0.4/mamonutils/db.py`

 * *Files identical despite different names*

### Comparing `mamon_utils-0.0.3/mamonutils/image_dimensions.py` & `mamon_utils-0.0.4/mamonutils/image_dimensions.py`

 * *Files identical despite different names*

