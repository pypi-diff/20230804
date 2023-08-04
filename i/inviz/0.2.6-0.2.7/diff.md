# Comparing `tmp/inviz-0.2.6.tar.gz` & `tmp/inviz-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.6.tar", last modified: Fri Aug  4 05:10:46 2023, max compression
+gzip compressed data, was "inviz-0.2.7.tar", last modified: Fri Aug  4 05:18:03 2023, max compression
```

## Comparing `inviz-0.2.6.tar` & `inviz-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.6/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.6/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:10:46.699131 inviz-0.2.6/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.6/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.6/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-04 05:10:46.699131 inviz-0.2.6/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1227 2023-08-04 05:10:33.000000 inviz-0.2.6/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:18:03.719075 inviz-0.2.7/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.7/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.7/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:18:03.719075 inviz-0.2.7/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.7/README.md
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-04 05:18:03.719075 inviz-0.2.7/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1194 2023-08-04 05:17:57.000000 inviz-0.2.7/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:18:03.719075 inviz-0.2.7/src/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:18:03.719075 inviz-0.2.7/src/inviz/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:36:54.000000 inviz-0.2.7/src/inviz/__init__.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:18:03.719075 inviz-0.2.7/src/inviz/cosmo/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:36:54.000000 inviz-0.2.7/src/inviz/cosmo/__init__.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2605 2023-08-04 04:36:54.000000 inviz-0.2.7/src/inviz/cosmo/cosmo.py
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.7/src/inviz/inviz.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:18:03.719075 inviz-0.2.7/src/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:18:03.000000 inviz-0.2.7/src/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      296 2023-08-04 05:18:03.000000 inviz-0.2.7/src/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-04 05:18:03.000000 inviz-0.2.7/src/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-04 05:18:03.000000 inviz-0.2.7/src/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-04 05:18:03.000000 inviz-0.2.7/src/inviz.egg-info/top_level.txt
```

### Comparing `inviz-0.2.6/LICENSE` & `inviz-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.6/PKG-INFO` & `inviz-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.6
+Version: 0.2.7
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.6/README.md` & `inviz-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.6/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.7/src/inviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.6
+Version: 0.2.7
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.6/inviz/inviz.py` & `inviz-0.2.7/src/inviz/inviz.py`

 * *Files identical despite different names*

### Comparing `inviz-0.2.6/setup.py` & `inviz-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.6",
+    version = "0.2.7",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
-    py_modules=["inviz"],
-    package_dir={'': 'inviz',
-                 'inviz.cosmo': 'inviz/cosmo'},
+#     py_modules=["inviz"],
+#     package_dir={'': 'inviz',
+#                  'inviz.cosmo': 'inviz/cosmo'},
 #    packages=['inviz'],
-    #package_dir={'': 'inviz'},
-    #long_description=long_description,
+#     package_dir={'': 'inviz'},
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
```

