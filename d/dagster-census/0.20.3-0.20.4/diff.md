# Comparing `tmp/dagster-census-0.20.3.tar.gz` & `tmp/dagster-census-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.20.3.tar", last modified: Mon Jul 31 23:05:35 2023, max compression
+gzip compressed data, was "dagster-census-0.20.4.tar", last modified: Thu Aug  3 22:01:27 2023, max compression
```

## Comparing `dagster-census-0.20.3.tar` & `dagster-census-0.20.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:35.104931 dagster-census-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-census-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-31 22:58:19.000000 dagster-census-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-31 23:05:35.104931 dagster-census-0.20.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:35.104931 dagster-census-0.20.3/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10284 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-census-0.20.3/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:35.104931 dagster-census-0.20.3/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 23:05:35.000000 dagster-census-0.20.3/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-31 23:05:35.104931 dagster-census-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-31 22:58:19.000000 dagster-census-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:27.176026 dagster-census-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:41.000000 dagster-census-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-08-03 21:49:41.000000 dagster-census-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-03 22:01:27.176026 dagster-census-0.20.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:27.176026 dagster-census-0.20.4/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-census-0.20.4/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:27.176026 dagster-census-0.20.4/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-03 22:01:27.000000 dagster-census-0.20.4/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-08-03 22:01:27.176026 dagster-census-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-08-03 21:49:41.000000 dagster-census-0.20.4/setup.py
```

### Comparing `dagster-census-0.20.3/LICENSE` & `dagster-census-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.20.3/PKG-INFO` & `dagster-census-0.20.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.20.3/dagster_census/ops.py` & `dagster-census-0.20.4/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.20.3/dagster_census/resources.py` & `dagster-census-0.20.4/dagster_census/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.20.3/dagster_census/types.py` & `dagster-census-0.20.4/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.20.3/dagster_census/utils.py` & `dagster-census-0.20.4/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.20.3/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.20.4/dagster_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.20.3/setup.py` & `dagster-census-0.20.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
-    install_requires=["dagster==1.4.3"],
+    install_requires=["dagster==1.4.4"],
     zip_safe=False,
 )
```

