# Comparing `tmp/aityz-1.0.3.tar.gz` & `tmp/aityz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aityz-1.0.3.tar", last modified: Sat Jul 29 04:17:21 2023, max compression
+gzip compressed data, was "aityz-1.1.0.tar", last modified: Fri Aug  4 10:59:30 2023, max compression
```

## Comparing `aityz-1.0.3.tar` & `aityz-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.873250 aityz-1.0.3/
--rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      447 2023-07-29 04:17:21.869997 aityz-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.837611 aityz-1.0.3/aityz/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.3/aityz/__init__.py
--rw-rw-rw-   0        0        0     8062 2023-07-29 04:17:04.000000 aityz-1.0.3/aityz/encryption.py
--rw-rw-rw-   0        0        0      908 2023-07-27 23:50:25.000000 aityz-1.0.3/aityz/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:17:21.865808 aityz-1.0.3/aityz.egg-info/
--rw-rw-rw-   0        0        0      447 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-29 04:17:21.000000 aityz-1.0.3/aityz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 04:17:21.873250 aityz-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      604 2023-07-29 04:17:20.000000 aityz-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:59:30.523670 aityz-1.1.0/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      447 2023-08-04 10:59:30.520984 aityz-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 10:59:30.490035 aityz-1.1.0/aityz/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.1.0/aityz/__init__.py
+-rw-rw-rw-   0        0        0     8062 2023-07-29 04:17:04.000000 aityz-1.1.0/aityz/encryption.py
+-rw-rw-rw-   0        0        0      908 2023-07-27 23:50:25.000000 aityz-1.1.0/aityz/exceptions.py
+-rw-rw-rw-   0        0        0     9596 2023-08-04 10:58:53.000000 aityz-1.1.0/aityz/nlp.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:59:30.514022 aityz-1.1.0/aityz.egg-info/
+-rw-rw-rw-   0        0        0      447 2023-08-04 10:59:30.000000 aityz-1.1.0/aityz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-08-04 10:59:30.000000 aityz-1.1.0/aityz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 10:59:30.000000 aityz-1.1.0/aityz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-04 10:59:30.000000 aityz-1.1.0/aityz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 10:59:30.000000 aityz-1.1.0/aityz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 10:59:30.523670 aityz-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-08-04 10:59:27.000000 aityz-1.1.0/setup.py
```

### Comparing `aityz-1.0.3/LICENSE` & `aityz-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aityz-1.0.3/aityz/encryption.py` & `aityz-1.1.0/aityz/encryption.py`

 * *Files identical despite different names*

### Comparing `aityz-1.0.3/aityz/exceptions.py` & `aityz-1.1.0/aityz/exceptions.py`

 * *Files identical despite different names*

### Comparing `aityz-1.0.3/pyproject.toml` & `aityz-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aityz-1.0.3/setup.py` & `aityz-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aityz',
-    version='1.0.3',
+    version='1.1.0',
     packages=find_packages(),
     install_requires=[
         'rsa',
-        'pycryptodome'
+        'torch',
+        'pycryptodome',
+        'transformers',
+        'accelerate'
     ],
     author='Aityz',
     author_email='itzaityz@gmail.com',
     description='The multipurpose package, built for programmers',
     long_description='Aityz Library is a multipurpose library made for many different use cases for Python. From '
                      'Machine Learning to Encryption, it has simplified many different ways of using Python.',
     url='https://github.com/Aityz/Library',
```

