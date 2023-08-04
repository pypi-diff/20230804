# Comparing `tmp/idelium-1.0.5.tar.gz` & `tmp/idelium-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelium-1.0.5.tar", last modified: Thu Aug  3 14:58:17 2023, max compression
+gzip compressed data, was "idelium-1.0.6.tar", last modified: Fri Aug  4 16:07:45 2023, max compression
```

## Comparing `idelium-1.0.5.tar` & `idelium-1.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.658455 idelium-1.0.5/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      541 2021-11-05 11:16:26.000000 idelium-1.0.5/LICENSE.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)      218 2023-07-03 14:50:05.000000 idelium-1.0.5/MANIFEST.in
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-08-03 14:58:17.658579 idelium-1.0.5/PKG-INFO
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     2344 2023-07-20 16:52:00.000000 idelium-1.0.5/README.md
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2033 2023-06-30 13:38:23.000000 idelium-1.0.5/pyproject.toml
--rw-rw-rw-   0 idelfuschini   (501) staff       (20)     1281 2023-08-03 14:58:17.659804 idelium-1.0.5/setup.cfg
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     4455 2023-07-05 13:06:58.000000 idelium-1.0.5/setup.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.643385 idelium-1.0.5/src/
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.646199 idelium-1.0.5/src/idelium/
--rw-r--r--   0 idelfuschini   (501) staff       (20)      361 2023-07-05 07:52:27.000000 idelium-1.0.5/src/idelium/__init__.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.650578 idelium-1.0.5/src/idelium/_internal/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2023-07-03 13:43:10.000000 idelium-1.0.5/src/idelium/_internal/__init__.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.651539 idelium-1.0.5/src/idelium/_internal/bdd/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2022-02-21 11:18:20.000000 idelium-1.0.5/src/idelium/_internal/bdd/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      193 2022-02-21 18:55:48.000000 idelium-1.0.5/src/idelium/_internal/bdd/bdd.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      273 2022-02-21 18:29:38.000000 idelium-1.0.5/src/idelium/_internal/bdd/webservice.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.654209 idelium-1.0.5/src/idelium/_internal/commons/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.5/src/idelium/_internal/commons/__init__.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    13873 2021-12-02 13:19:23.000000 idelium-1.0.5/src/idelium/_internal/commons/androideventkey.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      822 2021-12-02 13:22:25.000000 idelium-1.0.5/src/idelium/_internal/commons/ideliumprinter.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      494 2021-12-02 14:11:51.000000 idelium-1.0.5/src/idelium/_internal/commons/proxy.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)      152 2021-12-02 14:15:27.000000 idelium-1.0.5/src/idelium/_internal/commons/resultenum.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)      794 2021-12-02 16:50:19.000000 idelium-1.0.5/src/idelium/_internal/commons/seleniumby.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2798 2021-12-02 16:45:25.000000 idelium-1.0.5/src/idelium/_internal/commons/seleniumkeyevent.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.654510 idelium-1.0.5/src/idelium/_internal/extra/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.5/src/idelium/_internal/extra/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     9027 2023-07-05 07:54:25.000000 idelium-1.0.5/src/idelium/_internal/ideliumclib.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     6392 2023-07-21 16:55:51.000000 idelium-1.0.5/src/idelium/_internal/ideliummanager.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3054 2022-01-17 18:40:07.000000 idelium-1.0.5/src/idelium/_internal/ideliumserver.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    15865 2023-07-21 14:34:45.000000 idelium-1.0.5/src/idelium/_internal/ideliumws.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)     2558 2023-08-03 14:58:10.000000 idelium-1.0.5/src/idelium/_internal/main.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.655400 idelium-1.0.5/src/idelium/_internal/thirdparties/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2600 2023-07-03 16:48:58.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/ideliumpostman.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    19193 2023-07-03 16:48:58.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/ideliumzephyr.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.656740 idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/
--rw-r--r--   0 idelfuschini   (501) staff       (20)        0 2022-05-23 20:39:45.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/__init__.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     6996 2022-08-26 14:29:29.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/core.py
--rw-r--r--   0 idelfuschini   (501) staff       (20)     2846 2022-05-23 20:39:45.000000 idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/extractors.py
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.657947 idelium-1.0.5/src/idelium/_internal/wrappers/
--rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.5/src/idelium/_internal/wrappers/__init__.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    29783 2023-07-03 16:48:58.000000 idelium-1.0.5/src/idelium/_internal/wrappers/ideliumappium.py
--rw-rw-r--   0 idelfuschini   (501) staff       (20)    18419 2023-08-03 14:47:40.000000 idelium-1.0.5/src/idelium/_internal/wrappers/ideliumselenium.py
--rw-rw-rw-   0 idelfuschini   (501) staff       (20)      294 2023-07-03 13:37:10.000000 idelium-1.0.5/src/idelium/py.typed
-drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-03 14:58:17.648408 idelium-1.0.5/src/idelium.egg-info/
--rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/PKG-INFO
--rw-r--r--   0 idelfuschini   (501) staff       (20)     1496 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/SOURCES.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/dependency_links.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)       56 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/entry_points.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-03 14:35:54.000000 idelium-1.0.5/src/idelium.egg-info/not-zip-safe
--rw-r--r--   0 idelfuschini   (501) staff       (20)      111 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/requires.txt
--rw-r--r--   0 idelfuschini   (501) staff       (20)        8 2023-08-03 14:58:17.000000 idelium-1.0.5/src/idelium.egg-info/top_level.txt
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.192076 idelium-1.0.6/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      541 2021-11-05 11:16:26.000000 idelium-1.0.6/LICENSE.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      218 2023-07-03 14:50:05.000000 idelium-1.0.6/MANIFEST.in
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-08-04 16:07:45.192189 idelium-1.0.6/PKG-INFO
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     2344 2023-07-20 16:52:00.000000 idelium-1.0.6/README.md
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2033 2023-06-30 13:38:23.000000 idelium-1.0.6/pyproject.toml
+-rw-rw-rw-   0 idelfuschini   (501) staff       (20)     1281 2023-08-04 16:07:45.195690 idelium-1.0.6/setup.cfg
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     4455 2023-07-05 13:06:58.000000 idelium-1.0.6/setup.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.182890 idelium-1.0.6/src/
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.185059 idelium-1.0.6/src/idelium/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      361 2023-07-05 07:52:27.000000 idelium-1.0.6/src/idelium/__init__.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.187650 idelium-1.0.6/src/idelium/_internal/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2023-07-03 13:43:10.000000 idelium-1.0.6/src/idelium/_internal/__init__.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.188100 idelium-1.0.6/src/idelium/_internal/bdd/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2022-02-21 11:18:20.000000 idelium-1.0.6/src/idelium/_internal/bdd/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      193 2022-02-21 18:55:48.000000 idelium-1.0.6/src/idelium/_internal/bdd/bdd.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      273 2022-02-21 18:29:38.000000 idelium-1.0.6/src/idelium/_internal/bdd/webservice.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.189705 idelium-1.0.6/src/idelium/_internal/commons/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.6/src/idelium/_internal/commons/__init__.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    13873 2021-12-02 13:19:23.000000 idelium-1.0.6/src/idelium/_internal/commons/androideventkey.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      822 2021-12-02 13:22:25.000000 idelium-1.0.6/src/idelium/_internal/commons/ideliumprinter.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      494 2021-12-02 14:11:51.000000 idelium-1.0.6/src/idelium/_internal/commons/proxy.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)      152 2021-12-02 14:15:27.000000 idelium-1.0.6/src/idelium/_internal/commons/resultenum.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      794 2021-12-02 16:50:19.000000 idelium-1.0.6/src/idelium/_internal/commons/seleniumby.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2798 2021-12-02 16:45:25.000000 idelium-1.0.6/src/idelium/_internal/commons/seleniumkeyevent.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.189877 idelium-1.0.6/src/idelium/_internal/extra/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.6/src/idelium/_internal/extra/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     9143 2023-08-04 15:31:57.000000 idelium-1.0.6/src/idelium/_internal/ideliumclib.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     6392 2023-08-04 14:23:42.000000 idelium-1.0.6/src/idelium/_internal/ideliummanager.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3054 2022-01-17 18:40:07.000000 idelium-1.0.6/src/idelium/_internal/ideliumserver.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    16061 2023-08-04 16:03:11.000000 idelium-1.0.6/src/idelium/_internal/ideliumws.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)     2558 2023-08-04 13:52:18.000000 idelium-1.0.6/src/idelium/_internal/main.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.190301 idelium-1.0.6/src/idelium/_internal/thirdparties/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2600 2023-07-03 16:48:58.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/ideliumpostman.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    19193 2023-07-03 16:48:58.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/ideliumzephyr.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.190787 idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        0 2022-05-23 20:39:45.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/__init__.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     6996 2022-08-26 14:29:29.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/core.py
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     2846 2022-05-23 20:39:45.000000 idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/extractors.py
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.191843 idelium-1.0.6/src/idelium/_internal/wrappers/
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)        0 2021-08-13 11:45:16.000000 idelium-1.0.6/src/idelium/_internal/wrappers/__init__.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    29781 2023-08-04 15:48:00.000000 idelium-1.0.6/src/idelium/_internal/wrappers/ideliumappium.py
+-rw-rw-r--   0 idelfuschini   (501) staff       (20)    18432 2023-08-04 16:07:38.000000 idelium-1.0.6/src/idelium/_internal/wrappers/ideliumselenium.py
+-rw-rw-rw-   0 idelfuschini   (501) staff       (20)      294 2023-07-03 13:37:10.000000 idelium-1.0.6/src/idelium/py.typed
+drwxr-xr-x   0 idelfuschini   (501) staff       (20)        0 2023-08-04 16:07:45.186432 idelium-1.0.6/src/idelium.egg-info/
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     3648 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/PKG-INFO
+-rw-r--r--   0 idelfuschini   (501) staff       (20)     1496 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/SOURCES.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/dependency_links.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)       56 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/entry_points.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        1 2023-07-03 14:35:54.000000 idelium-1.0.6/src/idelium.egg-info/not-zip-safe
+-rw-r--r--   0 idelfuschini   (501) staff       (20)      111 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/requires.txt
+-rw-r--r--   0 idelfuschini   (501) staff       (20)        8 2023-08-04 16:07:45.000000 idelium-1.0.6/src/idelium.egg-info/top_level.txt
```

### Comparing `idelium-1.0.5/LICENSE.txt` & `idelium-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/PKG-INFO` & `idelium-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelium
-Version: 1.0.5
+Version: 1.0.6
 Summary: Command line Test Automation Tool
 Home-page: https://idelium.io/
 Author: Idel Fuschini
 Author-email: idel.fuschini@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/idelium/idelium-cli/issues
 Project-URL: Project, https://idelium.io
