# Comparing `tmp/Swagger2Tests-1.0.4.tar.gz` & `tmp/Swagger2Tests-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Swagger2Tests-1.0.4.tar", last modified: Fri Aug  4 10:34:20 2023, max compression
+gzip compressed data, was "Swagger2Tests-1.0.5.tar", last modified: Fri Aug  4 10:36:35 2023, max compression
```

## Comparing `Swagger2Tests-1.0.4.tar` & `Swagger2Tests-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:34:20.413256 Swagger2Tests-1.0.4/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:34:20.412745 Swagger2Tests-1.0.4/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:34:20.405870 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      346 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       56 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        4 2023-08-04 10:34:20.000000 Swagger2Tests-1.0.4/Swagger2Tests.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 10:34:20.413496 Swagger2Tests-1.0.4/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      895 2023-08-04 10:34:07.000000 Swagger2Tests-1.0.4/setup.py
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:34:20.409146 Swagger2Tests-1.0.4/src/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     6617 2023-08-04 06:38:23.000000 Swagger2Tests-1.0.4/src/Swagger2Tests.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:27:37.000000 Swagger2Tests-1.0.4/src/__init__.py
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:34:20.411772 Swagger2Tests-1.0.4/src/constants/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.4/src/constants/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      190 2023-08-04 07:32:20.000000 Swagger2Tests-1.0.4/src/constants/base_constants.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3246 2023-08-04 07:59:02.000000 Swagger2Tests-1.0.4/src/loadswagger.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:36:35.420230 Swagger2Tests-1.0.5/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:36:35.419552 Swagger2Tests-1.0.5/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:36:35.409535 Swagger2Tests-1.0.5/Swagger2Tests/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     6617 2023-08-04 06:38:23.000000 Swagger2Tests-1.0.5/Swagger2Tests/Swagger2Tests.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:27:37.000000 Swagger2Tests-1.0.5/Swagger2Tests/__init__.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:36:35.417822 Swagger2Tests-1.0.5/Swagger2Tests/constants/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.5/Swagger2Tests/constants/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      190 2023-08-04 07:32:20.000000 Swagger2Tests-1.0.5/Swagger2Tests/constants/base_constants.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3246 2023-08-04 07:59:02.000000 Swagger2Tests-1.0.5/Swagger2Tests/loadswagger.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:36:35.416364 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      396 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       66 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       14 2023-08-04 10:36:35.000000 Swagger2Tests-1.0.5/Swagger2Tests.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 10:36:35.420494 Swagger2Tests-1.0.5/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      905 2023-08-04 10:36:31.000000 Swagger2Tests-1.0.5/setup.py
```

### Comparing `Swagger2Tests-1.0.4/PKG-INFO` & `Swagger2Tests-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.4
+Version: 1.0.5
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.4/Swagger2Tests.egg-info/PKG-INFO` & `Swagger2Tests-1.0.5/Swagger2Tests.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.4
+Version: 1.0.5
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.4/setup.py` & `Swagger2Tests-1.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 readmepath = 'README.md'
 setup(
     name='Swagger2Tests',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'Swagger2Tests = src.loadswagger:main'
+            'Swagger2Tests = Swagger2Tests.loadswagger:main'
         ]
     },
     install_requires=[
         'argparse','jinja2','pytest','requests','coloredlogs','Faker'
     ],
     author='visonforcoding',
     author_email='visonforcoding@gmail.com',
```

### Comparing `Swagger2Tests-1.0.4/src/Swagger2Tests.py` & `Swagger2Tests-1.0.5/Swagger2Tests/Swagger2Tests.py`

 * *Files identical despite different names*

### Comparing `Swagger2Tests-1.0.4/src/loadswagger.py` & `Swagger2Tests-1.0.5/Swagger2Tests/loadswagger.py`

 * *Files identical despite different names*

