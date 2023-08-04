# Comparing `tmp/pykebab-0.8.3.tar.gz` & `tmp/pykebab-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.8.3.tar", max compression
+gzip compressed data, was "pykebab-0.9.0.tar", max compression
```

## Comparing `pykebab-0.8.3.tar` & `pykebab-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/cli/cli.py
--rw-r--r--   0        0        0      902 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/exceptions.py
--rw-r--r--   0        0        0     2586 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/k8s.py
--rw-r--r--   0        0        0      744 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/loaders.py
--rw-r--r--   0        0        0     2368 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/magic.py
--rw-r--r--   0        0        0     1575 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/openers.py
--rw-r--r--   0        0        0    22900 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/utils.py
--rw-r--r--   0        0        0     1086 2023-07-31 12:40:52.844894 pykebab-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 pykebab-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/cli/cli.py
+-rw-r--r--   0        0        0      902 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/exceptions.py
+-rw-r--r--   0        0        0     2586 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/k8s.py
+-rw-r--r--   0        0        0      744 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/loaders.py
+-rw-r--r--   0        0        0     2368 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/magic.py
+-rw-r--r--   0        0        0     1575 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/openers.py
+-rw-r--r--   0        0        0    22900 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/utils.py
+-rw-r--r--   0        0        0      957 2023-08-04 03:09:43.628775 pykebab-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 pykebab-0.9.0/PKG-INFO
```

### Comparing `pykebab-0.8.3/kebab/__init__.py` & `pykebab-0.9.0/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/aws.py` & `pykebab-0.9.0/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/cli/cli.py` & `pykebab-0.9.0/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/constants.py` & `pykebab-0.9.0/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/k8s.py` & `pykebab-0.9.0/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/loaders.py` & `pykebab-0.9.0/kebab/loaders.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/magic.py` & `pykebab-0.9.0/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/openers.py` & `pykebab-0.9.0/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/sources.py` & `pykebab-0.9.0/kebab/sources.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/kebab/utils.py` & `pykebab-0.9.0/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.3/pyproject.toml` & `pykebab-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.8.3"
+version = "0.9.0"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 deprecation = "^2.1.0"
 pydantic = "^2.0.3"
 # cli
 click = { version = "^8.1.5", optional = true }
 # aws
-boto3 = { version = "^1.28.3", optional = true }
+boto3 = { version = "^1.28.19", optional = true }
 # k8s
-kubernetes = { version = "^26.1.0", optional = true }
-configparser = "^5.3.0"
+kubernetes = { version = "^27.2.0", optional = true }
+configparser = "^6.0.0"
 pyyaml = "^6.0.1"
 setuptools = "^68.0.0"
-pyxdg = "^0.28"
-jupyter = "^1.0.0"
 
 [tool.poetry.extras]
 cli = ["click"]
 k8s = ["kubernetes"]
 aws = ["boto3"]
 
 [tool.poetry.dev-dependencies]
-pytest = { version = "*" }
-pytest-cov = { version = "*" }
-pytest-black = { version = "*" }
-mock = { version = "*" }
-black = { version = "*" }
-flake8 = { version = "*" }
-flake8-black = { version = "*"}
+pytest = "*"
+pytest-cov = "*"
+pytest-black = "*"
+mock = "*"
+black = "*"
+flake8 = "*"
+flake8-black = "*"
 
 [tool.poetry.scripts]
 kebab = 'kebab.cli:run'
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
```

### Comparing `pykebab-0.8.3/PKG-INFO` & `pykebab-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.8.3
+Version: 0.9.0
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws
 Provides-Extra: cli
 Provides-Extra: k8s
-Requires-Dist: boto3 (>=1.28.3,<2.0.0) ; extra == "aws"
+Requires-Dist: boto3 (>=1.28.19,<2.0.0) ; extra == "aws"
 Requires-Dist: click (>=8.1.5,<9.0.0) ; extra == "cli"
-Requires-Dist: configparser (>=5.3.0,<6.0.0)
+Requires-Dist: configparser (>=6.0.0,<7.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "k8s"
+Requires-Dist: kubernetes (>=27.2.0,<28.0.0) ; extra == "k8s"
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: setuptools (>=68.0.0,<69.0.0)
```

