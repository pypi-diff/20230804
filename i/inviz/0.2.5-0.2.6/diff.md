# Comparing `tmp/inviz-0.2.5.tar.gz` & `tmp/inviz-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.5.tar", last modified: Fri Aug  4 04:41:17 2023, max compression
+gzip compressed data, was "inviz-0.2.6.tar", last modified: Fri Aug  4 05:10:46 2023, max compression
```

## Comparing `inviz-0.2.5.tar` & `inviz-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.619294 inviz-0.2.5/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.5/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.5/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 04:41:17.609294 inviz-0.2.5/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.5/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.609294 inviz-0.2.5/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.609294 inviz-0.2.5/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.5/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-04 04:41:17.619294 inviz-0.2.5/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1180 2023-08-04 04:36:54.000000 inviz-0.2.5/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.6/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.6/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:10:46.699131 inviz-0.2.6/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.6/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 05:10:46.699131 inviz-0.2.6/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-04 05:10:46.000000 inviz-0.2.6/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.6/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-04 05:10:46.699131 inviz-0.2.6/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1227 2023-08-04 05:10:33.000000 inviz-0.2.6/setup.py
```

### Comparing `inviz-0.2.5/LICENSE` & `inviz-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.5/PKG-INFO` & `inviz-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.5
+Version: 0.2.6
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.5/README.md` & `inviz-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.5/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.6/inviz/inviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.5
+Version: 0.2.6
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.5/inviz/inviz.py` & `inviz-0.2.6/inviz/inviz.py`

 * *Files identical despite different names*

