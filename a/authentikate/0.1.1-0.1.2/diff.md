# Comparing `tmp/authentikate-0.1.1.tar.gz` & `tmp/authentikate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentikate-0.1.1.tar", max compression
+gzip compressed data, was "authentikate-0.1.2.tar", max compression
```

## Comparing `authentikate-0.1.1.tar` & `authentikate-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.1/README.md
--rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.1/authentikate/__init__.py
--rw-r--r--   0        0        0      157 2023-08-03 14:19:57.192109 authentikate-0.1.1/authentikate/admin.py
--rw-r--r--   0        0        0      156 2023-08-03 14:19:57.200110 authentikate-0.1.1/authentikate/apps.py
--rw-r--r--   0        0        0      474 2023-08-03 14:19:57.204110 authentikate-0.1.1/authentikate/decode.py
--rw-r--r--   0        0        0      409 2023-08-03 14:19:57.212109 authentikate-0.1.1/authentikate/errors.py
--rw-r--r--   0        0        0     2542 2023-08-03 14:19:57.216110 authentikate-0.1.1/authentikate/expand.py
--rw-r--r--   0        0        0     5875 2023-08-03 14:19:57.180109 authentikate-0.1.1/authentikate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-08-03 14:19:57.180109 authentikate-0.1.1/authentikate/migrations/__init__.py
--rw-r--r--   0        0        0      850 2023-08-03 14:19:57.228110 authentikate-0.1.1/authentikate/models.py
--rw-r--r--   0        0        0     1863 2023-08-03 14:19:57.236110 authentikate-0.1.1/authentikate/settings.py
--rw-r--r--   0        0        0        0 2023-08-03 15:19:29.893577 authentikate-0.1.1/authentikate/strawberry/__init__.py
--rw-r--r--   0        0        0      300 2023-08-03 15:19:17.041502 authentikate-0.1.1/authentikate/strawberry/filters.py
--rw-r--r--   0        0        0      241 2023-08-03 15:19:36.301615 authentikate-0.1.1/authentikate/strawberry/types.py
--rw-r--r--   0        0        0     1810 2023-08-03 14:19:57.244110 authentikate-0.1.1/authentikate/structs.py
--rw-r--r--   0        0        0     1884 2023-08-03 14:19:57.264110 authentikate-0.1.1/authentikate/utils.py
--rw-r--r--   0        0        0     1704 2023-08-03 15:20:53.218064 authentikate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 authentikate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.2/README.md
+-rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.2/authentikate/__init__.py
+-rw-r--r--   0        0        0      157 2023-08-03 14:19:57.192109 authentikate-0.1.2/authentikate/admin.py
+-rw-r--r--   0        0        0      156 2023-08-03 14:19:57.200110 authentikate-0.1.2/authentikate/apps.py
+-rw-r--r--   0        0        0      474 2023-08-03 14:19:57.204110 authentikate-0.1.2/authentikate/decode.py
+-rw-r--r--   0        0        0      409 2023-08-03 14:19:57.212109 authentikate-0.1.2/authentikate/errors.py
+-rw-r--r--   0        0        0     2542 2023-08-03 14:19:57.216110 authentikate-0.1.2/authentikate/expand.py
+-rw-r--r--   0        0        0     5875 2023-08-03 14:19:57.180109 authentikate-0.1.2/authentikate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:19:57.180109 authentikate-0.1.2/authentikate/migrations/__init__.py
+-rw-r--r--   0        0        0      850 2023-08-03 14:19:57.228110 authentikate-0.1.2/authentikate/models.py
+-rw-r--r--   0        0        0     1863 2023-08-03 14:19:57.236110 authentikate-0.1.2/authentikate/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:19:29.893577 authentikate-0.1.2/authentikate/strawberry/__init__.py
+-rw-r--r--   0        0        0      300 2023-08-03 15:19:17.041502 authentikate-0.1.2/authentikate/strawberry/filters.py
+-rw-r--r--   0        0        0      241 2023-08-03 15:19:36.301615 authentikate-0.1.2/authentikate/strawberry/types.py
+-rw-r--r--   0        0        0     1810 2023-08-03 14:19:57.244110 authentikate-0.1.2/authentikate/structs.py
+-rw-r--r--   0        0        0     1884 2023-08-03 14:19:57.264110 authentikate-0.1.2/authentikate/utils.py
+-rw-r--r--   0        0        0     1700 2023-08-04 12:46:37.320469 authentikate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 authentikate-0.1.2/PKG-INFO
```

### Comparing `authentikate-0.1.1/authentikate/expand.py` & `authentikate-0.1.2/authentikate/expand.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/authentikate/migrations/0001_initial.py` & `authentikate-0.1.2/authentikate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/authentikate/models.py` & `authentikate-0.1.2/authentikate/models.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/authentikate/settings.py` & `authentikate-0.1.2/authentikate/settings.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/authentikate/structs.py` & `authentikate-0.1.2/authentikate/structs.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/authentikate/utils.py` & `authentikate-0.1.2/authentikate/utils.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.1/pyproject.toml` & `authentikate-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "authentikate"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "authentikate" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyjwt = "^2.8.0"
-pydantic = "^2.1.1"
+pydantic = "<2"
 
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
 ignore_missing_imports = true
 strict = true
```