```

### Comparing `idelium-1.0.5/README.md` & `idelium-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/pyproject.toml` & `idelium-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/setup.cfg` & `idelium-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/setup.py` & `idelium-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/commons/androideventkey.py` & `idelium-1.0.6/src/idelium/_internal/commons/androideventkey.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/commons/ideliumprinter.py` & `idelium-1.0.6/src/idelium/_internal/commons/ideliumprinter.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/commons/seleniumby.py` & `idelium-1.0.6/src/idelium/_internal/commons/seleniumby.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/commons/seleniumkeyevent.py` & `idelium-1.0.6/src/idelium/_internal/commons/seleniumkeyevent.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/ideliumclib.py` & `idelium-1.0.6/src/idelium/_internal/ideliumclib.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,26 +109,28 @@
             'ideliumServer': False,
             'ideliumServerPort': 8691,
         }
     def define_parameters(self,args,ideliumws,printer):
         ''' set all necessary parameters '''
         cl_params= self.get_default_parameters()
         check_required=self.get_reguired_parameters()
-        cl_params['dir_idelium_scripts'] = tempfile.gettempdir()
+        cl_params['dir_idelium_scripts'] = tempfile.mkdtemp()
         count=0
         for i in args:
             array_command=i.split("=")
             command=array_command[0][2:]
             if command in cl_params:
                 if command == 'ideliumKey':
                     cl_params['ideliumKey']=''
                     if len(array_command)==3:
                         cl_params['ideliumKey'] = array_command[1] + '=' 
                     else:
                         cl_params['ideliumKey'] = array_command[1]
