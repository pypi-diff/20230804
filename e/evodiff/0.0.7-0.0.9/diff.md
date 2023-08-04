# Comparing `tmp/evodiff-0.0.7.tar.gz` & `tmp/evodiff-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodiff-0.0.7.tar", last modified: Fri Aug  4 17:29:38 2023, max compression
+gzip compressed data, was "evodiff-0.0.9.tar", last modified: Fri Aug  4 17:53:37 2023, max compression
```

## Comparing `evodiff-0.0.7.tar` & `evodiff-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:29:38.118209 evodiff-0.0.7/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.7/LICENSE
--rw-r--r--   0 nityathakkar   (501) staff       (20)       16 2023-08-04 17:18:36.000000 evodiff-0.0.7/MANIFEST.in
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:29:38.117811 evodiff-0.0.7/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.7/README.md
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:29:38.040587 evodiff-0.0.7/config/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.7/config/config38M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.7/config/config640M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.7/config/configMSA-600M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.7/config/configMSA.json
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:29:38.051204 evodiff-0.0.7/evodiff/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/__init__.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.7/evodiff/collaters.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/constants.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/data.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/losses.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/metrics.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/model.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.7/evodiff/plot.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    11990 2023-08-04 17:24:45.000000 evodiff-0.0.7/evodiff/pretrained.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.7/evodiff/utils.py
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:29:38.117280 evodiff-0.0.7/evodiff.egg-info/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:29:37.000000 evodiff-0.0.7/evodiff.egg-info/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-04 17:29:37.000000 evodiff-0.0.7/evodiff.egg-info/SOURCES.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-04 17:29:37.000000 evodiff-0.0.7/evodiff.egg-info/dependency_links.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-04 17:29:37.000000 evodiff-0.0.7/evodiff.egg-info/top_level.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-04 17:29:02.000000 evodiff-0.0.7/pyproject.toml
--rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-04 17:29:38.118317 evodiff-0.0.7/setup.cfg
--rw-r--r--   0 nityathakkar   (501) staff       (20)      801 2023-08-04 17:29:05.000000 evodiff-0.0.7/setup.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:53:37.673694 evodiff-0.0.9/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.9/LICENSE
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       15 2023-08-04 17:32:09.000000 evodiff-0.0.9/MANIFEST.in
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:53:37.673092 evodiff-0.0.9/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.9/README.md
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:53:37.621651 evodiff-0.0.9/config/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.9/config/config38M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.9/config/config640M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.9/config/configMSA-600M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.9/config/configMSA.json
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:53:37.647800 evodiff-0.0.9/evodiff/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/__init__.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.9/evodiff/collaters.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/constants.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/data.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/losses.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/metrics.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/model.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.9/evodiff/plot.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    11990 2023-08-04 17:24:45.000000 evodiff-0.0.9/evodiff/pretrained.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.9/evodiff/utils.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:53:37.671581 evodiff-0.0.9/evodiff.egg-info/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:53:37.000000 evodiff-0.0.9/evodiff.egg-info/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-04 17:53:37.000000 evodiff-0.0.9/evodiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-04 17:53:37.000000 evodiff-0.0.9/evodiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-04 17:53:37.000000 evodiff-0.0.9/evodiff.egg-info/top_level.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-04 17:50:04.000000 evodiff-0.0.9/pyproject.toml
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-04 17:53:37.673864 evodiff-0.0.9/setup.cfg
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      931 2023-08-04 17:53:16.000000 evodiff-0.0.9/setup.py
```

### Comparing `evodiff-0.0.7/LICENSE` & `evodiff-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/PKG-INFO` & `evodiff-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
```

### Comparing `evodiff-0.0.7/README.md` & `evodiff-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/collaters.py` & `evodiff-0.0.9/evodiff/collaters.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/data.py` & `evodiff-0.0.9/evodiff/data.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/losses.py` & `evodiff-0.0.9/evodiff/losses.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/metrics.py` & `evodiff-0.0.9/evodiff/metrics.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/model.py` & `evodiff-0.0.9/evodiff/model.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/plot.py` & `evodiff-0.0.9/evodiff/plot.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/pretrained.py` & `evodiff-0.0.9/evodiff/pretrained.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff/utils.py` & `evodiff-0.0.9/evodiff/utils.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.7/evodiff.egg-info/PKG-INFO` & `evodiff-0.0.9/evodiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
```

