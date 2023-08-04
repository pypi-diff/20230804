# Comparing `tmp/synerty-peek-3.4.8.tar.gz` & `tmp/synerty-peek-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synerty-peek-3.4.8.tar", last modified: Tue Jul 11 02:53:17 2023, max compression
+gzip compressed data, was "synerty-peek-3.4.9.tar", last modified: Wed Jul 19 06:51:57 2023, max compression
```

## Comparing `synerty-peek-3.4.8.tar` & `synerty-peek-3.4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:17.546964 synerty-peek-3.4.8/
--rw-r--r--   0 root         (0) root         (0)      462 2023-07-11 02:53:17.546964 synerty-peek-3.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2984 2023-07-11 02:51:12.000000 synerty-peek-3.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:17.545964 synerty-peek-3.4.8/peek/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-11 02:51:12.000000 synerty-peek-3.4.8/peek/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-11 02:53:17.555964 synerty-peek-3.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2051 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:17.545964 synerty-peek-3.4.8/synerty_peek.egg-info/
--rw-r--r--   0 root         (0) root         (0)      462 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      802 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-11 02:53:17.000000 synerty-peek-3.4.8/synerty_peek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:57.486026 synerty-peek-3.4.9/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-07-19 06:51:57.486026 synerty-peek-3.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-07-19 06:49:48.000000 synerty-peek-3.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:57.486026 synerty-peek-3.4.9/peek/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-19 06:49:49.000000 synerty-peek-3.4.9/peek/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-19 06:51:57.496026 synerty-peek-3.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:57.486026 synerty-peek-3.4.9/synerty_peek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      802 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-19 06:51:57.000000 synerty-peek-3.4.9/synerty_peek.egg-info/top_level.txt
```

### Comparing `synerty-peek-3.4.8/README.rst` & `synerty-peek-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `synerty-peek-3.4.8/setup.py` & `synerty-peek-3.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from setuptools import find_packages, setup
 
 pip_package_name = "synerty-peek"
-package_version = "3.4.8"
+package_version = "3.4.9"
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

### Comparing `synerty-peek-3.4.8/synerty_peek.egg-info/requires.txt` & `synerty-peek-3.4.9/synerty_peek.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-peek-admin-doc==3.4.*,>=3.4.8
-peek-admin-app==3.4.*,>=3.4.8
-peek-agent-service==3.4.*,>=3.4.8
-peek-core-device==3.4.*,>=3.4.8
-peek-core-docdb==3.4.*,>=3.4.8
-peek-core-email==3.4.*,>=3.4.8
-peek-core-search==3.4.*,>=3.4.8
-peek-core-user==3.4.*,>=3.4.8
-peek-core-screen==3.4.*,>=3.4.8
-peek-field-doc==3.4.*,>=3.4.8
-peek-field-app==3.4.*,>=3.4.8
-peek-field-service==3.4.*,>=3.4.8
-peek-logic-service==3.4.*,>=3.4.8
-peek-office-doc==3.4.*,>=3.4.8
-peek-office-app==3.4.*,>=3.4.8
-peek-office-service==3.4.*,>=3.4.8
-peek-platform==3.4.*,>=3.4.8
-peek-plugin-base==3.4.*,>=3.4.8
-peek-storage-service==3.4.*,>=3.4.8
-peek-worker-service==3.4.*,>=3.4.8
-peek-abstract-chunked-index==3.4.*,>=3.4.8
-peek-abstract-chunked-data-loader==3.4.*,>=3.4.8
+peek-admin-doc==3.4.*,>=3.4.9
+peek-admin-app==3.4.*,>=3.4.9
+peek-agent-service==3.4.*,>=3.4.9
+peek-core-device==3.4.*,>=3.4.9
+peek-core-docdb==3.4.*,>=3.4.9
+peek-core-email==3.4.*,>=3.4.9
+peek-core-search==3.4.*,>=3.4.9
+peek-core-user==3.4.*,>=3.4.9
+peek-core-screen==3.4.*,>=3.4.9
+peek-field-doc==3.4.*,>=3.4.9
+peek-field-app==3.4.*,>=3.4.9
+peek-field-service==3.4.*,>=3.4.9
+peek-logic-service==3.4.*,>=3.4.9
+peek-office-doc==3.4.*,>=3.4.9
+peek-office-app==3.4.*,>=3.4.9
+peek-office-service==3.4.*,>=3.4.9
+peek-platform==3.4.*,>=3.4.9
+peek-plugin-base==3.4.*,>=3.4.9
+peek-storage-service==3.4.*,>=3.4.9
+peek-worker-service==3.4.*,>=3.4.9
+peek-abstract-chunked-index==3.4.*,>=3.4.9
+peek-abstract-chunked-data-loader==3.4.*,>=3.4.9
 sphinx
 sphinx-rtd-theme
 sphinx-autobuild
 pytmpdir<1.1.0,>=1.0.2
 py-spy
```

