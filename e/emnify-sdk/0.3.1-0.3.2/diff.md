# Comparing `tmp/emnify-sdk-0.3.1.tar.gz` & `tmp/emnify-sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emnify-sdk-0.3.1.tar", last modified: Mon Jun 19 13:12:31 2023, max compression
+gzip compressed data, was "emnify-sdk-0.3.2.tar", last modified: Fri Aug  4 11:25:19 2023, max compression
```

## Comparing `emnify-sdk-0.3.1.tar` & `emnify-sdk-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    11312 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3415 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.662402 emnify-sdk-0.3.1/emnify/
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/api_manager.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/constants.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/emnify.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.662402 emnify-sdk-0.3.1/emnify/modules/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.662402 emnify-sdk-0.3.1/emnify/modules/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96544 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/api/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/emnify/modules/device/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/device/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/device/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)    14053 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/device/manager.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/device/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/emnify/modules/operator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/operator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/operator/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/operator/manager.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/operator/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/emnify/modules/sim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/sim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/sim/api_call_manager.py
--rw-r--r--   0 root         (0) root         (0)     5161 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/sim/manager.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/emnify/modules/sim/models.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-19 13:12:27.000000 emnify-sdk-0.3.1/emnify/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/emnify_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-19 13:12:31.000000 emnify-sdk-0.3.1/emnify_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-06-19 13:12:31.000000 emnify-sdk-0.3.1/emnify_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 13:12:31.000000 emnify-sdk-0.3.1/emnify_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-19 13:12:31.000000 emnify-sdk-0.3.1/emnify_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-19 13:12:31.000000 emnify-sdk-0.3.1/emnify_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-19 13:12:26.000000 emnify-sdk-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:12:31.666402 emnify-sdk-0.3.1/tests/
--rw-r--r--   0 root         (0) root         (0)    11265 2023-06-19 13:11:35.000000 emnify-sdk-0.3.1/tests/test_emnify.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11312 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/api_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/constants.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/emnify.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/modules/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/modules/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96544 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/api/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/modules/device/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/device/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/device/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)    14053 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/device/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/device/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/modules/operator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/operator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/operator/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/operator/manager.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/operator/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify/modules/sim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/sim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/sim/api_call_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/sim/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/emnify/modules/sim/models.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-08-04 11:25:15.000000 emnify-sdk-0.3.2/emnify/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/emnify_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-08-04 11:25:19.000000 emnify-sdk-0.3.2/emnify_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 11:25:19.000000 emnify-sdk-0.3.2/emnify_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 11:25:19.000000 emnify-sdk-0.3.2/emnify_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-08-04 11:25:19.000000 emnify-sdk-0.3.2/emnify_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-04 11:25:19.000000 emnify-sdk-0.3.2/emnify_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-08-04 11:25:15.000000 emnify-sdk-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:25:19.774032 emnify-sdk-0.3.2/tests/
+-rw-r--r--   0 root         (0) root         (0)    11265 2023-08-04 11:24:33.000000 emnify-sdk-0.3.2/tests/test_emnify.py
```

### Comparing `emnify-sdk-0.3.1/LICENSE` & `emnify-sdk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/PKG-INFO` & `emnify-sdk-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emnify-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Supply your swarm of IoT Devices with cloud connectivity by EMnify. Automate your routines with this SDK for Python.
 Home-page: https://github.com/EMnify/emnify-sdk-python
 Author: EMnify
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/EMnify/emnify-sdk-python
 Keywords: Swagger,EMnify Python SDK,IoT
 Requires-Python: >=3.6
```

### Comparing `emnify-sdk-0.3.1/README.md` & `emnify-sdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/api_manager.py` & `emnify-sdk-0.3.2/emnify/api_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/constants.py` & `emnify-sdk-0.3.2/emnify/constants.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/emnify.py` & `emnify-sdk-0.3.2/emnify/emnify.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/errors.py` & `emnify-sdk-0.3.2/emnify/errors.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/api/models.py` & `emnify-sdk-0.3.2/emnify/modules/api/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/device/api_call_manager.py` & `emnify-sdk-0.3.2/emnify/modules/device/api_call_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/device/manager.py` & `emnify-sdk-0.3.2/emnify/modules/device/manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/device/models.py` & `emnify-sdk-0.3.2/emnify/modules/device/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/sim/api_call_manager.py` & `emnify-sdk-0.3.2/emnify/modules/sim/api_call_manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/sim/manager.py` & `emnify-sdk-0.3.2/emnify/modules/sim/manager.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify/modules/sim/models.py` & `emnify-sdk-0.3.2/emnify/modules/sim/models.py`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/emnify_sdk.egg-info/PKG-INFO` & `emnify-sdk-0.3.2/emnify_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emnify-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Supply your swarm of IoT Devices with cloud connectivity by EMnify. Automate your routines with this SDK for Python.
 Home-page: https://github.com/EMnify/emnify-sdk-python
 Author: EMnify
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/EMnify/emnify-sdk-python
 Keywords: Swagger,EMnify Python SDK,IoT
 Requires-Python: >=3.6
```

### Comparing `emnify-sdk-0.3.1/emnify_sdk.egg-info/SOURCES.txt` & `emnify-sdk-0.3.2/emnify_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emnify-sdk-0.3.1/setup.py` & `emnify-sdk-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 from setuptools import setup, find_packages
 import os
 
 NAME = os.getenv('PYPI_PACKAGE_NAME') or "emnify-sdk"
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `emnify-sdk-0.3.1/tests/test_emnify.py` & `emnify-sdk-0.3.2/tests/test_emnify.py`

 * *Files identical despite different names*

