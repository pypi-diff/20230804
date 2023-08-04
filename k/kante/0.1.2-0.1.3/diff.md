# Comparing `tmp/kante-0.1.2.tar.gz` & `tmp/kante-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kante-0.1.2.tar", max compression
+gzip compressed data, was "kante-0.1.3.tar", max compression
```

## Comparing `kante-0.1.2.tar` & `kante-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       22 2023-08-03 15:22:07.514496 kante-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-08-03 15:22:26.526607 kante-0.1.2/kante/__init__.py
--rw-r--r--   0        0        0        1 2023-08-03 15:22:26.530607 kante-0.1.2/kante/admin.py
--rw-r--r--   0        0        0      142 2023-08-03 15:22:26.542607 kante-0.1.2/kante/apps.py
--rw-r--r--   0        0        0     1550 2023-08-03 18:00:19.988599 kante-0.1.2/kante/channel.py
--rw-r--r--   0        0        0      120 2023-08-03 15:22:26.502607 kante-0.1.2/kante/consumers/__init__.py
--rw-r--r--   0        0        0      256 2023-08-03 15:22:26.502607 kante-0.1.2/kante/consumers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1450 2023-08-03 15:22:26.502607 kante-0.1.2/kante/consumers/__pycache__/http.cpython-310.pyc
--rw-r--r--   0        0        0     1215 2023-08-03 15:22:26.502607 kante-0.1.2/kante/consumers/__pycache__/ws.cpython-310.pyc
--rw-r--r--   0        0        0     1727 2023-08-03 18:01:45.041024 kante-0.1.2/kante/consumers/http.py
--rw-r--r--   0        0        0     1157 2023-08-03 18:00:46.804733 kante-0.1.2/kante/consumers/ws.py
--rw-r--r--   0        0        0     1491 2023-08-03 15:24:58.683491 kante-0.1.2/kante/context.py
--rw-r--r--   0        0        0     2363 2023-08-03 15:22:26.562607 kante-0.1.2/kante/cors.py
--rw-r--r--   0        0        0      637 2023-08-03 15:22:26.570607 kante-0.1.2/kante/directives.py
--rw-r--r--   0        0        0        0 2023-08-03 15:22:26.514607 kante-0.1.2/kante/migrations/__init__.py
--rw-r--r--   0        0        0      140 2023-08-03 15:22:26.514607 kante-0.1.2/kante/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      148 2023-08-03 15:22:26.614608 kante-0.1.2/kante/types.py
--rw-r--r--   0        0        0     1742 2023-08-03 18:02:02.217110 kante-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 kante-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-08-03 15:22:07.514496 kante-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 15:22:26.526607 kante-0.1.3/kante/__init__.py
+-rw-r--r--   0        0        0        1 2023-08-03 15:22:26.530607 kante-0.1.3/kante/admin.py
+-rw-r--r--   0        0        0      142 2023-08-03 15:22:26.542607 kante-0.1.3/kante/apps.py
+-rw-r--r--   0        0        0     1550 2023-08-03 18:00:19.988599 kante-0.1.3/kante/channel.py
+-rw-r--r--   0        0        0      120 2023-08-03 15:22:26.502607 kante-0.1.3/kante/consumers/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-03 15:22:26.502607 kante-0.1.3/kante/consumers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1450 2023-08-03 15:22:26.502607 kante-0.1.3/kante/consumers/__pycache__/http.cpython-310.pyc
+-rw-r--r--   0        0        0     1215 2023-08-03 15:22:26.502607 kante-0.1.3/kante/consumers/__pycache__/ws.cpython-310.pyc
+-rw-r--r--   0        0        0     1727 2023-08-03 18:01:45.041024 kante-0.1.3/kante/consumers/http.py
+-rw-r--r--   0        0        0     1157 2023-08-03 18:00:46.804733 kante-0.1.3/kante/consumers/ws.py
+-rw-r--r--   0        0        0     1491 2023-08-03 15:24:58.683491 kante-0.1.3/kante/context.py
+-rw-r--r--   0        0        0     2363 2023-08-03 15:22:26.562607 kante-0.1.3/kante/cors.py
+-rw-r--r--   0        0        0      637 2023-08-03 15:22:26.570607 kante-0.1.3/kante/directives.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:22:26.514607 kante-0.1.3/kante/migrations/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-03 15:22:26.514607 kante-0.1.3/kante/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      148 2023-08-03 15:22:26.614608 kante-0.1.3/kante/types.py
+-rw-r--r--   0        0        0     1722 2023-08-04 12:48:01.732877 kante-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 kante-0.1.3/PKG-INFO
```

### Comparing `kante-0.1.2/kante/channel.py` & `kante-0.1.3/kante/channel.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/consumers/__pycache__/http.cpython-310.pyc` & `kante-0.1.3/kante/consumers/__pycache__/http.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/consumers/__pycache__/ws.cpython-310.pyc` & `kante-0.1.3/kante/consumers/__pycache__/ws.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/consumers/http.py` & `kante-0.1.3/kante/consumers/http.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/consumers/ws.py` & `kante-0.1.3/kante/consumers/ws.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/context.py` & `kante-0.1.3/kante/context.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/cors.py` & `kante-0.1.3/kante/cors.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/kante/directives.py` & `kante-0.1.3/kante/directives.py`

 * *Files identical despite different names*

### Comparing `kante-0.1.2/pyproject.toml` & `kante-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "kante"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "kante" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "^2.1.1"
-authentikate = "0.1.1"
+authentikate = "0.1.2"
 strawberry-graphql = "^0.199.2"
 koherent = "0.1.1"
 channels = "^4.0.0"
 
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
```

