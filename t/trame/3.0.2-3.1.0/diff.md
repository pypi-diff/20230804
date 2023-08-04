# Comparing `tmp/trame-3.0.2.tar.gz` & `tmp/trame-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-3.0.2.tar", last modified: Thu Jul 20 23:45:35 2023, max compression
+gzip compressed data, was "trame-3.1.0.tar", last modified: Fri Aug  4 01:06:14 2023, max compression
```

## Comparing `trame-3.0.2.tar` & `trame-3.1.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 23:45:30.000000 trame-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 23:45:30.000000 trame-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 23:45:35.082388 trame-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6111 2023-07-20 23:45:30.000000 trame-3.0.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-20 23:45:35.082388 trame-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 23:45:30.000000 trame-3.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.078388 trame-3.0.2/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-20 23:45:30.000000 trame-3.0.2/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-20 23:45:30.000000 trame-3.0.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/app/
--rw-r--r--   0 root         (0) root         (0)     4988 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-07-20 23:45:30.000000 trame-3.0.2/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:45:30.000000 trame-3.0.2/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-07-20 23:45:30.000000 trame-3.0.2/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-07-20 23:45:30.000000 trame-3.0.2/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:45:30.000000 trame-3.0.2/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-20 23:45:30.000000 trame-3.0.2/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-07-20 23:45:30.000000 trame-3.0.2/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-20 23:45:30.000000 trame-3.0.2/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:45:30.000000 trame-3.0.2/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:45:30.000000 trame-3.0.2/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-20 23:45:30.000000 trame-3.0.2/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-07-20 23:45:30.000000 trame-3.0.2/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-20 23:45:30.000000 trame-3.0.2/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.082388 trame-3.0.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:45:30.000000 trame-3.0.2/trame/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:45:35.078388 trame-3.0.2/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6849 2023-07-20 23:45:35.000000 trame-3.0.2/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-07-20 23:45:35.000000 trame-3.0.2/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 23:45:35.000000 trame-3.0.2/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 23:45:35.000000 trame-3.0.2/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 23:45:35.000000 trame-3.0.2/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-04 01:06:10.000000 trame-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 01:06:10.000000 trame-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-08-04 01:06:14.792469 trame-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-08-04 01:06:10.000000 trame-3.1.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      922 2023-08-04 01:06:14.792469 trame-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 01:06:10.000000 trame-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.788469 trame-3.1.0/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-04 01:06:10.000000 trame-3.1.0/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 01:06:10.000000 trame-3.1.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.788469 trame-3.1.0/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-08-04 01:06:10.000000 trame-3.1.0/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 01:06:10.000000 trame-3.1.0/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2023-08-04 01:06:10.000000 trame-3.1.0/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-08-04 01:06:10.000000 trame-3.1.0/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/decorators/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-08-04 01:06:10.000000 trame-3.1.0/trame/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       86 2023-08-04 01:06:10.000000 trame-3.1.0/trame/decorators/dev.py
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-08-04 01:06:10.000000 trame-3.1.0/trame/decorators/klass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 01:06:10.000000 trame-3.1.0/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-08-04 01:06:10.000000 trame-3.1.0/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-08-04 01:06:10.000000 trame-3.1.0/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-08-04 01:06:10.000000 trame-3.1.0/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 01:06:10.000000 trame-3.1.0/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 01:06:10.000000 trame-3.1.0/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-08-04 01:06:10.000000 trame-3.1.0/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-08-04 01:06:10.000000 trame-3.1.0/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-08-04 01:06:10.000000 trame-3.1.0/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.792469 trame-3.1.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 01:06:10.000000 trame-3.1.0/trame/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 01:06:14.788469 trame-3.1.0/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-08-04 01:06:14.000000 trame-3.1.0/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      786 2023-08-04 01:06:14.000000 trame-3.1.0/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 01:06:14.000000 trame-3.1.0/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-04 01:06:14.000000 trame-3.1.0/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-04 01:06:14.000000 trame-3.1.0/trame.egg-info/top_level.txt
```

### Comparing `trame-3.0.2/LICENSE` & `trame-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/PKG-INFO` & `trame-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.0.2
+Version: 3.1.0
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.0.2/README.rst` & `trame-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/setup.cfg` & `trame-3.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 3.0.2
+version = 3.1.0
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-3.0.2/trame/LICENSE` & `trame-3.1.0/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/__init__.py` & `trame-3.1.0/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/demo.py` & `trame-3.1.0/trame/app/demo.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/dev.py` & `trame-3.1.0/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/file_upload.py` & `trame-3.1.0/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/jupyter.py` & `trame-3.1.0/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/mimetypes.py` & `trame-3.1.0/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/singleton.py` & `trame-3.1.0/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/app/testing.py` & `trame-3.1.0/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/assets/local.py` & `trame-3.1.0/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/assets/remote.py` & `trame-3.1.0/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/env/paraview.py` & `trame-3.1.0/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/env/utils.py` & `trame-3.1.0/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/env/venv.py` & `trame-3.1.0/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/tools/app.py` & `trame-3.1.0/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame/tools/www.py` & `trame-3.1.0/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-3.0.2/trame.egg-info/PKG-INFO` & `trame-3.1.0/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.0.2
+Version: 3.1.0
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.0.2/trame.egg-info/SOURCES.txt` & `trame-3.1.0/trame.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 trame/app/jupyter.py
 trame/app/mimetypes.py
 trame/app/singleton.py
 trame/app/testing.py
 trame/assets/__init__.py
 trame/assets/local.py
 trame/assets/remote.py
+trame/decorators/__init__.py
+trame/decorators/dev.py
+trame/decorators/klass.py
 trame/env/__init__.py
 trame/env/paraview.py
 trame/env/utils.py
 trame/env/venv.py
 trame/modules/__init__.py
 trame/tools/__init__.py
 trame/tools/app.py
```

