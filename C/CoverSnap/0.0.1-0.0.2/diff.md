# Comparing `tmp/coversnap-0.0.1.tar.gz` & `tmp/coversnap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coversnap-0.0.1.tar", last modified: Fri Aug  4 02:02:49 2023, max compression
+gzip compressed data, was "coversnap-0.0.2.tar", last modified: Fri Aug  4 08:17:22 2023, max compression
```

## Comparing `coversnap-0.0.1.tar` & `coversnap-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-08-04 02:02:24.588730 coversnap-0.0.1/LICENSE
--rw-r--r--   0        0        0       12 2023-08-04 02:02:24.588730 coversnap-0.0.1/README.md
--rw-r--r--   0        0        0     1365 2023-08-04 02:02:49.888576 coversnap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-04 02:02:24.588730 coversnap-0.0.1/src/coversnap/__init__.py
--rw-r--r--   0        0        0      167 2023-08-04 02:02:24.588730 coversnap-0.0.1/src/coversnap/__main__.py
--rw-r--r--   0        0        0       31 2023-08-04 02:02:24.588730 coversnap-0.0.1/src/coversnap/hello.py
--rw-r--r--   0        0        0       80 2023-08-04 02:02:24.588730 coversnap-0.0.1/tests/test_hi.py
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 coversnap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-04 08:16:57.738610 coversnap-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1664 2023-08-04 08:16:57.738610 coversnap-0.0.2/README.md
+-rw-r--r--   0        0        0     1464 2023-08-04 08:17:22.766428 coversnap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/__init__.py
+-rw-r--r--   0        0        0     1155 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/__main__.py
+-rw-r--r--   0        0        0     1671 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/capture.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      638 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/test_captureimage.py
+-rw-r--r--   0        0        0      236 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/test_checkimage.py
+-rw-r--r--   0        0        0      973 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/util.py
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 coversnap-0.0.2/PKG-INFO
```

### Comparing `coversnap-0.0.1/LICENSE` & `coversnap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coversnap-0.0.1/pyproject.toml` & `coversnap-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CoverSnap"
-version = "0.0.1"
+version = "0.0.2"
 description = "a convenient Python library for capturing cover image from video"
 authors = [
     { name = "Tohrusky", email = "65994850+Tohrusky@users.noreply.github.com" },
 ]
 dependencies = [
     "opencv-python",
     "Pathlib",
@@ -40,25 +40,29 @@
 [tool.pdm.scripts.dev]
 composite = [
     "pdm install --dev",
 ]
 help = "Install the dev packages"
 
 [tool.pdm.scripts.test]
-cmd = "pytest --cov=src --cov-report=html"
+cmd = "pytest --cov=src --cov-config=.coveragerc --cov-report=xml --cov-report=html"
 help = "Run tests with coverage"
 
 [tool.pdm.scripts.lint]
 cmd = "pre-commit run --all-files"
 help = "Check code style against linters using pre-commit"
 
 [tool.pdm.scripts.pre_lint]
 composite = [
     "pre-commit install",
 ]
 help = "pre_lint hook: Installs pre-commit hooks"
 
+[tool.mypy]
+ignore_missing_imports = true
+strict = true
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

