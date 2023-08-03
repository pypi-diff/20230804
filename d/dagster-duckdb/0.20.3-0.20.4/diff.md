# Comparing `tmp/dagster-duckdb-0.20.3.tar.gz` & `tmp/dagster-duckdb-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.20.3.tar", last modified: Mon Jul 31 23:05:52 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.20.4.tar", last modified: Thu Aug  3 22:00:11 2023, max compression
```

## Comparing `dagster-duckdb-0.20.3.tar` & `dagster-duckdb-0.20.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:52.377059 dagster-duckdb-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-31 23:05:52.377059 dagster-duckdb-0.20.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:52.377059 dagster-duckdb-0.20.3/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:05:52.377059 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 23:05:52.000000 dagster-duckdb-0.20.3/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-31 23:05:52.377059 dagster-duckdb-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1495 2023-07-31 22:58:19.000000 dagster-duckdb-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:11.451463 dagster-duckdb-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      642 2023-08-03 22:00:11.451463 dagster-duckdb-0.20.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:11.451463 dagster-duckdb-0.20.4/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:11.451463 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-03 22:00:11.000000 dagster-duckdb-0.20.4/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-08-03 22:00:11.455463 dagster-duckdb-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-08-03 21:49:41.000000 dagster-duckdb-0.20.4/setup.py
```

### Comparing `dagster-duckdb-0.20.3/LICENSE` & `dagster-duckdb-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.3/PKG-INFO` & `dagster-duckdb-0.20.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.20.3/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.20.4/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.3/dagster_duckdb/resource.py` & `dagster-duckdb-0.20.4/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.20.3/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.20.4/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-0.20.3/setup.py` & `dagster-duckdb-0.20.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.4.3",
+        "dagster==1.4.4",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

