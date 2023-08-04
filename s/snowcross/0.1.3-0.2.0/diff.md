# Comparing `tmp/snowcross-0.1.3.tar.gz` & `tmp/snowcross-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowcross-0.1.3.tar", last modified: Wed Aug  2 04:15:47 2023, max compression
+gzip compressed data, was "snowcross-0.2.0.tar", last modified: Fri Aug  4 02:59:22 2023, max compression
```

## Comparing `snowcross-0.1.3.tar` & `snowcross-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 04:15:21.000000 snowcross-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 04:15:21.000000 snowcross-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-02 04:15:47.394590 snowcross-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 04:15:21.000000 snowcross-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-02 04:15:21.000000 snowcross-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 04:15:21.000000 snowcross-0.1.3/requirements-locator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 04:15:21.000000 snowcross-0.1.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 04:15:21.000000 snowcross-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:15:47.394590 snowcross-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 04:15:21.000000 snowcross-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/snowcross/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:21.000000 snowcross-0.1.3/snowcross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-02 04:15:21.000000 snowcross-0.1.3/snowcross/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 04:15:21.000000 snowcross-0.1.3/snowcross/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-02 04:15:21.000000 snowcross-0.1.3/snowcross/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-08-02 04:15:21.000000 snowcross-0.1.3/snowcross/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/snowcross.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-02 04:15:47.000000 snowcross-0.1.3/snowcross.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-02 04:15:47.000000 snowcross-0.1.3/snowcross.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:15:47.000000 snowcross-0.1.3/snowcross.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 04:15:47.000000 snowcross-0.1.3/snowcross.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 04:15:47.000000 snowcross-0.1.3/snowcross.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:21.000000 snowcross-0.1.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-02 04:15:21.000000 snowcross-0.1.3/tests/fixtures/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-02 04:15:21.000000 snowcross-0.1.3/tests/fixtures/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:47.394590 snowcross-0.1.3/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:15:21.000000 snowcross-0.1.3/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 04:15:21.000000 snowcross-0.1.3/tests/helpers/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 02:58:54.000000 snowcross-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 02:58:54.000000 snowcross-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-04 02:59:22.218912 snowcross-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-04 02:58:54.000000 snowcross-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-04 02:58:54.000000 snowcross-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 02:58:54.000000 snowcross-0.2.0/requirements-locator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-04 02:58:54.000000 snowcross-0.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 02:58:54.000000 snowcross-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:59:22.218912 snowcross-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 02:58:54.000000 snowcross-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/snowcross/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:54.000000 snowcross-0.2.0/snowcross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-04 02:58:54.000000 snowcross-0.2.0/snowcross/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-04 02:58:54.000000 snowcross-0.2.0/snowcross/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-04 02:58:54.000000 snowcross-0.2.0/snowcross/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-08-04 02:58:54.000000 snowcross-0.2.0/snowcross/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/snowcross.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-04 02:59:22.000000 snowcross-0.2.0/snowcross.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-04 02:59:22.000000 snowcross-0.2.0/snowcross.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:59:22.000000 snowcross-0.2.0/snowcross.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-04 02:59:22.000000 snowcross-0.2.0/snowcross.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 02:59:22.000000 snowcross-0.2.0/snowcross.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:54.000000 snowcross-0.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-04 02:58:54.000000 snowcross-0.2.0/tests/fixtures/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-04 02:58:54.000000 snowcross-0.2.0/tests/fixtures/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:59:22.218912 snowcross-0.2.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:54.000000 snowcross-0.2.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-04 02:58:54.000000 snowcross-0.2.0/tests/helpers/docker.py
```

### Comparing `snowcross-0.1.3/LICENSE` & `snowcross-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/PKG-INFO` & `snowcross-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.1.3
+Version: 0.2.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: locator
 Provides-Extra: test
 License-File: LICENSE
 
 Adaptors for tools and services in a Snowflake-centric data platform.
 
 ## Requirements
 
-Requires Python 3.8 or above.
+Requires Python 3.10 or above.
```

### Comparing `snowcross-0.1.3/README.md` & `snowcross-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 > [PyPI](https://pypi.org/project/snowcross/)! All commits, pull requests and this readme are
 > hidden, however the source code is easily extracted from published artifacts. Refrain from
 > including any references to proprietary code, infrastructure or architecture. This package is
 > for generic utilities for tools and services only.
 
 ## Requirements
 
-Requires Python 3.8 or above.
+Requires Python 3.10 or above.
 
 ## Usage
 
 You can install from [PyPI](https://pypi.org/project/snowcross/):
 
 ```shell
 pip install snowcross
```

### Comparing `snowcross-0.1.3/setup.py` & `snowcross-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 from setuptools import setup, find_packages
 
-if sys.version_info < (3, 6):
-    raise ValueError("Requires Python 3.6+")
+if sys.version_info < (3, 10):
+    raise ValueError("Requires Python 3.10+")
 
 
 def requires_from_file(filename: str) -> list:
     with open(filename, "r", encoding="utf-8") as f:
         return [x.strip() for x in f if x.strip()]
 
 
@@ -29,12 +29,10 @@
     extras_require={
         "locator": requires_from_file("requirements-locator.txt"),
         "test": requires_from_file("requirements-test.txt"),
     },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `snowcross-0.1.3/snowcross/aws.py` & `snowcross-0.2.0/snowcross/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/snowcross/errors.py` & `snowcross-0.2.0/snowcross/errors.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/snowcross/locator.py` & `snowcross-0.2.0/snowcross/locator.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/snowcross/snowflake.py` & `snowcross-0.2.0/snowcross/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/snowcross.egg-info/PKG-INFO` & `snowcross-0.2.0/snowcross.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.1.3
+Version: 0.2.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: locator
 Provides-Extra: test
 License-File: LICENSE
 
 Adaptors for tools and services in a Snowflake-centric data platform.
 
 ## Requirements
 
-Requires Python 3.8 or above.
+Requires Python 3.10 or above.
```

### Comparing `snowcross-0.1.3/tests/fixtures/aws.py` & `snowcross-0.2.0/tests/fixtures/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/tests/fixtures/snowflake.py` & `snowcross-0.2.0/tests/fixtures/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.1.3/tests/helpers/docker.py` & `snowcross-0.2.0/tests/helpers/docker.py`

 * *Files identical despite different names*

