# Comparing `tmp/bosminer-0.1.0.tar.gz` & `tmp/bosminer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosminer-0.1.0.tar", max compression
+gzip compressed data, was "bosminer-0.2.0.tar", max compression
```

## Comparing `bosminer-0.1.0.tar` & `bosminer-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1685 2023-05-30 14:44:30.842865 bosminer-0.1.0/README.md
--rw-r--r--   0        0        0     1578 2023-05-30 14:44:53.210713 bosminer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 14:44:30.868865 bosminer-0.1.0/src/bosminer/__init__.py
--rw-r--r--   0        0        0     2653 2023-05-30 14:44:30.843865 bosminer-0.1.0/src/bosminer/client.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 bosminer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3239 2023-08-04 21:18:01.355810 bosminer-0.2.0/README.md
+-rw-r--r--   0        0        0     1722 2023-08-04 21:18:21.720620 bosminer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-04 21:18:01.381809 bosminer-0.2.0/src/bosminer/__init__.py
+-rw-r--r--   0        0        0     2653 2023-08-04 21:18:01.356810 bosminer-0.2.0/src/bosminer/client.py
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 bosminer-0.2.0/PKG-INFO
```

### Comparing `bosminer-0.1.0/pyproject.toml` & `bosminer-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 [tool.poetry]
 name = "bosminer"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["teosibileau <teo.sibileau@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry.dependencies]
 python = "^3.9, <4.0"
+grpc-requests = "^0.1.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 ipython = "^8.13.2"
 pre-commit = "^3.3.1"
 coverage = "^7.2.5"
 pytest-cov = "^4.0.0"
 twine = "^4.0.2"
 build = "^0.10.0"
+jupyterlab = "^4.0.2"
+grpcio-tools = "^1.56.2"
+pytest-grpc = "^0.8.0"
+grpcio-reflection = "^1.56.2"
+ipdb = "^0.13.13"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "./src"
```

### Comparing `bosminer-0.1.0/src/bosminer/client.py` & `bosminer-0.2.0/src/bosminer/client.py`

 * *Files identical despite different names*

