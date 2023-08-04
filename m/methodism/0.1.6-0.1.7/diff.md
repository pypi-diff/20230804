# Comparing `tmp/methodism-0.1.6.tar.gz` & `tmp/methodism-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.1.6.tar", last modified: Fri Aug  4 12:36:07 2023, max compression
+gzip compressed data, was "methodism-0.1.7.tar", last modified: Fri Aug  4 12:48:54 2023, max compression
```

## Comparing `methodism-0.1.6.tar` & `methodism-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.908416 methodism-0.1.6/
--rw-rw-rw-   0        0        0     4537 2023-08-04 12:36:07.908416 methodism-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4055 2023-06-05 09:21:58.000000 methodism-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.891892 methodism-0.1.6/methodism/
--rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.6/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.6/methodism/costumizing.py
--rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.6/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.6/methodism/error_messages.py
--rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.6/methodism/helper.py
--rw-rw-rw-   0        0        0     7019 2023-08-04 12:34:12.000000 methodism-0.1.6/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.907422 methodism-0.1.6/methodism.egg-info/
--rw-rw-rw-   0        0        0     4537 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-08-04 12:35:30.000000 methodism-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-08-04 12:36:07.910421 methodism-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 12:48:54.825121 methodism-0.1.7/
+-rw-rw-rw-   0        0        0     4537 2023-08-04 12:48:54.825121 methodism-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4055 2023-06-05 09:21:58.000000 methodism-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 12:48:54.805133 methodism-0.1.7/methodism/
+-rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.7/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.7/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.7/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.7/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.7/methodism/helper.py
+-rw-rw-rw-   0        0        0     7019 2023-08-04 12:34:12.000000 methodism-0.1.7/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:48:54.823121 methodism-0.1.7/methodism.egg-info/
+-rw-rw-rw-   0        0        0     4537 2023-08-04 12:48:54.000000 methodism-0.1.7/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-08-04 12:48:54.000000 methodism-0.1.7/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 12:48:54.000000 methodism-0.1.7/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 12:48:54.000000 methodism-0.1.7/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-08-04 12:48:23.000000 methodism-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-08-04 12:48:54.827122 methodism-0.1.7/setup.cfg
```

### Comparing `methodism-0.1.6/PKG-INFO` & `methodism-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.6
+Version: 0.1.7
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.6/README.md` & `methodism-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism/costumizing.py` & `methodism-0.1.7/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism/decors.py` & `methodism-0.1.7/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism/error_messages.py` & `methodism-0.1.7/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism/helper.py` & `methodism-0.1.7/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism/main.py` & `methodism-0.1.7/methodism/main.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.6/methodism.egg-info/PKG-INFO` & `methodism-0.1.7/methodism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.6
+Version: 0.1.7
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.6/pyproject.toml` & `methodism-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.1.6/setup.cfg` & `methodism-0.1.7/setup.cfg`

 * *Files identical despite different names*

