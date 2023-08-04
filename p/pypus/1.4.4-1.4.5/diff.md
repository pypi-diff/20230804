# Comparing `tmp/pypus-1.4.4.tar.gz` & `tmp/pypus-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.4.4.tar", max compression
+gzip compressed data, was "pypus-1.4.5.tar", max compression
```

## Comparing `pypus-1.4.4.tar` & `pypus-1.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.000000 pypus-1.4.4/LICENSE
--rw-r--r--   0        0        0      104 2023-08-01 16:02:31.000000 pypus-1.4.4/README.md
--rw-r--r--   0        0        0      721 2023-08-01 22:36:30.322671 pypus-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      937 2023-07-31 18:46:58.000000 pypus-1.4.4/src/pypus/Octo.py
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.000000 pypus-1.4.4/src/pypus/__init__.py
--rw-r--r--   0        0        0    33379 2023-08-01 21:23:28.000000 pypus-1.4.4/src/pypus/cli.py
--rw-r--r--   0        0        0      601 2023-07-31 21:09:19.000000 pypus-1.4.4/src/pypus/shelf.py
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 pypus-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.000000 pypus-1.4.5/LICENSE
+-rw-r--r--   0        0        0      187 2023-08-04 18:29:55.628423 pypus-1.4.5/README.md
+-rw-r--r--   0        0        0      722 2023-08-04 18:32:38.589366 pypus-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.000000 pypus-1.4.5/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.000000 pypus-1.4.5/src/pypus/__init__.py
+-rw-r--r--   0        0        0    33379 2023-08-01 21:23:28.000000 pypus-1.4.5/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 21:09:19.000000 pypus-1.4.5/src/pypus/shelf.py
+-rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 pypus-1.4.5/PKG-INFO
```

### Comparing `pypus-1.4.4/LICENSE` & `pypus-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.4.4/pyproject.toml` & `pypus-1.4.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pypus"
-version = "1.4.4"
+version = "1.4.5"
 description = "Octopus cli toolkit"
 authors = ["Michael MacKenna <mpmackenna@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://mpmackenna.github.io/pypus"
+homepage = "https://github.com/mpmackenna/pypus"
 documentation = "https://mpmackenna.github.io/pypus"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.25.1"
 click = "^8.0.0"
 termcolor = "^1.1.0"
```

### Comparing `pypus-1.4.4/src/pypus/Octo.py` & `pypus-1.4.5/src/pypus/Octo.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.4/src/pypus/cli.py` & `pypus-1.4.5/src/pypus/cli.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.4/src/pypus/shelf.py` & `pypus-1.4.5/src/pypus/shelf.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.4/PKG-INFO` & `pypus-1.4.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.4.4
+Version: 1.4.5
 Summary: Octopus cli toolkit
-Home-page: https://mpmackenna.github.io/pypus
+Home-page: https://github.com/mpmackenna/pypus
 License: MIT
 Author: Michael MacKenna
 Author-email: mpmackenna@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,7 +25,10 @@
 
 ## Install
 
 ```bash
 $ pip install pypus
 ```
 
+## Documentation
+[GitHub Pages Read the docs](https://mpmackenna.github.io/pypus)
+
```

