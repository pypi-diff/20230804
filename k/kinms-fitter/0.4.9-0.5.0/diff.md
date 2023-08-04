# Comparing `tmp/kinms_fitter-0.4.9.tar.gz` & `tmp/kinms_fitter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinms_fitter-0.4.9.tar", last modified: Wed Jul 12 13:02:42 2023, max compression
+gzip compressed data, was "kinms_fitter-0.5.0.tar", last modified: Fri Aug  4 09:21:44 2023, max compression
```

## Comparing `kinms_fitter-0.4.9.tar` & `kinms_fitter-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.783744 kinms_fitter-0.4.9/
--rw-r--r--   0 tdavis     (503) staff       (20)        0 2021-01-07 12:48:31.000000 kinms_fitter-0.4.9/LICENSE
--rw-r--r--   0 tdavis     (503) staff       (20)      575 2023-07-12 13:02:42.783585 kinms_fitter-0.4.9/PKG-INFO
--rw-r--r--   0 tdavis     (503) staff       (20)        0 2022-08-24 14:57:04.000000 kinms_fitter-0.4.9/README.md
-drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.782609 kinms_fitter-0.4.9/kinms_fitter/
--rwxr--r--   0 tdavis     (503) staff       (20)      291 2022-08-24 14:32:42.000000 kinms_fitter-0.4.9/kinms_fitter/__init__.py
--rwxr--r--   0 tdavis     (503) staff       (20)     9679 2023-04-06 14:09:43.000000 kinms_fitter-0.4.9/kinms_fitter/diskThick_funcs.py
--rwxr--r--   0 tdavis     (503) staff       (20)    41273 2023-07-12 12:58:40.000000 kinms_fitter-0.4.9/kinms_fitter/kinms_fitter.py
--rwxr--r--   0 tdavis     (503) staff       (20)    40353 2023-03-08 15:55:21.000000 kinms_fitter-0.4.9/kinms_fitter/kinms_fitter_old.py
--rwxr--r--   0 tdavis     (503) staff       (20)     1680 2023-02-15 10:57:33.000000 kinms_fitter-0.4.9/kinms_fitter/prior_funcs.py
--rwxr--r--   0 tdavis     (503) staff       (20)    17861 2023-06-01 08:47:13.000000 kinms_fitter-0.4.9/kinms_fitter/sb_profs.py
--rw-r--r--   0 tdavis     (503) staff       (20)     2342 2023-02-21 14:38:07.000000 kinms_fitter-0.4.9/kinms_fitter/transformClouds.py
--rwxr--r--   0 tdavis     (503) staff       (20)    37043 2023-03-31 08:43:11.000000 kinms_fitter-0.4.9/kinms_fitter/velocity_profs.py
--rwxr--r--   0 tdavis     (503) staff       (20)     9608 2023-02-21 14:38:22.000000 kinms_fitter-0.4.9/kinms_fitter/warp_funcs.py
-drwxr-xr-x   0 tdavis     (503) staff       (20)        0 2023-07-12 13:02:42.783410 kinms_fitter-0.4.9/kinms_fitter.egg-info/
--rw-r--r--   0 tdavis     (503) staff       (20)      575 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (503) staff       (20)      498 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (503) staff       (20)        1 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (503) staff       (20)       82 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/requires.txt
--rw-r--r--   0 tdavis     (503) staff       (20)       13 2023-07-12 13:02:42.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (503) staff       (20)        0 2021-01-07 12:53:57.000000 kinms_fitter-0.4.9/kinms_fitter.egg-info/zip-safe
--rw-r--r--   0 tdavis     (503) staff       (20)       38 2023-07-12 13:02:42.783789 kinms_fitter-0.4.9/setup.cfg
--rw-r--r--   0 tdavis     (503) staff       (20)     1056 2023-07-12 12:58:53.000000 kinms_fitter-0.4.9/setup.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 09:21:44.358645 kinms_fitter-0.5.0/
+-rw-r--r--   0 tdavis     (501) staff       (20)    35149 2021-01-07 12:48:31.000000 kinms_fitter-0.5.0/LICENSE
+-rw-r--r--   0 tdavis     (501) staff       (20)     2079 2023-08-04 09:21:44.358477 kinms_fitter-0.5.0/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)     1530 2022-08-24 14:57:04.000000 kinms_fitter-0.5.0/README.md
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 09:21:44.357208 kinms_fitter-0.5.0/kinms_fitter/
+-rwxr--r--   0 tdavis     (501) staff       (20)      291 2022-08-24 14:32:42.000000 kinms_fitter-0.5.0/kinms_fitter/__init__.py
+-rwxr--r--   0 tdavis     (501) staff       (20)     9679 2023-04-06 14:09:43.000000 kinms_fitter-0.5.0/kinms_fitter/diskThick_funcs.py
+-rwxr--r--   0 tdavis     (501) staff       (20)    41273 2023-07-12 12:58:38.000000 kinms_fitter-0.5.0/kinms_fitter/kinms_fitter.py
+-rwxr--r--   0 tdavis     (501) staff       (20)    40353 2023-03-08 15:55:21.000000 kinms_fitter-0.5.0/kinms_fitter/kinms_fitter_old.py
+-rwxr--r--   0 tdavis     (501) staff       (20)     1680 2023-02-15 10:57:33.000000 kinms_fitter-0.5.0/kinms_fitter/prior_funcs.py
+-rwxr--r--   0 tdavis     (501) staff       (20)    17861 2023-06-01 08:47:13.000000 kinms_fitter-0.5.0/kinms_fitter/sb_profs.py
+-rw-r--r--   0 tdavis     (501) staff       (20)     2342 2023-02-21 14:38:07.000000 kinms_fitter-0.5.0/kinms_fitter/transformClouds.py
+-rwxr--r--   0 tdavis     (501) staff       (20)    37043 2023-03-31 08:43:11.000000 kinms_fitter-0.5.0/kinms_fitter/velocity_profs.py
+-rwxr--r--   0 tdavis     (501) staff       (20)     9608 2023-02-21 14:38:22.000000 kinms_fitter-0.5.0/kinms_fitter/warp_funcs.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-08-04 09:21:44.358104 kinms_fitter-0.5.0/kinms_fitter.egg-info/
+-rw-r--r--   0 tdavis     (501) staff       (20)     2079 2023-08-04 09:21:44.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)      498 2023-08-04 09:21:44.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-08-04 09:21:44.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       82 2023-08-04 09:21:44.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       13 2023-08-04 09:21:44.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2021-01-07 12:53:57.000000 kinms_fitter-0.5.0/kinms_fitter.egg-info/zip-safe
+-rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-08-04 09:21:44.358690 kinms_fitter-0.5.0/setup.cfg
+-rw-r--r--   0 tdavis     (501) staff       (20)     1056 2023-08-04 09:21:07.000000 kinms_fitter-0.5.0/setup.py
```

### Comparing `kinms_fitter-0.4.9/kinms_fitter/diskThick_funcs.py` & `kinms_fitter-0.5.0/kinms_fitter/diskThick_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/kinms_fitter.py` & `kinms_fitter-0.5.0/kinms_fitter/kinms_fitter.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/kinms_fitter_old.py` & `kinms_fitter-0.5.0/kinms_fitter/kinms_fitter_old.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/prior_funcs.py` & `kinms_fitter-0.5.0/kinms_fitter/prior_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/sb_profs.py` & `kinms_fitter-0.5.0/kinms_fitter/sb_profs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/transformClouds.py` & `kinms_fitter-0.5.0/kinms_fitter/transformClouds.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/velocity_profs.py` & `kinms_fitter-0.5.0/kinms_fitter/velocity_profs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/kinms_fitter/warp_funcs.py` & `kinms_fitter-0.5.0/kinms_fitter/warp_funcs.py`

 * *Files identical despite different names*

### Comparing `kinms_fitter-0.4.9/setup.py` & `kinms_fitter-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='kinms_fitter',
-       version='0.4.9',
+       version='0.5.0',
        description='Wrapper for KinMSpy that automates most common galaxy fitting tasks',
        url='https://github.com/TimothyADavis/KinMS_fitter',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='GNU GPLv3',
```

