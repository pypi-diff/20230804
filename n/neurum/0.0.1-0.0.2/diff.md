# Comparing `tmp/neurum-0.0.1.tar.gz` & `tmp/neurum-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurum-0.0.1.tar", last modified: Mon Jul 31 20:24:11 2023, max compression
+gzip compressed data, was "neurum-0.0.2.tar", last modified: Fri Aug  4 12:25:04 2023, max compression
```

## Comparing `neurum-0.0.1.tar` & `neurum-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vanshshah   (501) staff       (20)        0 2023-07-31 20:24:11.113839 neurum-0.0.1/
--rw-r--r--   0 vanshshah   (501) staff       (20)       79 2023-07-31 20:06:10.000000 neurum-0.0.1/CHANGELOG.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)     1057 2023-07-31 19:13:01.000000 neurum-0.0.1/LICENSE.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)       26 2023-07-31 19:12:59.000000 neurum-0.0.1/MANIFEST.in
--rw-r--r--   0 vanshshah   (501) staff       (20)      564 2023-07-31 20:24:11.113737 neurum-0.0.1/PKG-INFO
--rw-r--r--   0 vanshshah   (501) staff       (20)       53 2023-07-31 19:08:55.000000 neurum-0.0.1/README.txt
-drwxr-xr-x   0 vanshshah   (501) staff       (20)        0 2023-07-31 20:24:11.113593 neurum-0.0.1/neurum.egg-info/
--rw-r--r--   0 vanshshah   (501) staff       (20)      564 2023-07-31 20:24:11.000000 neurum-0.0.1/neurum.egg-info/PKG-INFO
--rw-r--r--   0 vanshshah   (501) staff       (20)      224 2023-07-31 20:24:11.000000 neurum-0.0.1/neurum.egg-info/SOURCES.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)        1 2023-07-31 20:24:11.000000 neurum-0.0.1/neurum.egg-info/dependency_links.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)       26 2023-07-31 20:24:11.000000 neurum-0.0.1/neurum.egg-info/requires.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)        1 2023-07-31 20:24:11.000000 neurum-0.0.1/neurum.egg-info/top_level.txt
--rw-r--r--   0 vanshshah   (501) staff       (20)      778 2023-07-31 18:58:18.000000 neurum-0.0.1/neurum.py
--rw-r--r--   0 vanshshah   (501) staff       (20)       38 2023-07-31 20:24:11.113870 neurum-0.0.1/setup.cfg
--rw-r--r--   0 vanshshah   (501) staff       (20)      798 2023-07-31 20:23:37.000000 neurum-0.0.1/setup.py
--rw-r--r--   0 vanshshah   (501) staff       (20)       48 2023-07-31 19:07:01.000000 neurum-0.0.1/test.py
+drwxr-xr-x   0 vanshshah   (501) staff       (20)        0 2023-08-04 12:25:04.796548 neurum-0.0.2/
+-rw-r--r--   0 vanshshah   (501) staff       (20)       79 2023-07-31 20:06:10.000000 neurum-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)     1057 2023-07-31 19:13:01.000000 neurum-0.0.2/LICENSE.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)       26 2023-07-31 19:12:59.000000 neurum-0.0.2/MANIFEST.in
+-rw-r--r--   0 vanshshah   (501) staff       (20)      564 2023-08-04 12:25:04.796438 neurum-0.0.2/PKG-INFO
+-rw-r--r--   0 vanshshah   (501) staff       (20)       53 2023-07-31 19:08:55.000000 neurum-0.0.2/README.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)       13 2023-08-03 14:21:11.000000 neurum-0.0.2/__init__.py
+drwxr-xr-x   0 vanshshah   (501) staff       (20)        0 2023-08-04 12:25:04.796288 neurum-0.0.2/neurum.egg-info/
+-rw-r--r--   0 vanshshah   (501) staff       (20)      564 2023-08-04 12:25:04.000000 neurum-0.0.2/neurum.egg-info/PKG-INFO
+-rw-r--r--   0 vanshshah   (501) staff       (20)      226 2023-08-04 12:25:04.000000 neurum-0.0.2/neurum.egg-info/SOURCES.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)        1 2023-08-04 12:25:04.000000 neurum-0.0.2/neurum.egg-info/dependency_links.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)       26 2023-08-04 12:25:04.000000 neurum-0.0.2/neurum.egg-info/requires.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)        1 2023-08-04 12:25:04.000000 neurum-0.0.2/neurum.egg-info/top_level.txt
+-rw-r--r--   0 vanshshah   (501) staff       (20)       38 2023-08-04 12:25:04.796583 neurum-0.0.2/setup.cfg
+-rw-r--r--   0 vanshshah   (501) staff       (20)      798 2023-08-04 12:22:51.000000 neurum-0.0.2/setup.py
+-rw-r--r--   0 vanshshah   (501) staff       (20)       48 2023-07-31 19:07:01.000000 neurum-0.0.2/test.py
```

### Comparing `neurum-0.0.1/LICENSE.txt` & `neurum-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurum-0.0.1/PKG-INFO` & `neurum-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurum
-Version: 0.0.1
+Version: 0.0.2
 Summary: A powerful multimodal AI sdk for python by Neurum Inc..
 Home-page: 
 Author: Vansh Shah
 Author-email: vanshshah836@gmail.com
 Keywords: ai api sdk llm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `neurum-0.0.1/neurum.egg-info/PKG-INFO` & `neurum-0.0.2/neurum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurum
-Version: 0.0.1
+Version: 0.0.2
 Summary: A powerful multimodal AI sdk for python by Neurum Inc..
 Home-page: 
 Author: Vansh Shah
 Author-email: vanshshah836@gmail.com
 Keywords: ai api sdk llm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `neurum-0.0.1/setup.py` & `neurum-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                'Operating System :: Unix',  
                'License :: OSI Approved :: MIT License', 
                'Programming Language :: Python :: 3',]
 
 
 setup(
     name= 'neurum', 
-    version='0.0.1',
+    version='0.0.2',
     description='A powerful multimodal AI sdk for python by Neurum Inc..',
     url='',
     author='Vansh Shah', 
     author_email='vanshshah836@gmail.com',
     License='MIT', 
     classifiers=classifiers, 
     keywords='ai api sdk llm',
```

