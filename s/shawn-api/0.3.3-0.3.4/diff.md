# Comparing `tmp/shawn_api-0.3.3.tar.gz` & `tmp/shawn_api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shawn_api-0.3.3.tar", last modified: Fri Aug  4 09:50:06 2023, max compression
+gzip compressed data, was "shawn_api-0.3.4.tar", last modified: Fri Aug  4 09:53:11 2023, max compression
```

## Comparing `shawn_api-0.3.3.tar` & `shawn_api-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 09:50:06.295912 shawn_api-0.3.3/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:50:06.294912 shawn_api-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 09:50:06.295912 shawn_api-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-08-04 09:50:04.000000 shawn_api-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:50:06.286912 shawn_api-0.3.3/shawn_api/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:49:32.000000 shawn_api-0.3.3/shawn_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:50:06.293912 shawn_api-0.3.3/shawn_api.egg-info/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:50:06.000000 shawn_api-0.3.3/shawn_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-08-04 09:50:06.000000 shawn_api-0.3.3/shawn_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 09:50:06.000000 shawn_api-0.3.3/shawn_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 09:50:06.000000 shawn_api-0.3.3/shawn_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-04 09:50:06.000000 shawn_api-0.3.3/shawn_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.987006 shawn_api-0.3.4/
+-rw-rw-rw-   0        0        0      651 2023-08-04 09:53:11.986006 shawn_api-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:53:11.987006 shawn_api-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-08-04 09:53:09.000000 shawn_api-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.974006 shawn_api-0.3.4/shawn_api/
+-rw-rw-rw-   0        0        0        0 2023-08-04 09:49:32.000000 shawn_api-0.3.4/shawn_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.985006 shawn_api-0.3.4/shawn_api/models/
+-rw-rw-rw-   0        0        0       33 2023-08-04 08:38:38.000000 shawn_api-0.3.4/shawn_api/models/__init__.py
+-rw-rw-rw-   0        0        0     1469 2023-08-04 08:58:38.000000 shawn_api-0.3.4/shawn_api/models/chat.py
+-rw-rw-rw-   0        0        0      148 2023-08-04 08:38:38.000000 shawn_api-0.3.4/shawn_api/models/model.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.981006 shawn_api-0.3.4/shawn_api.egg-info/
+-rw-rw-rw-   0        0        0      651 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/top_level.txt
```

### Comparing `shawn_api-0.3.3/PKG-INFO` & `shawn_api-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn_api
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shawn_api-0.3.3/setup.py` & `shawn_api-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 
 setup(
     name="shawn_api",
-    version="0.3.3",
+    version="0.3.4",
     description="A Python library for shawn test api",
     author="Shawn-Tam",
     author_email="shawn@dcoean.ai",
-    packages=["shawn_api"],
+    packages=["shawn_api", "shawn_api.models"],
     install_requires=[
         "requests",
         "aiohttp",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",  # or "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Intended Audience :: Developers",
```

### Comparing `shawn_api-0.3.3/shawn_api.egg-info/PKG-INFO` & `shawn_api-0.3.4/shawn_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

