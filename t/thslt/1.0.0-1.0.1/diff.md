# Comparing `tmp/thslt-1.0.0.tar.gz` & `tmp/thslt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thslt-1.0.0.tar", last modified: Fri Aug  4 16:12:26 2023, max compression
+gzip compressed data, was "thslt-1.0.1.tar", last modified: Fri Aug  4 16:22:37 2023, max compression
```

## Comparing `thslt-1.0.0.tar` & `thslt-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:12:26.699252 thslt-1.0.0/
--rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5663 2023-08-04 16:12:26.662254 thslt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5167 2023-08-04 16:11:45.000000 thslt-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 16:12:26.699252 thslt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-08-04 16:12:07.000000 thslt-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:12:26.656253 thslt-1.0.0/thslt.egg-info/
--rw-rw-rw-   0        0        0     5663 2023-08-04 16:12:26.000000 thslt-1.0.0/thslt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-08-04 16:12:26.000000 thslt-1.0.0/thslt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:12:26.000000 thslt-1.0.0/thslt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 16:12:26.000000 thslt-1.0.0/thslt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 16:12:26.659254 thslt-1.0.0/thst/
--rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.0/thst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.483991 thslt-1.0.1/
+-rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5663 2023-08-04 16:22:37.479992 thslt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5167 2023-08-04 16:11:45.000000 thslt-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 16:22:37.483991 thslt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-08-04 16:21:54.000000 thslt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.472992 thslt-1.0.1/thslt.egg-info/
+-rw-rw-rw-   0        0        0     5663 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.476992 thslt-1.0.1/thst/
+-rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.1/thst/__init__.py
```

### Comparing `thslt-1.0.0/LICENSE.txt` & `thslt-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thslt-1.0.0/PKG-INFO` & `thslt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `thslt-1.0.0/README.md` & `thslt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `thslt-1.0.0/setup.py` & `thslt-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="thslt",
-    version="1.0.0",
+    version="1.0.1",
     author="Papangkon Ninarundech",
     author_email="papangkonsk@gmail.com",
     description="A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `thslt-1.0.0/thslt.egg-info/PKG-INFO` & `thslt-1.0.1/thslt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `thslt-1.0.0/thst/__init__.py` & `thslt-1.0.1/thst/__init__.py`

 * *Files identical despite different names*

