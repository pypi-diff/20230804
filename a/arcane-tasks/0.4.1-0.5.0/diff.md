# Comparing `tmp/arcane-tasks-0.4.1.tar.gz` & `tmp/arcane_tasks-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-tasks-0.4.1.tar", max compression
+gzip compressed data, was "arcane_tasks-0.5.0.tar", max compression
```

## Comparing `arcane-tasks-0.4.1.tar` & `arcane_tasks-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      530 2022-07-21 15:05:16.366176 arcane-tasks-0.4.1/README.md
--rw-r--r--   0        0        0     2930 2022-07-21 15:05:16.366176 arcane-tasks-0.4.1/arcane/tasks.py
--rw-r--r--   0        0        0      424 2022-07-21 15:05:16.366176 arcane-tasks-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1213 2022-07-21 15:05:30.581317 arcane-tasks-0.4.1/setup.py
--rw-r--r--   0        0        0     1156 2022-07-21 15:05:30.581581 arcane-tasks-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      530 2023-08-04 09:24:47.822558 arcane_tasks-0.5.0/README.md
+-rw-r--r--   0        0        0     3257 2023-08-04 09:24:47.822558 arcane_tasks-0.5.0/arcane/tasks.py
+-rw-r--r--   0        0        0      425 2023-08-04 09:24:47.822558 arcane_tasks-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 arcane_tasks-0.5.0/PKG-INFO
```

### Comparing `arcane-tasks-0.4.1/README.md` & `arcane_tasks-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `arcane-tasks-0.4.1/PKG-INFO` & `arcane_tasks-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: arcane-tasks
-Version: 0.4.1
+Version: 0.5.0
 Summary: Override tasks client
 Author: Arcane
 Author-email: product@arcane.run
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arcane-core (>=1.6.0,<2.0.0)
 Requires-Dist: backoff (==1.10.0)
-Requires-Dist: google-cloud-tasks (==2.8.1)
+Requires-Dist: google-cloud-tasks (==2.14.0)
 Description-Content-Type: text/markdown
 
 # Arcane CloudTask
 
 This package is base on [google-cloud-cloudtasks](https://pypi.org/project/google-cloud-tasks/).
 
 ## Get Started
```

