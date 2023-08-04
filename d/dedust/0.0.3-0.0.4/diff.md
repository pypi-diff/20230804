# Comparing `tmp/dedust-0.0.3.tar.gz` & `tmp/dedust-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedust-0.0.3.tar", last modified: Fri Aug  4 21:07:15 2023, max compression
+gzip compressed data, was "dedust-0.0.4.tar", last modified: Fri Aug  4 21:07:38 2023, max compression
```

## Comparing `dedust-0.0.3.tar` & `dedust-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2023-08-04 12:38:31.476509 dedust-0.0.3/.DS_Store
--rw-r--r--   0        0        0       26 2023-08-04 21:07:12.827629 dedust-0.0.3/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-20 20:08:32.030831 dedust-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1363 2023-08-04 21:06:55.812898 dedust-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.3/dedust/__init__.py
--rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.3/dedust/api.py
--rw-r--r--   0        0        0     1553 2023-06-11 09:24:19.451717 dedust-0.0.3/dedust/functions.py
--rw-r--r--   0        0        0      998 2023-06-11 09:24:41.554230 dedust-0.0.3/dedust/tokens.py
--rw-r--r--   0        0        0      580 2023-08-04 21:05:40.414918 dedust-0.0.3/examples/full.py
--rw-r--r--   0        0        0      286 2023-08-04 21:06:43.464851 dedust-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dedust-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-08-04 12:38:31.476509 dedust-0.0.4/.DS_Store
+-rw-r--r--   0        0        0       26 2023-08-04 21:07:12.827629 dedust-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-20 20:08:32.030831 dedust-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1363 2023-08-04 21:06:55.812898 dedust-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.4/dedust/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.4/dedust/api.py
+-rw-r--r--   0        0        0     1553 2023-06-11 09:24:19.451717 dedust-0.0.4/dedust/functions.py
+-rw-r--r--   0        0        0      998 2023-06-11 09:24:41.554230 dedust-0.0.4/dedust/tokens.py
+-rw-r--r--   0        0        0      580 2023-08-04 21:05:40.414918 dedust-0.0.4/examples/full.py
+-rw-r--r--   0        0        0      286 2023-08-04 21:07:35.967648 dedust-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dedust-0.0.4/PKG-INFO
```

### Comparing `dedust-0.0.3/.DS_Store` & `dedust-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/LICENSE.md` & `dedust-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/README.md` & `dedust-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/dedust/functions.py` & `dedust-0.0.4/dedust/functions.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/dedust/tokens.py` & `dedust-0.0.4/dedust/tokens.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/examples/full.py` & `dedust-0.0.4/examples/full.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.3/PKG-INFO` & `dedust-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedust
-Version: 0.0.3
+Version: 0.0.4
 Summary: DeDust - DeDust v2 API for Python.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: flask
 
 # DeDust API for Python
```

