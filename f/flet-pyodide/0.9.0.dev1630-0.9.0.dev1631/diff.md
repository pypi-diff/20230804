# Comparing `tmp/flet_pyodide-0.9.0.dev1630.tar.gz` & `tmp/flet_pyodide-0.9.0.dev1631.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.9.0.dev1630.tar", max compression
+gzip compressed data, was "flet_pyodide-0.9.0.dev1631.tar", max compression
```

## Comparing `flet_pyodide-0.9.0.dev1630.tar` & `flet_pyodide-0.9.0.dev1631.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/README.md
--rw-r--r--   0        0        0      644 2023-08-02 21:47:43.614242 flet_pyodide-0.9.0.dev1630/pyproject.toml
--rw-r--r--   0        0        0       61 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2285 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-08-02 21:47:06.476835 flet_pyodide-0.9.0.dev1630/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1630/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/README.md
+-rw-r--r--   0        0        0      644 2023-08-04 18:59:18.585171 flet_pyodide-0.9.0.dev1631/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2285 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-08-04 18:58:41.311380 flet_pyodide-0.9.0.dev1631/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1631/PKG-INFO
```

### Comparing `flet_pyodide-0.9.0.dev1630/README.md` & `flet_pyodide-0.9.0.dev1631/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1630/pyproject.toml` & `flet_pyodide-0.9.0.dev1631/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.9.0.dev1630"
+version = "0.9.0.dev1631"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.9.0.dev1630"
+flet-core = "0.9.0.dev1631"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.9.0.dev1630/src/flet/flet.py` & `flet_pyodide-0.9.0.dev1631/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1630/src/flet/pyodide_connection.py` & `flet_pyodide-0.9.0.dev1631/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1630/PKG-INFO` & `flet_pyodide-0.9.0.dev1631/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.9.0.dev1630
+Version: 0.9.0.dev1631
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.9.0.dev1630)
+Requires-Dist: flet-core (==0.9.0.dev1631)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

