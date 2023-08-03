# Comparing `tmp/dagster-msteams-0.20.3.tar.gz` & `tmp/dagster-msteams-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.20.3.tar", last modified: Mon Jul 31 23:07:05 2023, max compression
+gzip compressed data, was "dagster-msteams-0.20.4.tar", last modified: Thu Aug  3 21:59:28 2023, max compression
```

## Comparing `dagster-msteams-0.20.3.tar` & `dagster-msteams-0.20.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:05.829606 dagster-msteams-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-31 23:07:05.829606 dagster-msteams-0.20.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:05.829606 dagster-msteams-0.20.3/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3751 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:05.829606 dagster-msteams-0.20.3/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 23:07:05.000000 dagster-msteams-0.20.3/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-31 23:07:05.829606 dagster-msteams-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-31 22:58:19.000000 dagster-msteams-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:28.219139 dagster-msteams-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2023-08-03 21:59:28.219139 dagster-msteams-0.20.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:28.219139 dagster-msteams-0.20.4/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:28.219139 dagster-msteams-0.20.4/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-03 21:59:28.000000 dagster-msteams-0.20.4/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-08-03 21:59:28.219139 dagster-msteams-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-08-03 21:49:41.000000 dagster-msteams-0.20.4/setup.py
```

### Comparing `dagster-msteams-0.20.3/LICENSE` & `dagster-msteams-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/PKG-INFO` & `dagster-msteams-0.20.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.20.3
+Version: 0.20.4
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.20.3/dagster_msteams/card.py` & `dagster-msteams-0.20.4/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/dagster_msteams/client.py` & `dagster-msteams-0.20.4/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/dagster_msteams/hooks.py` & `dagster-msteams-0.20.4/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/dagster_msteams/resources.py` & `dagster-msteams-0.20.4/dagster_msteams/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/dagster_msteams/sensors.py` & `dagster-msteams-0.20.4/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.20.3/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.20.4/dagster_msteams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.20.3
+Version: 0.20.4
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-msteams-0.20.3/setup.py` & `dagster-msteams-0.20.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,12 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_msteams_tests*"]),
     install_requires=[
-        "dagster==1.4.3",
+        "dagster==1.4.4",
         "requests>=2,<3",
     ],
     zip_safe=False,
 )
```

