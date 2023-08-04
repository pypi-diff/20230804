# Comparing `tmp/neco_f-0.0.3.tar.gz` & `tmp/neco_f-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_f-0.0.3.tar", last modified: Fri Aug  4 07:40:47 2023, max compression
+gzip compressed data, was "neco_f-0.0.4.tar", last modified: Fri Aug  4 07:58:09 2023, max compression
```

## Comparing `neco_f-0.0.3.tar` & `neco_f-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 07:40:47.033199 neco_f-0.0.3/
--rw-rw-rw-   0        0        0      417 2023-08-04 07:40:47.033199 neco_f-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-08-04 06:26:40.000000 neco_f-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 07:40:47.032200 neco_f-0.0.3/neco_f.egg-info/
--rw-rw-rw-   0        0        0      417 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 07:40:46.000000 neco_f-0.0.3/neco_f.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 07:40:47.034199 neco_f-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-08-04 07:40:14.000000 neco_f-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:09.002982 neco_f-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 neco_f-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      600 2023-08-04 07:58:09.001982 neco_f-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-08-04 07:56:05.000000 neco_f-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:09.000982 neco_f-0.0.4/neco_f.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-08-04 07:58:08.000000 neco_f-0.0.4/neco_f.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-08-04 07:58:08.000000 neco_f-0.0.4/neco_f.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:58:08.000000 neco_f-0.0.4/neco_f.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-04 07:58:08.000000 neco_f-0.0.4/neco_f.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:58:08.000000 neco_f-0.0.4/neco_f.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:58:09.002982 neco_f-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-08-04 07:57:59.000000 neco_f-0.0.4/setup.py
```

### Comparing `neco_f-0.0.3/setup.py` & `neco_f-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='neco_f',
-    version='0.0.3',
+    version='0.0.4',
     author='neco_arc',
     author_email='3306601284@qq.com',
-    description='A simple Python library',
+    description='一个鱼龙混杂的库',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/johndoe/my_library',
+    url='https://github.com/sweetnotice/neco_f',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
```

