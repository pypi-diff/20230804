# Comparing `tmp/chartsworth-0.2.0.tar.gz` & `tmp/chartsworth-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartsworth-0.2.0.tar", max compression
+gzip compressed data, was "chartsworth-0.3.0.tar", max compression
```

## Comparing `chartsworth-0.2.0.tar` & `chartsworth-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.2.0/README.md
--rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.2.0/chartsworth/__init__.py
--rw-r--r--   0        0        0     4181 2023-08-04 11:32:15.604618 chartsworth-0.2.0/chartsworth/client.py
--rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.2.0/chartsworth/plot.py
--rw-r--r--   0        0        0      574 2023-08-04 11:35:51.757810 chartsworth-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 chartsworth-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.3.0/README.md
+-rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.3.0/chartsworth/__init__.py
+-rw-r--r--   0        0        0     4181 2023-08-04 11:32:15.604618 chartsworth-0.3.0/chartsworth/client.py
+-rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.3.0/chartsworth/plot.py
+-rw-r--r--   0        0        0      572 2023-08-04 11:40:33.915865 chartsworth-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 chartsworth-0.3.0/PKG-INFO
```

### Comparing `chartsworth-0.2.0/chartsworth/client.py` & `chartsworth-0.3.0/chartsworth/client.py`

 * *Files identical despite different names*

### Comparing `chartsworth-0.2.0/chartsworth/plot.py` & `chartsworth-0.3.0/chartsworth/plot.py`

 * *Files identical despite different names*

### Comparing `chartsworth-0.2.0/pyproject.toml` & `chartsworth-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "chartsworth"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.12"
 slack-sdk = "^3.21.3"
 chatlab = {extras = ["noteable"], version = "1.0.0a13"}
-numpy = "^1.25.2"
-matplotlib = "^3.7.2"
+numpy = ">=1.23"
+matplotlib = ">=3.6"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core"]
```

