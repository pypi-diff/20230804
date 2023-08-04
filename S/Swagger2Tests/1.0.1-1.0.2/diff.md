# Comparing `tmp/Swagger2Tests-1.0.1.tar.gz` & `tmp/Swagger2Tests-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Swagger2Tests-1.0.1.tar", last modified: Fri Aug  4 09:17:40 2023, max compression
+gzip compressed data, was "Swagger2Tests-1.0.2.tar", last modified: Fri Aug  4 09:38:14 2023, max compression
```

## Comparing `Swagger2Tests-1.0.1.tar` & `Swagger2Tests-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:17:40.450856 Swagger2Tests-1.0.1/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 09:17:40.450389 Swagger2Tests-1.0.1/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:17:40.446651 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       56 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       10 2023-08-04 09:17:40.000000 Swagger2Tests-1.0.1/Swagger2Tests.egg-info/top_level.txt
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:17:40.448478 Swagger2Tests-1.0.1/constants/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.1/constants/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      190 2023-08-04 07:32:20.000000 Swagger2Tests-1.0.1/constants/base_constants.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 09:17:40.451101 Swagger2Tests-1.0.1/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      878 2023-08-04 09:11:24.000000 Swagger2Tests-1.0.1/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:38:14.446445 Swagger2Tests-1.0.2/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 09:38:14.445997 Swagger2Tests-1.0.2/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:38:14.438337 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      282 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       52 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       10 2023-08-04 09:38:14.000000 Swagger2Tests-1.0.2/Swagger2Tests.egg-info/top_level.txt
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:38:14.439456 Swagger2Tests-1.0.2/constants/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.2/constants/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      190 2023-08-04 07:32:20.000000 Swagger2Tests-1.0.2/constants/base_constants.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 09:38:14.446615 Swagger2Tests-1.0.2/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      874 2023-08-04 09:38:09.000000 Swagger2Tests-1.0.2/setup.py
```

### Comparing `Swagger2Tests-1.0.1/PKG-INFO` & `Swagger2Tests-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.1
+Version: 1.0.2
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.1/Swagger2Tests.egg-info/PKG-INFO` & `Swagger2Tests-1.0.2/Swagger2Tests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.1
+Version: 1.0.2
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.1/setup.py` & `Swagger2Tests-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 readmepath = '../README.md'
 setup(
     name='Swagger2Tests',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'Swagger2Tests = src.loadswagger:main'
+            'Swagger2Tests = loadswagger:main'
         ]
     },
     install_requires=[
         'argparse','jinja2','pytest','requests','coloredlogs','Faker'
     ],
     author='visonforcoding',
     author_email='visonforcoding@gmail.com',
```

