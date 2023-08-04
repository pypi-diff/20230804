# Comparing `tmp/chalk-harness-1.2.0.tar.gz` & `tmp/chalk-harness-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.2.0.tar", last modified: Thu Aug  3 21:54:23 2023, max compression
+gzip compressed data, was "chalk-harness-1.2.1.tar", last modified: Fri Aug  4 17:33:31 2023, max compression
```

## Comparing `chalk-harness-1.2.0.tar` & `chalk-harness-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 21:54:23.000000 chalk-harness-1.2.0/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 21:54:23.000000 chalk-harness-1.2.0/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:54:23.000000 chalk-harness-1.2.0/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 21:54:23.000000 chalk-harness-1.2.0/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 21:54:23.000000 chalk-harness-1.2.0/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:23.244463 chalk-harness-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:54:07.000000 chalk-harness-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:31.288736 chalk-harness-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 17:33:31.288736 chalk-harness-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:31.284736 chalk-harness-1.2.1/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 17:33:31.000000 chalk-harness-1.2.1/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-04 17:33:31.000000 chalk-harness-1.2.1/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:33:31.000000 chalk-harness-1.2.1/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:33:31.000000 chalk-harness-1.2.1/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 17:33:31.000000 chalk-harness-1.2.1/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:31.284736 chalk-harness-1.2.1/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:33:31.288736 chalk-harness-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:31.288736 chalk-harness-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:33:19.000000 chalk-harness-1.2.1/tests/__init__.py
```

### Comparing `chalk-harness-1.2.0/PKG-INFO` & `chalk-harness-1.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.2.0/README.md` & `chalk-harness-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.0/chalk_harness.egg-info/PKG-INFO` & `chalk-harness-1.2.1/chalk_harness.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.2.0/chalkharness/__init__.py` & `chalk-harness-1.2.1/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.0/setup.py` & `chalk-harness-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.0/tests/SanityTestCase.py` & `chalk-harness-1.2.1/tests/SanityTestCase.py`

 * *Files identical despite different names*

