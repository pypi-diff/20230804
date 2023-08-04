# Comparing `tmp/typer_common_functions-0.0.4.tar.gz` & `tmp/typer_common_functions-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_common_functions-0.0.4.tar", max compression
+gzip compressed data, was "typer_common_functions-0.0.5.tar", max compression
```

## Comparing `typer_common_functions-0.0.4.tar` & `typer_common_functions-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7633 2023-08-04 09:40:24.477624 typer_common_functions-0.0.4/LICENSE
--rw-r--r--   0        0        0     1940 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      119 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/readme.md
--rw-r--r--   0        0        0      174 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/__init__.py
--rw-r--r--   0        0        0     1216 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/logging.py
--rw-r--r--   0        0        0     7650 2023-08-04 09:40:24.481624 typer_common_functions-0.0.4/src/typer_common_functions/typer.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 typer_common_functions-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1918 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/readme.md
+-rw-r--r--   0        0        0      174 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/src/typer_common_functions/__init__.py
+-rw-r--r--   0        0        0     1216 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/src/typer_common_functions/logging.py
+-rw-r--r--   0        0        0     7650 2023-08-04 09:49:39.682824 typer_common_functions-0.0.5/src/typer_common_functions/typer.py
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 typer_common_functions-0.0.5/PKG-INFO
```

### Comparing `typer_common_functions-0.0.4/LICENSE` & `typer_common_functions-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.4/pyproject.toml` & `typer_common_functions-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-common-functions"
-version = "0.0.4"
+version = "0.0.5"
 description = "Commonly used Functions around the Typer CLI Library"
 authors = ["Joshua Kreuder <joshua_kreuder@outlook.com>"]
 keywords=["cli","typer"]
 readme="readme.md"
 license="LGPL-3"
 homepage="https://github.com/OpenJKSoftware/typer-common-functions"
 repository="https://github.com/OpenJKSoftware/typer-common-functions"
@@ -12,28 +12,28 @@
     "LICENSE",
 ]
 
 [tool.poetry_bumpversion.file."src/typer_common_functions/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
-typer = {extras = ["all"], version = "^0.7"}
+typer = {extras = ["all"], version = "^0"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pre-commit = "^2.20.0"
-isort = "^5.10.1"
-black = "^22.6.0"
+pytest = "^7.1"
+pre-commit = "^2.20"
+isort = "^5.10"
+black = "^22.6"
 mypy = "^0.961"
-bandit = "^1.7.4"
-pydocstyle = "^6.1.1"
-pylint = "^2.14.5"
-flake8 = "^4.0.1"
-flake8-docstrings = "^1.6.0"
-flake8-black = "^0.3.3"
+bandit = "^1.7"
+pydocstyle = "^6.1"
+pylint = "^2.14"
+flake8 = "^4.0"
+flake8-docstrings = "^1.6"
+flake8-black = "^0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

### Comparing `typer_common_functions-0.0.4/src/typer_common_functions/logging.py` & `typer_common_functions-0.0.5/src/typer_common_functions/logging.py`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.4/src/typer_common_functions/typer.py` & `typer_common_functions-0.0.5/src/typer_common_functions/typer.py`

 * *Files identical despite different names*

### Comparing `typer_common_functions-0.0.4/PKG-INFO` & `typer_common_functions-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: typer-common-functions
-Version: 0.0.4
+Version: 0.0.5
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
-Requires-Dist: typer[all] (>=0.7,<0.8)
+Requires-Dist: typer[all] (>=0,<1)
 Project-URL: Repository, https://github.com/OpenJKSoftware/typer-common-functions
 Description-Content-Type: text/markdown
 
 # Typer Common Functions
 
 Some Helpful Functions around the wonderful CLI Library [Typer](https://typer.tiangolo.com/)
```

