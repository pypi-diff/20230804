# Comparing `tmp/dagster-snowflake-pandas-0.20.3.tar.gz` & `tmp/dagster-snowflake-pandas-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.20.3.tar", last modified: Mon Jul 31 23:06:44 2023, max compression
+gzip compressed data, was "dagster-snowflake-pandas-0.20.4.tar", last modified: Thu Aug  3 22:00:32 2023, max compression
```

## Comparing `dagster-snowflake-pandas-0.20.3.tar` & `dagster-snowflake-pandas-0.20.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:44.713448 dagster-snowflake-pandas-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-31 23:06:44.713448 dagster-snowflake-pandas-0.20.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:44.713448 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    11760 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:44.713448 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      137 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-31 23:06:44.000000 dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-31 23:06:44.717448 dagster-snowflake-pandas-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-31 22:58:19.000000 dagster-snowflake-pandas-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:32.231617 dagster-snowflake-pandas-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-03 22:00:32.231617 dagster-snowflake-pandas-0.20.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:32.231617 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      413 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:00:32.231617 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      137 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-03 22:00:32.000000 dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-08-03 22:00:32.235617 dagster-snowflake-pandas-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-08-03 21:49:41.000000 dagster-snowflake-pandas-0.20.4/setup.py
```

### Comparing `dagster-snowflake-pandas-0.20.3/LICENSE` & `dagster-snowflake-pandas-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.20.3/PKG-INFO` & `dagster-snowflake-pandas-0.20.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas/snowflake_pandas_type_handler.py` & `dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas/snowflake_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.20.3/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-0.20.4/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.20.3/setup.py` & `dagster-snowflake-pandas-0.20.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
     install_requires=[
-        "dagster==1.4.3",
-        "dagster-snowflake==0.20.3",
+        "dagster==1.4.4",
+        "dagster-snowflake==0.20.4",
         "pandas",
         "requests",
         "snowflake-connector-python[pandas]",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
```

