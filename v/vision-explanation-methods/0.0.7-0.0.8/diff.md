# Comparing `tmp/vision_explanation_methods-0.0.7.tar.gz` & `tmp/vision_explanation_methods-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_explanation_methods-0.0.7.tar", last modified: Thu May  4 16:07:01 2023, max compression
+gzip compressed data, was "vision_explanation_methods-0.0.8.tar", last modified: Fri Aug  4 15:02:37 2023, max compression
```

## Comparing `vision_explanation_methods-0.0.7.tar` & `vision_explanation_methods-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.806374 vision_explanation_methods-0.0.7/vision_explanation_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/DRISE_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.810374 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/drise.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 15:38:13.000000 vision_explanation_methods-0.0.7/vision_explanation_methods/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:07:01.806374 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 16:07:01.000000 vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.932467 vision_explanation_methods-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-04 15:02:37.932467 vision_explanation_methods-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:02:37.932467 vision_explanation_methods-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.928467 vision_explanation_methods-0.0.8/vision_explanation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/DRISE_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.928467 vision_explanation_methods-0.0.8/vision_explanation_methods/error_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/error_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/error_labeling/error_labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.928467 vision_explanation_methods-0.0.8/vision_explanation_methods/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/evaluation/pointing_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.932467 vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/drise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-04 14:38:21.000000 vision_explanation_methods-0.0.8/vision_explanation_methods/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:02:37.928467 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 15:02:37.000000 vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/top_level.txt
```

### Comparing `vision_explanation_methods-0.0.7/LICENSE.txt` & `vision_explanation_methods-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/PKG-INFO` & `vision_explanation_methods-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_explanation_methods
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.7/README.md` & `vision_explanation_methods-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/setup.py` & `vision_explanation_methods-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/vision_explanation_methods/DRISE_runner.py` & `vision_explanation_methods-0.0.8/vision_explanation_methods/DRISE_runner.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/common.py` & `vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/common.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/vision_explanation_methods/explanations/drise.py` & `vision_explanation_methods-0.0.8/vision_explanation_methods/explanations/drise.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.7/vision_explanation_methods.egg-info/PKG-INFO` & `vision_explanation_methods-0.0.8/vision_explanation_methods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-explanation-methods
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

