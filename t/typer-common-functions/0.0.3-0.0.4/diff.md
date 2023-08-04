# Comparing `tmp/typer_common_functions-0.0.3.tar.gz` & `tmp/typer_common_functions-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_common_functions-0.0.3.tar", max compression
+gzip compressed data, was "typer_common_functions-0.0.4.tar", max compression
```

## Comparing `typer_common_functions-0.0.3.tar` & `typer_common_functions-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     7633 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/LICENSE
--rw-r--r--   0        0        0     1942 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/readme.md
--rw-r--r--   0        0        0      174 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/src/typer_common_functions/__init__.py
--rw-r--r--   0        0        0     1216 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/src/typer_common_functions/logging.py
--rw-r--r--   0        0        0     7650 2023-02-02 08:09:18.058112 typer_common_functions-0.0.3/src/typer_common_functions/typer.py
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 typer_common_functions-0.0.3/setup.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 typer_common_functions-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-08-04 09:40:24.477624 typer_common_functions-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1940 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/readme.md
+-rw-r--r--   0        0        0      174 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/__init__.py
+-rw-r--r--   0        0        0     1216 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/logging.py
+-rw-r--r--   0        0        0     7650 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/typer.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 typer_common_functions-0.0.4/PKG-INFO
```

### Comparing `typer_common_functions-0.0.3/LICENSE` & `typer_common_functions-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.3/pyproject.toml` & `typer_common_functions-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-common-functions"
-version = "0.0.3"
+version = "0.0.4"
 description = "Commonly used Functions around the Typer CLI Library"
 authors = ["Joshua Kreuder <joshua_kreuder@outlook.com>"]
 keywords=["cli","typer"]
 readme="readme.md"
 license="LGPL-3"
 homepage="https://github.com/OpenJKSoftware/typer-common-functions"
 repository="https://github.com/OpenJKSoftware/typer-common-functions"
@@ -12,15 +12,15 @@
     "LICENSE",
 ]
 
 [tool.poetry_bumpversion.file."src/typer_common_functions/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = {extras = ["all"], version = "^0.7"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pre-commit = "^2.20.0"
 isort = "^5.10.1"
 black = "^22.6.0"
 mypy = "^0.961"
```

### Comparing `typer_common_functions-0.0.3/src/typer_common_functions/logging.py` & `typer_common_functions-0.0.4/src/typer_common_functions/logging.py`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.3/src/typer_common_functions/typer.py` & `typer_common_functions-0.0.4/src/typer_common_functions/typer.py`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.3/PKG-INFO` & `typer_common_functions-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: typer-common-functions
-Version: 0.0.3
+Version: 0.0.4
 Summary: Commonly used Functions around the Typer CLI Library
 Home-page: https://github.com/OpenJKSoftware/typer-common-functions
 License: LGPL-3
 Keywords: cli,typer
 Author: Joshua Kreuder
 Author-email: joshua_kreuder@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.7,<0.8)
 Project-URL: Repository, https://github.com/OpenJKSoftware/typer-common-functions
 Description-Content-Type: text/markdown
 
 # Typer Common Functions
 
 Some Helpful Functions around the wonderful CLI Library [Typer](https://typer.tiangolo.com/)
```

