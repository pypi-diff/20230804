# Comparing `tmp/AndroidTools-0.1.0.tar.gz` & `tmp/AndroidTools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AndroidTools-0.1.0.tar", last modified: Tue Aug  1 22:06:02 2023, max compression
+gzip compressed data, was "AndroidTools-0.1.1.tar", last modified: Fri Aug  4 03:36:52 2023, max compression
```

## Comparing `AndroidTools-0.1.0.tar` & `AndroidTools-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.767173 AndroidTools-0.1.0/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.762184 AndroidTools-0.1.0/AndTools/
--rw-r--r--   0 1a         (501) staff       (20)     2562 2023-07-17 08:59:51.000000 AndroidTools-0.1.0/AndTools/Pack.py
--rw-r--r--   0 1a         (501) staff       (20)     9319 2023-08-01 19:12:05.000000 AndroidTools-0.1.0/AndTools/TEA.py
--rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.1.0/AndTools/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      269 2023-07-17 08:24:35.000000 AndroidTools-0.1.0/AndTools/byte_.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.762846 AndroidTools-0.1.0/AndroidTools.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      397 2023-08-01 22:06:02.000000 AndroidTools-0.1.0/AndroidTools.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      460 2023-08-01 22:06:02.000000 AndroidTools-0.1.0/AndroidTools.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2023-08-01 22:06:02.000000 AndroidTools-0.1.0/AndroidTools.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)       19 2023-08-01 22:06:02.000000 AndroidTools-0.1.0/AndroidTools.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.764175 AndroidTools-0.1.0/Jce/
--rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.1.0/Jce/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.1.0/Jce/bytebuffer.py
--rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.1.0/Jce/exception.py
--rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.1.0/Jce/stream.py
--rw-r--r--   0 1a         (501) staff       (20)     1746 2023-08-01 06:13:47.000000 AndroidTools-0.1.0/Jce/struct.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.766340 AndroidTools-0.1.0/Jce_b/
--rw-r--r--   0 1a         (501) staff       (20)     1153 2023-08-01 06:18:45.000000 AndroidTools-0.1.0/Jce_b/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     5686 2023-08-01 05:44:52.000000 AndroidTools-0.1.0/Jce_b/buffer.py
--rw-r--r--   0 1a         (501) staff       (20)     1035 2023-08-01 05:44:52.000000 AndroidTools-0.1.0/Jce_b/head.py
--rw-r--r--   0 1a         (501) staff       (20)      203 2023-08-01 06:44:28.000000 AndroidTools-0.1.0/Jce_b/jcetypes.py
--rw-r--r--   0 1a         (501) staff       (20)    12506 2023-08-01 22:04:55.000000 AndroidTools-0.1.0/Jce_b/reader.py
--rw-r--r--   0 1a         (501) staff       (20)      426 2023-08-01 05:44:52.000000 AndroidTools-0.1.0/Jce_b/struct.py
--rw-r--r--   0 1a         (501) staff       (20)      522 2023-08-01 05:44:52.000000 AndroidTools-0.1.0/Jce_b/typing.py
--rw-r--r--   0 1a         (501) staff       (20)     6467 2023-08-01 10:53:17.000000 AndroidTools-0.1.0/Jce_b/writer.py
--rw-r--r--   0 1a         (501) staff       (20)      397 2023-08-01 22:06:02.766959 AndroidTools-0.1.0/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.1.0/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2023-08-01 22:06:02.767219 AndroidTools-0.1.0/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      636 2023-08-01 22:06:02.000000 AndroidTools-0.1.0/setup.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 22:06:02.766652 AndroidTools-0.1.0/test/
--rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.1.0/test/test_Jce.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.093183 AndroidTools-0.1.1/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.088631 AndroidTools-0.1.1/AndTools/
+-rw-r--r--   0 1a         (501) staff       (20)     2562 2023-07-17 08:59:51.000000 AndroidTools-0.1.1/AndTools/Pack.py
+-rw-r--r--   0 1a         (501) staff       (20)     9319 2023-08-01 19:12:05.000000 AndroidTools-0.1.1/AndTools/TEA.py
+-rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.1.1/AndTools/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      414 2023-08-04 03:36:25.000000 AndroidTools-0.1.1/AndTools/byte_.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.089203 AndroidTools-0.1.1/AndroidTools.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      397 2023-08-04 03:36:52.000000 AndroidTools-0.1.1/AndroidTools.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      460 2023-08-04 03:36:52.000000 AndroidTools-0.1.1/AndroidTools.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2023-08-04 03:36:52.000000 AndroidTools-0.1.1/AndroidTools.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)       19 2023-08-04 03:36:52.000000 AndroidTools-0.1.1/AndroidTools.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.090379 AndroidTools-0.1.1/Jce/
+-rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.1.1/Jce/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.1.1/Jce/bytebuffer.py
+-rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.1.1/Jce/exception.py
+-rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.1.1/Jce/stream.py
+-rw-r--r--   0 1a         (501) staff       (20)     1746 2023-08-01 06:13:47.000000 AndroidTools-0.1.1/Jce/struct.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.092389 AndroidTools-0.1.1/Jce_b/
+-rw-r--r--   0 1a         (501) staff       (20)     1153 2023-08-01 06:18:45.000000 AndroidTools-0.1.1/Jce_b/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     5686 2023-08-01 05:44:52.000000 AndroidTools-0.1.1/Jce_b/buffer.py
+-rw-r--r--   0 1a         (501) staff       (20)     1035 2023-08-01 05:44:52.000000 AndroidTools-0.1.1/Jce_b/head.py
+-rw-r--r--   0 1a         (501) staff       (20)      203 2023-08-01 06:44:28.000000 AndroidTools-0.1.1/Jce_b/jcetypes.py
+-rw-r--r--   0 1a         (501) staff       (20)    12506 2023-08-01 22:04:55.000000 AndroidTools-0.1.1/Jce_b/reader.py
+-rw-r--r--   0 1a         (501) staff       (20)      426 2023-08-01 05:44:52.000000 AndroidTools-0.1.1/Jce_b/struct.py
+-rw-r--r--   0 1a         (501) staff       (20)      522 2023-08-01 05:44:52.000000 AndroidTools-0.1.1/Jce_b/typing.py
+-rw-r--r--   0 1a         (501) staff       (20)     6467 2023-08-01 10:53:17.000000 AndroidTools-0.1.1/Jce_b/writer.py
+-rw-r--r--   0 1a         (501) staff       (20)      397 2023-08-04 03:36:52.092942 AndroidTools-0.1.1/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.1.1/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2023-08-04 03:36:52.093233 AndroidTools-0.1.1/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      636 2023-08-04 03:36:49.000000 AndroidTools-0.1.1/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-04 03:36:52.092626 AndroidTools-0.1.1/test/
+-rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.1.1/test/test_Jce.py
```

### Comparing `AndroidTools-0.1.0/AndTools/Pack.py` & `AndroidTools-0.1.1/AndTools/Pack.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/AndTools/TEA.py` & `AndroidTools-0.1.1/AndTools/TEA.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce/bytebuffer.py` & `AndroidTools-0.1.1/Jce/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce/stream.py` & `AndroidTools-0.1.1/Jce/stream.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce/struct.py` & `AndroidTools-0.1.1/Jce/struct.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/__init__.py` & `AndroidTools-0.1.1/Jce_b/__init__.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/buffer.py` & `AndroidTools-0.1.1/Jce_b/buffer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/head.py` & `AndroidTools-0.1.1/Jce_b/head.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/reader.py` & `AndroidTools-0.1.1/Jce_b/reader.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/typing.py` & `AndroidTools-0.1.1/Jce_b/typing.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/Jce_b/writer.py` & `AndroidTools-0.1.1/Jce_b/writer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.1.0/setup.py` & `AndroidTools-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding='utf-8') as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="AndroidTools",
-    version="0.1.0",
+    version="0.1.1",
     author="1a",
     author_email="grayrail1x3@gmail.com",
     description="Android Tools for Python",
     long_description='Android Tools for Python',
     long_description_content_type="text/markdown",
     url="https://github.com/grayrail000/PyJce",
     packages=setuptools.find_packages(),
```

### Comparing `AndroidTools-0.1.0/test/test_Jce.py` & `AndroidTools-0.1.1/test/test_Jce.py`

 * *Files identical despite different names*

