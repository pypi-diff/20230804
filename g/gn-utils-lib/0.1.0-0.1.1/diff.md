# Comparing `tmp/gn_utils_lib-0.1.0.tar.gz` & `tmp/gn_utils_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn_utils_lib-0.1.0.tar", max compression
+gzip compressed data, was "gn_utils_lib-0.1.1.tar", max compression
```

## Comparing `gn_utils_lib-0.1.0.tar` & `gn_utils_lib-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1491 2023-08-04 19:47:38.281885 gn_utils_lib-0.1.0/LICENSE
--rw-r--r--   0        0        0     3975 2023-08-04 19:47:38.461104 gn_utils_lib-0.1.0/README.md
--rw-r--r--   0        0        0     1596 2023-08-04 20:21:36.494213 gn_utils_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-21 15:31:23.218561 gn_utils_lib-0.1.0/src/gn_py_tracker/__init__.py
--rw-r--r--   0        0        0     1951 2023-08-04 19:54:32.269689 gn_utils_lib-0.1.0/src/gn_py_tracker/event.py
--rw-r--r--   0        0        0     3209 2023-08-04 19:56:38.037680 gn_utils_lib-0.1.0/src/gn_py_tracker/tracker.py
--rw-r--r--   0        0        0        0 2023-08-04 20:14:04.928382 gn_utils_lib-0.1.0/src/ninja_snake_lib/__init__.py
--rw-r--r--   0        0        0     1508 2023-08-04 19:54:32.266504 gn_utils_lib-0.1.0/src/ninja_snake_lib/decorators.py
--rw-r--r--   0        0        0     6167 2023-08-04 19:57:59.855619 gn_utils_lib-0.1.0/src/ninja_snake_lib/json_formatter.py
--rw-r--r--   0        0        0      770 2023-08-04 19:47:40.145907 gn_utils_lib-0.1.0/src/ninja_snake_lib/read_dotenv.py
--rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 gn_utils_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-08-04 19:47:38.281885 gn_utils_lib-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3975 2023-08-04 19:47:38.461104 gn_utils_lib-0.1.1/README.md
+-rw-r--r--   0        0        0     1670 2023-08-04 20:34:16.640039 gn_utils_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-21 15:31:23.218561 gn_utils_lib-0.1.1/src/gn_py_tracker/__init__.py
+-rw-r--r--   0        0        0     1951 2023-08-04 19:54:32.269689 gn_utils_lib-0.1.1/src/gn_py_tracker/event.py
+-rw-r--r--   0        0        0     3209 2023-08-04 19:56:38.037680 gn_utils_lib-0.1.1/src/gn_py_tracker/tracker.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:14:04.928382 gn_utils_lib-0.1.1/src/ninja_snake_lib/__init__.py
+-rw-r--r--   0        0        0     1508 2023-08-04 19:54:32.266504 gn_utils_lib-0.1.1/src/ninja_snake_lib/decorators.py
+-rw-r--r--   0        0        0     6167 2023-08-04 19:57:59.855619 gn_utils_lib-0.1.1/src/ninja_snake_lib/json_formatter.py
+-rw-r--r--   0        0        0      770 2023-08-04 19:47:40.145907 gn_utils_lib-0.1.1/src/ninja_snake_lib/read_dotenv.py
+-rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 gn_utils_lib-0.1.1/PKG-INFO
```

### Comparing `gn_utils_lib-0.1.0/LICENSE` & `gn_utils_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/README.md` & `gn_utils_lib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/pyproject.toml` & `gn_utils_lib-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "gn-utils-lib"
-version = "0.1.0"
+version = "0.1.1"
 description = "Biblioteca utilitaria para projetos Python no Getninjas"
 authors = [
+    "Goncalo Franco <goncalo.franco@getninjas.com.br>",
+]
+maintainers = [
     "Carlos Sa <carlos.sa@getninjas.com.br>",
     "Bruno Scherer <bruno.scherer@getninjas.com.br>",
     "Goncalo Franco <goncalo.franco@getninjas.com.br>",
 ]
 license = "BSD"
 readme = "README.md"
 packages = [
```

### Comparing `gn_utils_lib-0.1.0/src/gn_py_tracker/event.py` & `gn_utils_lib-0.1.1/src/gn_py_tracker/event.py`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/src/gn_py_tracker/tracker.py` & `gn_utils_lib-0.1.1/src/gn_py_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/src/ninja_snake_lib/decorators.py` & `gn_utils_lib-0.1.1/src/ninja_snake_lib/decorators.py`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/src/ninja_snake_lib/json_formatter.py` & `gn_utils_lib-0.1.1/src/ninja_snake_lib/json_formatter.py`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/src/ninja_snake_lib/read_dotenv.py` & `gn_utils_lib-0.1.1/src/ninja_snake_lib/read_dotenv.py`

 * *Files identical despite different names*

### Comparing `gn_utils_lib-0.1.0/PKG-INFO` & `gn_utils_lib-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gn-utils-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Biblioteca utilitaria para projetos Python no Getninjas
 License: BSD
-Author: Carlos Sa
-Author-email: carlos.sa@getninjas.com.br
+Author: Goncalo Franco
+Author-email: goncalo.franco@getninjas.com.br
+Maintainer: Carlos Sa
+Maintainer-email: carlos.sa@getninjas.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

