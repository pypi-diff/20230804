# Comparing `tmp/wbutils-0.0.2.tar.gz` & `tmp/wbutils-0.0.4.tar.gz`

## Comparing `wbutils-0.0.2.tar` & `wbutils-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/__init__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/artifact.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/directory.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/framework.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/include.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/io.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/keys.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/parsing/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wbutils-0.0.2/src/wbutils/parsing/pytorch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_directory.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_framework.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wbutils-0.0.2/tests/test_io.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 wbutils-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 wbutils-0.0.2/LICENSE
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wbutils-0.0.2/README.md
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 wbutils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 wbutils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/__init__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/artifact.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/directory.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/framework.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/include.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/io.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/keys.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/parsing/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wbutils-0.0.4/src/wbutils/parsing/pytorch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbutils-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 wbutils-0.0.4/tests/test_create_artifact.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wbutils-0.0.4/tests/test_directory.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wbutils-0.0.4/tests/test_framework.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wbutils-0.0.4/tests/test_io.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 wbutils-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 wbutils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wbutils-0.0.4/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 wbutils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 wbutils-0.0.4/PKG-INFO
```

### Comparing `wbutils-0.0.2/src/wbutils/__init__.py` & `wbutils-0.0.4/src/wbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/artifact.py` & `wbutils-0.0.4/src/wbutils/artifact.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/directory.py` & `wbutils-0.0.4/src/wbutils/directory.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/include.py` & `wbutils-0.0.4/src/wbutils/include.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/io.py` & `wbutils-0.0.4/src/wbutils/io.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/keys.py` & `wbutils-0.0.4/src/wbutils/keys.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/src/wbutils/parsing/pytorch.py` & `wbutils-0.0.4/src/wbutils/parsing/pytorch.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/tests/test_directory.py` & `wbutils-0.0.4/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/LICENSE` & `wbutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wbutils-0.0.2/pyproject.toml` & `wbutils-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Repository = "https://github.com/ankur-gupta/wbutils.git"
 
 [tool.hatch.version]
 path = "src/wbutils/version.py"
 
 [tool.hatch.envs.test]
 dependencies = [
+    "hatch",
     "coverage",
     "codecov",
     "pytest",
     "pytest-cov",
     "pytest-mock",
 ]
```

### Comparing `wbutils-0.0.2/PKG-INFO` & `wbutils-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbutils
-Version: 0.0.2
+Version: 0.0.4
 Summary: Helpful utilities to use Weights & Biases
 Project-URL: Homepage, https://github.com/ankur-gupta/wbutils
 Project-URL: Repository, https://github.com/ankur-gupta/wbutils.git
 Author-email: Ankur Gupta <7110058+ankur-gupta@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Ankur Gupta
```

