# Comparing `tmp/pytest-litter-0.0.1.tar.gz` & `tmp/pytest-litter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-litter-0.0.1.tar", last modified: Fri Aug  4 16:33:42 2023, max compression
+gzip compressed data, was "pytest-litter-0.0.2.tar", last modified: Fri Aug  4 17:22:17 2023, max compression
```

## Comparing `pytest-litter-0.0.1.tar` & `pytest-litter-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.376049 pytest-litter-0.0.1/.github/
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.380049 pytest-litter-0.0.1/.github/workflows/
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      664 2023-08-04 16:20:44.000000 pytest-litter-0.0.1/.github/workflows/ci.yaml
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      538 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/.github/workflows/publish.yaml
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     3077 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/.gitignore
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)    11357 2023-08-04 15:37:02.000000 pytest-litter-0.0.1/LICENSE
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)    13996 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/PKG-INFO
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      338 2023-08-04 15:54:09.000000 pytest-litter-0.0.1/README.md
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     3129 2023-08-04 16:12:35.000000 pytest-litter-0.0.1/pyproject.toml
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       16 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/requirements-lint.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       60 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/requirements-test.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       38 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/setup.cfg
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.376049 pytest-litter-0.0.1/src/
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.380049 pytest-litter-0.0.1/src/pytest_litter/
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       72 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/src/pytest_litter/__init__.py
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.380049 pytest-litter-0.0.1/src/pytest_litter/plugin/
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       26 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/src/pytest_litter/plugin/__init__.py
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     1265 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/src/pytest_litter/plugin/plugin.py
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     2084 2023-08-04 16:17:32.000000 pytest-litter-0.0.1/src/pytest_litter/plugin/utils.py
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     5024 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/src/pytest_litter/snapshots.py
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.380049 pytest-litter-0.0.1/src/pytest_litter.egg-info/
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)    13996 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/PKG-INFO
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      704 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/SOURCES.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)        1 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/dependency_links.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       55 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/entry_points.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       12 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/requires.txt
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)       14 2023-08-04 16:33:42.000000 pytest-litter-0.0.1/src/pytest_litter.egg-info/top_level.txt
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/tests/
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/tests/pytester/
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      156 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/tests/pytester/pytest.ini
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      646 2023-08-04 16:10:48.000000 pytest-litter-0.0.1/tests/pytester/pytester_tests.py
-drwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)        0 2023-08-04 16:33:42.384049 pytest-litter-0.0.1/tests/system_test/
--rwxrwxr-x   0 avikstroem  (1000) avikstroem  (1000)      596 2023-08-04 16:10:48.000000 pytest-litter-0.0.1/tests/system_test/system_test.sh
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     7435 2023-08-04 16:17:32.000000 pytest-litter-0.0.1/tests/test_plugin.py
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)     6526 2023-08-04 15:47:40.000000 pytest-litter-0.0.1/tests/test_snapshots.py
--rw-rw-r--   0 avikstroem  (1000) avikstroem  (1000)      359 2023-08-04 16:12:35.000000 pytest-litter-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/pytester/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/pytester/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/pytester/pytester_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/system_test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/system_test/system_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tox.ini
```

### Comparing `pytest-litter-0.0.1/.github/workflows/ci.yaml` & `pytest-litter-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/.github/workflows/publish.yaml` & `pytest-litter-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/.gitignore` & `pytest-litter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/LICENSE` & `pytest-litter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/PKG-INFO` & `pytest-litter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pytest-litter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pytest plugin which verifies that tests do not modify file trees.
+Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-litter-0.0.1/pyproject.toml` & `pytest-litter-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [project]
 name = "pytest-litter"
 description = "Pytest plugin which verifies that tests do not modify file trees."
+authors = [
+  {name="Anton Vikström"}
+]
 readme = "README.md"
 license = {file = "LICENSE"}
 urls = {repo = "https://github.com/mam-dev/pytest-litter"}
 requires-python = ">=3.9"
 dependencies = ["pytest >= 6.1"]
 dynamic = ["version"]
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-litter-0.0.1/src/pytest_litter/plugin/plugin.py` & `pytest-litter-0.0.2/src/pytest_litter/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/src/pytest_litter/plugin/utils.py` & `pytest-litter-0.0.2/src/pytest_litter/plugin/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/src/pytest_litter/snapshots.py` & `pytest-litter-0.0.2/src/pytest_litter/snapshots.py`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/src/pytest_litter.egg-info/PKG-INFO` & `pytest-litter-0.0.2/src/pytest_litter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pytest-litter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pytest plugin which verifies that tests do not modify file trees.
+Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-litter-0.0.1/src/pytest_litter.egg-info/SOURCES.txt` & `pytest-litter-0.0.2/src/pytest_litter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/tests/pytester/pytester_tests.py` & `pytest-litter-0.0.2/tests/pytester/pytester_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/tests/system_test/system_test.sh` & `pytest-litter-0.0.2/tests/system_test/system_test.sh`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/tests/test_plugin.py` & `pytest-litter-0.0.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.1/tests/test_snapshots.py` & `pytest-litter-0.0.2/tests/test_snapshots.py`

 * *Files identical despite different names*

