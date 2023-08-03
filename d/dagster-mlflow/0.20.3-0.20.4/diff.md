# Comparing `tmp/dagster-mlflow-0.20.3.tar.gz` & `tmp/dagster-mlflow-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.20.3.tar", last modified: Mon Jul 31 23:08:34 2023, max compression
+gzip compressed data, was "dagster-mlflow-0.20.4.tar", last modified: Thu Aug  3 22:01:49 2023, max compression
```

## Comparing `dagster-mlflow-0.20.3.tar` & `dagster-mlflow-0.20.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:34.098257 dagster-mlflow-0.20.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-31 23:08:34.098257 dagster-mlflow-0.20.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:34.098257 dagster-mlflow-0.20.3/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10915 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:34.098257 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-31 23:08:33.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-31 23:08:34.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:08:33.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:08:33.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-31 23:08:33.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 23:08:33.000000 dagster-mlflow-0.20.3/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-31 23:08:34.098257 dagster-mlflow-0.20.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1183 2023-07-31 22:58:19.000000 dagster-mlflow-0.20.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:49.200191 dagster-mlflow-0.20.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      571 2023-08-03 22:01:49.200191 dagster-mlflow-0.20.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:49.200191 dagster-mlflow-0.20.4/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10915 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:01:49.200191 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-03 22:01:49.000000 dagster-mlflow-0.20.4/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-08-03 22:01:49.200191 dagster-mlflow-0.20.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-08-03 21:49:41.000000 dagster-mlflow-0.20.4/setup.py
```

### Comparing `dagster-mlflow-0.20.3/LICENSE` & `dagster-mlflow-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.3/PKG-INFO` & `dagster-mlflow-0.20.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.20.3/dagster_mlflow/hooks.py` & `dagster-mlflow-0.20.4/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.3/dagster_mlflow/resources.py` & `dagster-mlflow-0.20.4/dagster_mlflow/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.20.3/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.20.4/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.20.3
+Version: 0.20.4
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.20.3/setup.py` & `dagster-mlflow-0.20.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
-    install_requires=["dagster==1.4.3", "mlflow", "pandas"],
+    install_requires=["dagster==1.4.4", "mlflow", "pandas"],
     zip_safe=False,
 )
```

