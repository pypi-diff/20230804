# Comparing `tmp/usetools-0.0.1.tar.gz` & `tmp/usetools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usetools-0.0.1.tar", last modified: Fri Aug  4 10:50:12 2023, max compression
+gzip compressed data, was "usetools-0.0.2.tar", last modified: Fri Aug  4 11:00:03 2023, max compression
```

## Comparing `usetools-0.0.1.tar` & `usetools-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:50:12.953478 usetools-0.0.1/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-08-04 10:44:48.000000 usetools-0.0.1/LICENSE.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      466 2023-08-04 10:50:12.953478 usetools-0.0.1/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      545 2023-08-04 10:48:03.000000 usetools-0.0.1/pyproject.toml
--rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-08-04 10:50:12.953478 usetools-0.0.1/setup.cfg
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:50:12.953478 usetools-0.0.1/src/
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:50:12.953478 usetools-0.0.1/src/usetools/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:47:24.000000 usetools-0.0.1/src/usetools/__init__.py
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:47:33.000000 usetools-0.0.1/src/usetools/example.py
-drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 10:50:12.953478 usetools-0.0.1/src/usetools.egg-info/
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      466 2023-08-04 10:50:12.000000 usetools-0.0.1/src/usetools.egg-info/PKG-INFO
--rw-rw-r--   0 lubo      (1000) lubo      (1000)      219 2023-08-04 10:50:12.000000 usetools-0.0.1/src/usetools.egg-info/SOURCES.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-08-04 10:50:12.000000 usetools-0.0.1/src/usetools.egg-info/dependency_links.txt
--rw-rw-r--   0 lubo      (1000) lubo      (1000)        9 2023-08-04 10:50:12.000000 usetools-0.0.1/src/usetools.egg-info/top_level.txt
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:00:03.902286 usetools-0.0.2/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     1075 2023-08-04 10:44:48.000000 usetools-0.0.2/LICENSE.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      466 2023-08-04 11:00:03.902286 usetools-0.0.2/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      545 2023-08-04 10:59:34.000000 usetools-0.0.2/pyproject.toml
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       38 2023-08-04 11:00:03.902286 usetools-0.0.2/setup.cfg
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:00:03.902286 usetools-0.0.2/usetools/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)       93 2023-08-04 10:57:57.000000 usetools-0.0.2/usetools/__init__.py
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)     2136 2023-08-04 10:55:11.000000 usetools-0.0.2/usetools/addfunction.py
+drwxrwxr-x   0 lubo      (1000) lubo      (1000)        0 2023-08-04 11:00:03.902286 usetools-0.0.2/usetools.egg-info/
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      466 2023-08-04 11:00:03.000000 usetools-0.0.2/usetools.egg-info/PKG-INFO
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)      199 2023-08-04 11:00:03.000000 usetools-0.0.2/usetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        1 2023-08-04 11:00:03.000000 usetools-0.0.2/usetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lubo      (1000) lubo      (1000)        9 2023-08-04 11:00:03.000000 usetools-0.0.2/usetools.egg-info/top_level.txt
```

### Comparing `usetools-0.0.1/LICENSE.txt` & `usetools-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `usetools-0.0.1/pyproject.toml` & `usetools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usetools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Additional functions for python scripts"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

