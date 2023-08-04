# Comparing `tmp/complex_mathematics-0.1.1.tar.gz` & `tmp/complex_mathematics-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_mathematics-0.1.1.tar", last modified: Fri Aug  4 16:22:37 2023, max compression
+gzip compressed data, was "complex_mathematics-1.1.1.tar", last modified: Fri Aug  4 18:06:59 2023, max compression
```

## Comparing `complex_mathematics-0.1.1.tar` & `complex_mathematics-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.776728 complex_mathematics-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      398 2023-08-04 16:22:37.775732 complex_mathematics-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.759774 complex_mathematics-0.1.1/complex_mathematics/
--rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-0.1.1/complex_mathematics/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-0.1.1/complex_mathematics/linalg.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.773738 complex_mathematics-0.1.1/complex_mathematics.egg-info/
--rw-rw-rw-   0        0        0      398 2023-08-04 16:22:37.000000 complex_mathematics-0.1.1/complex_mathematics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-08-04 16:22:37.000000 complex_mathematics-0.1.1/complex_mathematics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:22:37.000000 complex_mathematics-0.1.1/complex_mathematics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 16:22:37.000000 complex_mathematics-0.1.1/complex_mathematics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 16:22:37.000000 complex_mathematics-0.1.1/complex_mathematics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 16:22:37.776728 complex_mathematics-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-04 16:21:55.000000 complex_mathematics-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:06:59.325318 complex_mathematics-1.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      398 2023-08-04 18:06:59.324319 complex_mathematics-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 18:06:59.303375 complex_mathematics-1.1.1/complex_mathematics/
+-rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-1.1.1/complex_mathematics/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-1.1.1/complex_mathematics/linalg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:06:59.322326 complex_mathematics-1.1.1/complex_mathematics.egg-info/
+-rw-rw-rw-   0        0        0      398 2023-08-04 18:06:59.000000 complex_mathematics-1.1.1/complex_mathematics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-08-04 18:06:59.000000 complex_mathematics-1.1.1/complex_mathematics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 18:06:59.000000 complex_mathematics-1.1.1/complex_mathematics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 18:06:59.000000 complex_mathematics-1.1.1/complex_mathematics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 18:06:59.000000 complex_mathematics-1.1.1/complex_mathematics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 18:06:59.325318 complex_mathematics-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-04 18:06:36.000000 complex_mathematics-1.1.1/setup.py
```

### Comparing `complex_mathematics-0.1.1/LICENSE` & `complex_mathematics-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `complex_mathematics-0.1.1/complex_mathematics/__init__.py` & `complex_mathematics-1.1.1/complex_mathematics/__init__.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-0.1.1/complex_mathematics/linalg.py` & `complex_mathematics-1.1.1/complex_mathematics/linalg.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-0.1.1/setup.py` & `complex_mathematics-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='complex_mathematics',
-    version='0.1.1',
+    version='1.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy', 'scipy'
     ],
     license='MIT',
     author="Arnav Malhotra",
     author_email="emumalhotra@gmail.com",
```

