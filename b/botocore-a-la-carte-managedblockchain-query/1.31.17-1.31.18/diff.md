# Comparing `tmp/botocore-a-la-carte-managedblockchain-query-1.31.17.tar.gz` & `tmp/botocore-a-la-carte-managedblockchain-query-1.31.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-managedblockchain-query-1.31.17.tar", last modified: Wed Aug  2 01:13:10 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-managedblockchain-query-1.31.18.tar", last modified: Thu Aug  3 01:14:45 2023, max compression
```

## Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17.tar` & `botocore-a-la-carte-managedblockchain-query-1.31.18.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.658186 botocore-a-la-carte-managedblockchain-query-1.31.17/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 01:13:10.658186 botocore-a-la-carte-managedblockchain-query-1.31.17/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.654186 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.654186 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.654186 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.658186 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-08-02 01:12:30.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 01:12:30.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-08-02 01:12:30.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 01:12:30.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:13:10.658186 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:13:10.658186 botocore-a-la-carte-managedblockchain-query-1.31.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:13:10.000000 botocore-a-la-carte-managedblockchain-query-1.31.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-03 01:14:44.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-08-03 01:14:08.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 01:14:08.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-08-03 01:14:08.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 01:14:08.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 01:14:45.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-03 01:14:45.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:14:45.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 01:14:45.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:14:45.139012 botocore-a-la-carte-managedblockchain-query-1.31.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-03 01:14:44.000000 botocore-a-la-carte-managedblockchain-query-1.31.18/setup.py
```

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/LICENSE.txt` & `botocore-a-la-carte-managedblockchain-query-1.31.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/PKG-INFO` & `botocore-a-la-carte-managedblockchain-query-1.31.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-managedblockchain-query
-Version: 1.31.17
+Version: 1.31.18
 Summary: managedblockchain-query data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/endpoint-rule-set-1.json` & `botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/paginators-1.json` & `botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/botocore/data/managedblockchain-query/2023-05-04/service-2.json` & `botocore-a-la-carte-managedblockchain-query-1.31.18/botocore/data/managedblockchain-query/2023-05-04/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/PKG-INFO` & `botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-managedblockchain-query
-Version: 1.31.17
+Version: 1.31.18
 Summary: managedblockchain-query data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/botocore_a_la_carte_managedblockchain_query.egg-info/SOURCES.txt` & `botocore-a-la-carte-managedblockchain-query-1.31.18/botocore_a_la_carte_managedblockchain_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-managedblockchain-query-1.31.17/setup.py` & `botocore-a-la-carte-managedblockchain-query-1.31.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-managedblockchain-query',
-    version="1.31.17",
+    version="1.31.18",
     description='managedblockchain-query data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/managedblockchain-query/*/*.json'],
```

