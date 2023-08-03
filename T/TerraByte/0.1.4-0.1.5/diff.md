# Comparing `tmp/TerraByte-0.1.4.tar.gz` & `tmp/TerraByte-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraByte-0.1.4.tar", last modified: Mon Jul 10 10:53:45 2023, max compression
+gzip compressed data, was "TerraByte-0.1.5.tar", last modified: Thu Aug  3 23:29:01 2023, max compression
```

## Comparing `TerraByte-0.1.4.tar` & `TerraByte-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:53:45.560566 TerraByte-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 10:53:36.000000 TerraByte-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-10 10:53:45.560566 TerraByte-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-10 10:53:36.000000 TerraByte-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:53:45.556566 TerraByte-0.1.4/TerraByte/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 10:53:36.000000 TerraByte-0.1.4/TerraByte/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:53:45.560566 TerraByte-0.1.4/TerraByte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-10 10:53:45.000000 TerraByte-0.1.4/TerraByte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-10 10:53:45.000000 TerraByte-0.1.4/TerraByte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:53:45.000000 TerraByte-0.1.4/TerraByte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 10:53:45.000000 TerraByte-0.1.4/TerraByte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 10:53:45.000000 TerraByte-0.1.4/TerraByte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:53:45.560566 TerraByte-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-10 10:53:36.000000 TerraByte-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 23:28:52.000000 TerraByte-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-03 23:29:01.656201 TerraByte-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-08-03 23:28:52.000000 TerraByte-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/TerraByte/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/TerraByte/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/flash2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24433 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/multimodal_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model/terrabyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/TerraByte/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23403 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/TerraByte/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-03 23:28:52.000000 TerraByte-0.1.5/TerraByte/utils/stable_adamw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:29:01.656201 TerraByte-0.1.5/TerraByte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-03 23:29:01.000000 TerraByte-0.1.5/TerraByte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-03 23:29:01.000000 TerraByte-0.1.5/TerraByte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:29:01.000000 TerraByte-0.1.5/TerraByte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 23:29:01.000000 TerraByte-0.1.5/TerraByte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 23:29:01.000000 TerraByte-0.1.5/TerraByte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:29:01.656201 TerraByte-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-03 23:28:52.000000 TerraByte-0.1.5/setup.py
```

### Comparing `TerraByte-0.1.4/LICENSE` & `TerraByte-0.1.5/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Phil Wang
+Copyright (c) Kye Gomez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `TerraByte-0.1.4/PKG-INFO` & `TerraByte-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraByte
-Version: 0.1.4
+Version: 0.1.5
 Summary: TerraByte - Pytorch
 Home-page: https://github.com/kyegomez/TerraByte
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TerraByte-0.1.4/README.md` & `TerraByte-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,12 @@
     year      = {2021},
     publisher = {Zenodo},
     version   = {0.01},
     doi       = {10.5281/zenodo.5196578},
     url       = {https://doi.org/10.5281/zenodo.5196578}
 }
 ```
+
+
+# Todo:
+
+* Implement Optimus prime stacked attention with flash attention 2.0
```

#### html2text {}

```diff
@@ -33,8 +33,9 @@
 Processing Systems}, year = {2022} } ``` ```bibtex @misc{press2021ALiBi, title
 = {Train Short, Test Long: Attention with Linear Biases Enable Input Length
 Extrapolation}, author = {Ofir Press and Noah A. Smith and Mike Lewis}, year =
 {2021}, url = {https://ofir.io/train_short_test_long.pdf} } ``` ```bibtex
 @software{peng_bo_2021_5196578, author = {PENG Bo}, title = {BlinkDL/RWKV-LM:
 0.01}, month = {aug}, year = {2021}, publisher = {Zenodo}, version = {0.01},
 doi = {10.5281/zenodo.5196578}, url = {https://doi.org/10.5281/zenodo.5196578}
-} ```
+} ``` # Todo: * Implement Optimus prime stacked attention with flash attention
+2.0
```

### Comparing `TerraByte-0.1.4/TerraByte.egg-info/PKG-INFO` & `TerraByte-0.1.5/TerraByte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraByte
-Version: 0.1.4
+Version: 0.1.5
 Summary: TerraByte - Pytorch
 Home-page: https://github.com/kyegomez/TerraByte
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TerraByte-0.1.4/setup.py` & `TerraByte-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'TerraByte',
   packages = find_packages(),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'TerraByte - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/TerraByte',
   keywords = [
```

