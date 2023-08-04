# Comparing `tmp/thslt-1.0.2.tar.gz` & `tmp/thslt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thslt-1.0.2.tar", last modified: Fri Aug  4 16:31:44 2023, max compression
+gzip compressed data, was "thslt-1.0.3.tar", last modified: Fri Aug  4 18:12:51 2023, max compression
```

## Comparing `thslt-1.0.2.tar` & `thslt-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.017707 thslt-1.0.2/
--rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5665 2023-08-04 16:31:44.016703 thslt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5169 2023-08-04 16:30:05.000000 thslt-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 16:31:44.018705 thslt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-08-04 16:31:11.000000 thslt-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.010704 thslt-1.0.2/thslt.egg-info/
--rw-rw-rw-   0        0        0     5665 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.013705 thslt-1.0.2/thst/
--rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.2/thst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:12:51.670566 thslt-1.0.3/
+-rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5665 2023-08-04 18:12:51.669566 thslt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5169 2023-08-04 16:30:05.000000 thslt-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 18:12:51.671567 thslt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-08-04 18:10:29.000000 thslt-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:12:51.638568 thslt-1.0.3/thslt.egg-info/
+-rw-rw-rw-   0        0        0     5665 2023-08-04 18:12:50.000000 thslt-1.0.3/thslt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-08-04 18:12:51.000000 thslt-1.0.3/thslt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 18:12:50.000000 thslt-1.0.3/thslt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 18:12:50.000000 thslt-1.0.3/thslt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 18:12:51.666565 thslt-1.0.3/thst/
+-rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.3/thst/__init__.py
```

### Comparing `thslt-1.0.2/LICENSE.txt` & `thslt-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thslt-1.0.2/PKG-INFO` & `thslt-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `thslt-1.0.2/README.md` & `thslt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thslt-1.0.2/setup.py` & `thslt-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="thslt",
-    version="1.0.2",
+    version="1.0.3",
     author="Papangkon Ninarundech",
     author_email="papangkonsk@gmail.com",
     description="A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `thslt-1.0.2/thslt.egg-info/PKG-INFO` & `thslt-1.0.3/thslt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `thslt-1.0.2/thst/__init__.py` & `thslt-1.0.3/thst/__init__.py`

 * *Files identical despite different names*

