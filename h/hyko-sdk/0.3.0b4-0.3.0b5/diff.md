# Comparing `tmp/hyko_sdk-0.3.0b4.tar.gz` & `tmp/hyko_sdk-0.3.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b4.tar", last modified: Fri Aug  4 19:48:33 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b5.tar", last modified: Fri Aug  4 19:54:02 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b4.tar` & `hyko_sdk-0.3.0b5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b4/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b4/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b4/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b4/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1377 2023-08-04 19:41:51.000000 hyko_sdk-0.3.0b4/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b4/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      116 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b4/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      443 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:54:02.942993 hyko_sdk-0.3.0b5/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:54:02.942993 hyko_sdk-0.3.0b5/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b5/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:54:02.942993 hyko_sdk-0.3.0b5/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b5/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b5/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b5/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1377 2023-08-04 19:41:51.000000 hyko_sdk-0.3.0b5/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b5/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:54:02.942993 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:54:02.000000 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-04 19:54:02.000000 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 19:54:02.000000 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      114 2023-08-04 19:54:02.000000 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 19:54:02.000000 hyko_sdk-0.3.0b5/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b5/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      441 2023-08-04 19:54:02.946327 hyko_sdk-0.3.0b5/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b4/hyko_sdk/error.py` & `hyko_sdk-0.3.0b5/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b4/hyko_sdk/io.py` & `hyko_sdk-0.3.0b5/hyko_sdk/io.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b4/hyko_sdk/metadata.py` & `hyko_sdk-0.3.0b5/hyko_sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b4/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b5/hyko_sdk/utils.py`

 * *Files identical despite different names*

