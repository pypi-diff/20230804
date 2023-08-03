# Comparing `tmp/dagster-datahub-0.20.3.tar.gz` & `tmp/dagster-datahub-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.20.3.tar", last modified: Mon Jul 31 23:05:48 2023, max compression
+gzip compressed data, was "dagster-datahub-0.20.4.tar", last modified: Thu Aug  3 21:59:32 2023, max compression
```

## Comparing `dagster-datahub-0.20.3.tar` & `dagster-datahub-0.20.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:48.509031 dagster-datahub-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-31 23:05:48.509031 dagster-datahub-0.20.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:48.509031 dagster-datahub-0.20.3/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     4242 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:48.509031 dagster-datahub-0.20.3/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 23:05:48.000000 dagster-datahub-0.20.3/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-31 23:05:48.513031 dagster-datahub-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1424 2023-07-31 22:58:19.000000 dagster-datahub-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:32.159167 dagster-datahub-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-03 21:59:32.159167 dagster-datahub-0.20.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:32.155167 dagster-datahub-0.20.4/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:59:32.159167 dagster-datahub-0.20.4/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       84 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-03 21:59:32.000000 dagster-datahub-0.20.4/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-08-03 21:59:32.159167 dagster-datahub-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-08-03 21:49:41.000000 dagster-datahub-0.20.4/setup.py
```

### Comparing `dagster-datahub-0.20.3/LICENSE` & `dagster-datahub-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.20.3/PKG-INFO` & `dagster-datahub-0.20.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.20.3/dagster_datahub/resources.py` & `dagster-datahub-0.20.4/dagster_datahub/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.20.3/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.20.4/dagster_datahub.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-datahub-0.20.3/setup.py` & `dagster-datahub-0.20.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,14 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]<=0.10.2",
-        "dagster==1.4.3",
+        "dagster==1.4.4",
         "packaging",
         "requests",
     ],
     extras_require={},
     zip_safe=False,
 )
```

