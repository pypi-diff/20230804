# Comparing `tmp/neco_f-0.0.1.tar.gz` & `tmp/neco_f-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_f-0.0.1.tar", last modified: Fri Aug  4 07:11:48 2023, max compression
+gzip compressed data, was "neco_f-0.0.3.tar", last modified: Fri Aug  4 07:40:47 2023, max compression
```

## Comparing `neco_f-0.0.1.tar` & `neco_f-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 07:11:48.801534 neco_f-0.0.1/
--rw-rw-rw-   0        0        0      415 2023-08-04 07:11:48.800558 neco_f-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-08-04 06:26:40.000000 neco_f-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 07:11:48.799581 neco_f-0.0.1/neco_f.egg-info/
--rw-rw-rw-   0        0        0      415 2023-08-04 07:11:48.000000 neco_f-0.0.1/neco_f.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-08-04 07:11:48.000000 neco_f-0.0.1/neco_f.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 07:11:48.000000 neco_f-0.0.1/neco_f.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-08-04 07:11:48.000000 neco_f-0.0.1/neco_f.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 07:11:48.000000 neco_f-0.0.1/neco_f.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 07:11:48.801534 neco_f-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-08-04 07:10:04.000000 neco_f-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:40:47.033199 neco_f-0.0.3/
+-rw-rw-rw-   0        0        0      417 2023-08-04 07:40:47.033199 neco_f-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-08-04 06:26:40.000000 neco_f-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 07:40:47.032200 neco_f-0.0.3/neco_f.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:40:47.034199 neco_f-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2023-08-04 07:40:14.000000 neco_f-0.0.3/setup.py
```

### Comparing `neco_f-0.0.1/setup.py` & `neco_f-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
+with open('README.md', mode='r', encoding='utf-8') as f:
+    long_description = f.read()
 setup(
     name='neco_f',
-    version='0.0.1',
+    version='0.0.3',
     author='neco_arc',
     author_email='3306601284@qq.com',
     description='A simple Python library',
-    long_description='README.md',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/johndoe/my_library',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