+                elif command == "forcedownload":                
+                    cl_params['forcedownload'] = True
                 elif command == 'ideliumServer':
                     cl_params['ideliumServer'] = True
                 elif command == 'ideliumServerPort': 
                     cl_params['ideliumServerPort'] = int(array_command[1])
                 else:
                     cl_params[command]=array_command[1]
                 if command in check_required:
```

### Comparing `idelium-1.0.5/src/idelium/_internal/ideliummanager.py` & `idelium-1.0.6/src/idelium/_internal/ideliummanager.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/ideliumserver.py` & `idelium-1.0.6/src/idelium/_internal/ideliumserver.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/ideliumws.py` & `idelium-1.0.6/src/idelium/_internal/ideliumws.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,29 +220,32 @@
                                        config["is_debug"])
         for plugin_det in json_plugins:
             url = config["api_idelium"] + "plugin/" + str(plugin_det["id"])
             json_plugin = Connection.start("GET", url, None,
                                           config["ideliumKey"],
                                           config["is_debug"])
             #save  plugin for projectId
+            json_plugin_code=json.loads(json_plugin['code'])
             array_plugins[json_plugin["name"]] = json_plugin["code"]
-            py_file_path = (configuration_directories[TypeDir.PLUGIN_DIR] + "/" +
-                          json_plugin["name"] + ".py")
+            #py_file_path = (configuration_directories[TypeDir.PLUGIN_DIR] + "/" + json_plugin["name"] + ".py"
             plugins_dir = config["dir_idelium_scripts"] + "/plugin"
