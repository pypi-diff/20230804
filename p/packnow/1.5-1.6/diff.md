# Comparing `tmp/packnow-1.5.tar.gz` & `tmp/packnow-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packnow-1.5.tar", last modified: Thu Aug  3 13:02:35 2023, max compression
+gzip compressed data, was "packnow-1.6.tar", last modified: Thu Aug  3 13:06:17 2023, max compression
```

## Comparing `packnow-1.5.tar` & `packnow-1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.312289 packnow-1.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-08-03 12:54:35.000000 packnow-1.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:02:35.316290 packnow-1.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:51:15.000000 packnow-1.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.220280 packnow-1.5/packnow/
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-08-03 12:59:55.000000 packnow-1.5/packnow/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.5/packnow/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:46:02.000000 packnow-1.5/packnow/main.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.312289 packnow-1.5/packnow.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      295 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-08-03 13:02:28.000000 packnow-1.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-08-03 13:02:35.316290 packnow-1.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      707 2023-08-03 13:02:33.000000 packnow-1.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:06:17.523173 packnow-1.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-08-03 12:54:35.000000 packnow-1.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:06:17.523173 packnow-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:51:15.000000 packnow-1.6/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:06:17.519172 packnow-1.6/packnow/
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-08-03 12:59:55.000000 packnow-1.6/packnow/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.6/packnow/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:46:02.000000 packnow-1.6/packnow/main.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:06:17.523173 packnow-1.6/packnow.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:06:16.000000 packnow-1.6/packnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      295 2023-08-03 13:06:17.000000 packnow-1.6/packnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 13:06:16.000000 packnow-1.6/packnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 13:06:16.000000 packnow-1.6/packnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2023-08-03 13:06:16.000000 packnow-1.6/packnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 13:06:16.000000 packnow-1.6/packnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      803 2023-08-03 13:06:05.000000 packnow-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-08-03 13:06:17.527173 packnow-1.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      707 2023-08-03 13:06:07.000000 packnow-1.6/setup.py
```

### Comparing `packnow-1.5/LICENSE` & `packnow-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `packnow-1.5/PKG-INFO` & `packnow-1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.5
+Version: 1.6
 Summary: Pack everything, now.
 Author: AWeirdDev
 Author-email: AWeirdDev <aweirdscratcher@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `packnow-1.5/packnow/main.py` & `packnow-1.6/packnow/main.py`

 * *Files identical despite different names*

### Comparing `packnow-1.5/packnow.egg-info/PKG-INFO` & `packnow-1.6/packnow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.5
+Version: 1.6
 Summary: Pack everything, now.
 Author: AWeirdDev
 Author-email: AWeirdDev <aweirdscratcher@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `packnow-1.5/pyproject.toml` & `packnow-1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "packnow"
-version = "1.5"
+version = "1.6"
 description = "Pack everything, now."
 keywords = ["pack", "packing", "packnow"]
 authors = [
   { name = "AWeirdDev", email = "aweirdscratcher@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
@@ -22,10 +22,13 @@
   "termcolor", 
   "fastapi", 
   "questionary", 
   "websockets", 
   "uvicorn",
 ]
 
+[project.scripts]
+packnow = "packnow.main:main"
+
 [project.urls]
 "Homepage" = "https://github.com/AWeirdScratcher/packnow"
 "Bug Tracker" = "https://github.com/AWeirdScratcher/packnow/issues"
```

### Comparing `packnow-1.5/setup.py` & `packnow-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
   name="packnow",
   author="AWeirdDev",
-  version="1.5",
+  version="1.6",
   license="MIT License",
   description="Pack everything, now. Cross-platform.",
   long_description=readme,
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['packnow'],
   classifiers=[
```

