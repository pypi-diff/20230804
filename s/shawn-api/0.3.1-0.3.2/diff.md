# Comparing `tmp/shawn_api-0.3.1.tar.gz` & `tmp/shawn_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shawn_api-0.3.1.tar", last modified: Fri Aug  4 09:31:09 2023, max compression
+gzip compressed data, was "shawn_api-0.3.2.tar", last modified: Fri Aug  4 09:31:59 2023, max compression
```

## Comparing `shawn_api-0.3.1.tar` & `shawn_api-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 09:31:09.555401 shawn_api-0.3.1/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:31:09.554402 shawn_api-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 09:31:09.545403 shawn_api-0.3.1/models/
--rw-rw-rw-   0        0        0       33 2023-08-04 08:38:38.000000 shawn_api-0.3.1/models/__init__.py
--rw-rw-rw-   0        0        0     1469 2023-08-04 08:58:38.000000 shawn_api-0.3.1/models/chat.py
--rw-rw-rw-   0        0        0      148 2023-08-04 08:38:38.000000 shawn_api-0.3.1/models/model.py
--rw-rw-rw-   0        0        0       42 2023-08-04 09:31:09.555401 shawn_api-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-08-04 09:30:57.000000 shawn_api-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:31:09.553403 shawn_api-0.3.1/shawn_api.egg-info/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:31:09.000000 shawn_api-0.3.1/shawn_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-04 09:31:09.000000 shawn_api-0.3.1/shawn_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 09:31:09.000000 shawn_api-0.3.1/shawn_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 09:31:09.000000 shawn_api-0.3.1/shawn_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 09:31:09.000000 shawn_api-0.3.1/shawn_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 09:31:59.534705 shawn_api-0.3.2/
+-rw-rw-rw-   0        0        0      651 2023-08-04 09:31:59.533704 shawn_api-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 09:31:59.525705 shawn_api-0.3.2/models/
+-rw-rw-rw-   0        0        0       33 2023-08-04 08:38:38.000000 shawn_api-0.3.2/models/__init__.py
+-rw-rw-rw-   0        0        0     1469 2023-08-04 08:58:38.000000 shawn_api-0.3.2/models/chat.py
+-rw-rw-rw-   0        0        0      148 2023-08-04 08:38:38.000000 shawn_api-0.3.2/models/model.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:31:59.534705 shawn_api-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-08-04 09:31:57.000000 shawn_api-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:31:59.532731 shawn_api-0.3.2/shawn_api.egg-info/
+-rw-rw-rw-   0        0        0      651 2023-08-04 09:31:59.000000 shawn_api-0.3.2/shawn_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-04 09:31:59.000000 shawn_api-0.3.2/shawn_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:31:59.000000 shawn_api-0.3.2/shawn_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 09:31:59.000000 shawn_api-0.3.2/shawn_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 09:31:59.000000 shawn_api-0.3.2/shawn_api.egg-info/top_level.txt
```

### Comparing `shawn_api-0.3.1/PKG-INFO` & `shawn_api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn_api
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shawn_api-0.3.1/models/chat.py` & `shawn_api-0.3.2/models/chat.py`

 * *Files identical despite different names*

### Comparing `shawn_api-0.3.1/setup.py` & `shawn_api-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="shawn_api",
-    version="0.3.1",
+    version="0.3.2",
     description="A Python library for shawn test api",
     author="Shawn-Tam",
     author_email="shawn@dcoean.ai",
     packages=["models"],
     install_requires=[
         "requests",
         "aiohttp",
```

### Comparing `shawn_api-0.3.1/shawn_api.egg-info/PKG-INFO` & `shawn_api-0.3.2/shawn_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