+            py_file_path=(plugins_dir + "/" +
+                          json_plugin["name"] + ".py")
             if Path(plugins_dir).exists() is False:
-                os.mkdir(plugins_dir)
+                #os.mkdir(plugins_dir)
+                os.makedirs(plugins_dir)
                 if config["is_debug"] is True:
                     print("created temporary directory", plugins_dir)
-            py_file_path = plugins_dir + "/" + json_plugin["name"] + ".py"
-
-            if Path(py_file_path).exists(
-            ) is False or config["forcedownload"] is True:
-                py_file = open(py_file_path, "wt")
-                py_file.write(json_plugin["code"])
-                py_file.close()
+            if config["is_debug"] is True:
+                print("plugin file saved in:", py_file_path)
+            #if Path(py_file_path).exists(
+            #) is False or config["forcedownload"] is True:
+            py_file = open(py_file_path, "wt")
+            py_file.write(json_plugin_code[0])
+            py_file.close()
         #download environments
         json_environments = self.get_environments(config)
         printer.success("finish download file")
         for env in json_environments:
             url = config["api_idelium"] + "environment/" + str(env["id"])
             json_environment = Connection.start("GET", url, None,
                                                config["ideliumKey"],
```

### Comparing `idelium-1.0.5/src/idelium/_internal/main.py` & `idelium-1.0.6/src/idelium/_internal/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from idelium._internal.commons.ideliumprinter import InitPrinter
 
 
 idelium=StartManager()
 printer=InitPrinter()
 ideliumws=IdeliumWs()
 idelium_cl_lib=InitIdelium()
-IDELIUM_VERSION='1.0.5'
+IDELIUM_VERSION='1.0.6'
 
 def main(args: Optional[List[str]] = None) -> int:
     printer.print_important_text("Idelium Command Line " + IDELIUM_VERSION)
     printer.print_important_text ("Selenium version:" + idelium_cl_lib.get_selenium_version())
     if args is None:
         args = sys.argv
     define_parameters= idelium_cl_lib.define_parameters(args,ideliumws,printer)
```

### Comparing `idelium-1.0.5/src/idelium/_internal/thirdparties/ideliumpostman.py` & `idelium-1.0.6/src/idelium/_internal/thirdparties/ideliumpostman.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/thirdparties/ideliumzephyr.py` & `idelium-1.0.6/src/idelium/_internal/thirdparties/ideliumzephyr.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/core.py` & `idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/core.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/thirdparties/postpy2/extractors.py` & `idelium-1.0.6/src/idelium/_internal/thirdparties/postpy2/extractors.py`

 * *Files identical despite different names*

### Comparing `idelium-1.0.5/src/idelium/_internal/wrappers/ideliumappium.py` & `idelium-1.0.6/src/idelium/_internal/wrappers/ideliumappium.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,9 +714,9 @@
                 "appium_finger_print" : self.appium_finger_print,
                 "appium_find_element_by_accessibility_id" :
                     self.appium_find_element_by_accessibility_id,
                 "appium_switch_to" : self.appium_switch_to,
         }
         if command in commands.keys():
             return commands[command](driver,obj_config,object_step)
-        printer.danger ('Idelium Appium | action non trovata:' + command)
+        printer.danger ('Idelium Appium | action not found:' + command)
         return None
```

### Comparing `idelium-1.0.5/src/idelium/_internal/wrappers/ideliumselenium.py` & `idelium-1.0.6/src/idelium/_internal/wrappers/ideliumselenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,9 +428,9 @@
             "open_browser": self.open_browser,
             "write_localstorage": self.write_localstorage,
             "screen_shot": self.screen_shot,
             "sleep": self.sleep,
         }
         if command in commands.keys():
             return commands[command](driver, obj_config, object_step)
-        printer.danger("Idelium Selenium | action non trovata:" + command)
+        printer.warning("Idelium Selenium | action nof found try as plugin:" + command)
         return None
```

### Comparing `idelium-1.0.5/src/idelium.egg-info/PKG-INFO` & `idelium-1.0.6/src/idelium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelium
-Version: 1.0.5
+Version: 1.0.6
 Summary: Command line Test Automation Tool
 Home-page: https://idelium.io/
 Author: Idel Fuschini
 Author-email: idel.fuschini@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/idelium/idelium-cli/issues
 Project-URL: Project, https://idelium.io
```

### Comparing `idelium-1.0.5/src/idelium.egg-info/SOURCES.txt` & `idelium-1.0.6/src/idelium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

