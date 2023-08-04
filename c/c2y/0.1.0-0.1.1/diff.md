# Comparing `tmp/c2y-0.1.0.tar.gz` & `tmp/c2y-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2y-0.1.0.tar", max compression
+gzip compressed data, was "c2y-0.1.1.tar", max compression
```

## Comparing `c2y-0.1.0.tar` & `c2y-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853000 c2y-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-08-04 14:50:01.077143 c2y-0.1.0/README.md
--rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223000 c2y-0.1.0/c2y/__init__.py
--rw-r--r--   0        0        0      103 2023-07-31 07:46:09.233000 c2y-0.1.0/c2y/__main__.py
--rw-r--r--   0        0        0     9377 2023-07-31 12:10:58.309000 c2y-0.1.0/c2y/utils.py
--rw-r--r--   0        0        0      669 2023-08-04 14:40:29.900991 c2y-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 c2y-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-31 07:46:08.853000 c2y-0.1.1/LICENSE
+-rw-r--r--   0        0        0      519 2023-08-04 15:13:42.677467 c2y-0.1.1/README.md
+-rw-r--r--   0        0        0       45 2023-07-31 07:46:09.223000 c2y-0.1.1/c2y/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-31 07:46:09.233000 c2y-0.1.1/c2y/__main__.py
+-rw-r--r--   0        0        0     9377 2023-07-31 12:10:58.309000 c2y-0.1.1/c2y/utils.py
+-rw-r--r--   0        0        0      707 2023-08-04 15:09:08.015926 c2y-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 c2y-0.1.1/PKG-INFO
```

### Comparing `c2y-0.1.0/LICENSE` & `c2y-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c2y-0.1.0/c2y/utils.py` & `c2y-0.1.1/c2y/utils.py`

 * *Files identical despite different names*

### Comparing `c2y-0.1.0/pyproject.toml` & `c2y-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "c2y"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Convert coco datasets to yolo datasets"
 authors = ["hobbymarks <ihobbymarks@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.11,<3.13"
+python = ">=3.10,<3.13"
 yapf = "^0.40.1"
 isort = "^5.12.0"
 jupyterlab = "^4.0.3"
 jupyterlab-code-formatter = "^2.2.1"
 jupyterlab-execute-time = "^3.0.0"
 pyinstaller = "^5.13.0"
 pycocotools = "^2.0.6"
```

