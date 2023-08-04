# Comparing `tmp/propertize-0.0.2.tar.gz` & `tmp/propertize-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propertize-0.0.2.tar", last modified: Fri Aug  4 11:20:00 2023, max compression
+gzip compressed data, was "propertize-0.0.3.tar", last modified: Fri Aug  4 11:42:55 2023, max compression
```

## Comparing `propertize-0.0.2.tar` & `propertize-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:20:00.411270 propertize-0.0.2/
--rw-rw-r--   0 philip    (1000) philip    (1000)     1069 2023-07-12 09:20:03.000000 propertize-0.0.2/LICENSE
--rw-rw-r--   0 philip    (1000) philip    (1000)      667 2023-08-04 11:20:00.411270 propertize-0.0.2/PKG-INFO
--rw-rw-r--   0 philip    (1000) philip    (1000)        0 2023-07-12 10:01:30.000000 propertize-0.0.2/README.md
--rw-rw-r--   0 philip    (1000) philip    (1000)      103 2023-07-12 10:07:37.000000 propertize-0.0.2/pyproject.toml
--rw-rw-r--   0 philip    (1000) philip    (1000)       38 2023-08-04 11:20:00.411270 propertize-0.0.2/setup.cfg
--rw-rw-r--   0 philip    (1000) philip    (1000)     1205 2023-08-04 11:19:14.000000 propertize-0.0.2/setup.py
-drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:20:00.411270 propertize-0.0.2/src/
-drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:20:00.411270 propertize-0.0.2/src/propertize/
--rw-rw-r--   0 philip    (1000) philip    (1000)       26 2023-07-12 09:25:29.000000 propertize-0.0.2/src/propertize/__init__.py
--rw-rw-r--   0 philip    (1000) philip    (1000)      268 2023-08-04 11:19:14.000000 propertize-0.0.2/src/propertize/propertize.py
-drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:20:00.411270 propertize-0.0.2/src/propertize.egg-info/
--rw-rw-r--   0 philip    (1000) philip    (1000)      667 2023-08-04 11:20:00.000000 propertize-0.0.2/src/propertize.egg-info/PKG-INFO
--rw-rw-r--   0 philip    (1000) philip    (1000)      249 2023-08-04 11:20:00.000000 propertize-0.0.2/src/propertize.egg-info/SOURCES.txt
--rw-rw-r--   0 philip    (1000) philip    (1000)        1 2023-08-04 11:20:00.000000 propertize-0.0.2/src/propertize.egg-info/dependency_links.txt
--rw-rw-r--   0 philip    (1000) philip    (1000)       11 2023-08-04 11:20:00.000000 propertize-0.0.2/src/propertize.egg-info/top_level.txt
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:42:55.378139 propertize-0.0.3/
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1069 2023-07-12 09:20:03.000000 propertize-0.0.3/LICENSE
+-rw-rw-r--   0 philip    (1000) philip    (1000)      667 2023-08-04 11:42:55.378139 propertize-0.0.3/PKG-INFO
+-rw-rw-r--   0 philip    (1000) philip    (1000)        0 2023-07-12 10:01:30.000000 propertize-0.0.3/README.md
+-rw-rw-r--   0 philip    (1000) philip    (1000)      103 2023-07-12 10:07:37.000000 propertize-0.0.3/pyproject.toml
+-rw-rw-r--   0 philip    (1000) philip    (1000)       38 2023-08-04 11:42:55.378139 propertize-0.0.3/setup.cfg
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1205 2023-08-04 11:42:48.000000 propertize-0.0.3/setup.py
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:42:55.378139 propertize-0.0.3/src/
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:42:55.378139 propertize-0.0.3/src/propertize/
+-rw-rw-r--   0 philip    (1000) philip    (1000)       26 2023-07-12 09:25:29.000000 propertize-0.0.3/src/propertize/__init__.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)      268 2023-08-04 11:42:48.000000 propertize-0.0.3/src/propertize/propertize.py
+drwxrwxr-x   0 philip    (1000) philip    (1000)        0 2023-08-04 11:42:55.378139 propertize-0.0.3/src/propertize.egg-info/
+-rw-rw-r--   0 philip    (1000) philip    (1000)      667 2023-08-04 11:42:55.000000 propertize-0.0.3/src/propertize.egg-info/PKG-INFO
+-rw-rw-r--   0 philip    (1000) philip    (1000)      249 2023-08-04 11:42:55.000000 propertize-0.0.3/src/propertize.egg-info/SOURCES.txt
+-rw-rw-r--   0 philip    (1000) philip    (1000)        1 2023-08-04 11:42:55.000000 propertize-0.0.3/src/propertize.egg-info/dependency_links.txt
+-rw-rw-r--   0 philip    (1000) philip    (1000)       11 2023-08-04 11:42:55.000000 propertize-0.0.3/src/propertize.egg-info/top_level.txt
```

### Comparing `propertize-0.0.2/LICENSE` & `propertize-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propertize-0.0.2/PKG-INFO` & `propertize-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertize
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unwrap custom properties
 Home-page: https://github.com/jnawk/propertize
 Author: Philip Dowie
 Author-email: philip@jnawk.nz
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `propertize-0.0.2/setup.py` & `propertize-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # if on_rtd:
 #     requirements.append('sphinxcontrib-napoleon')
 #     requirements.append('Pallets-Sphinx-Themes')
 
 
 setup(
     name="propertize",
-    version="0.0.2",
+    version="0.0.3",
     author="Philip Dowie",
     author_email="philip@jnawk.nz",
     description="Unwrap custom properties",
     url="https://github.com/jnawk/propertize",
     license="MIT",
     long_description=__doc__,
     package_dir={"": "src"},
```

### Comparing `propertize-0.0.2/src/propertize.egg-info/PKG-INFO` & `propertize-0.0.3/src/propertize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertize
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unwrap custom properties
 Home-page: https://github.com/jnawk/propertize
 Author: Philip Dowie
 Author-email: philip@jnawk.nz
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

