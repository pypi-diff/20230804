# Comparing `tmp/s1282003_learn-2023.8.4.tar.gz` & `tmp/s1282003_learn-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s1282003_learn-2023.8.4.tar", last modified: Fri Aug  4 06:46:17 2023, max compression
+gzip compressed data, was "s1282003_learn-2023.8.5.tar", last modified: Fri Aug  4 06:52:25 2023, max compression
```

## Comparing `s1282003_learn-2023.8.4.tar` & `s1282003_learn-2023.8.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/
--rw-r--r--   0 s1282003 (18588) uday      (1000)    35823 2023-08-04 06:01:52.000000 s1282003_learn-2023.8.4/LICENSE
--rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/PKG-INFO
--rw-r--r--   0 s1282003 (18588) uday      (1000)       16 2023-08-04 06:01:51.000000 s1282003_learn-2023.8.4/README.md
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/s1282003_learn/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:15.000000 s1282003_learn-2023.8.4/s1282003_learn/__init__.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/s1282003_learn/statistics/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.4/s1282003_learn/statistics/__init__.py
--rw-r--r--   0 s1282003 (18588) uday      (1000)     2284 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.4/s1282003_learn/statistics/frequenciesOfItems.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/s1282003_learn/visualization/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:33.000000 s1282003_learn-2023.8.4/s1282003_learn/visualization/__init__.py
--rw-r--r--   0 s1282003 (18588) uday      (1000)     4754 2023-08-04 06:46:00.000000 s1282003_learn-2023.8.4/s1282003_learn/visualization/heatMapItemsFrequencies.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/s1282003_learn.egg-info/
--rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:46:17.000000 s1282003_learn-2023.8.4/s1282003_learn.egg-info/PKG-INFO
--rw-r--r--   0 s1282003 (18588) uday      (1000)      425 2023-08-04 06:46:17.000000 s1282003_learn-2023.8.4/s1282003_learn.egg-info/SOURCES.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)        1 2023-08-04 06:46:17.000000 s1282003_learn-2023.8.4/s1282003_learn.egg-info/dependency_links.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)      194 2023-08-04 06:46:17.000000 s1282003_learn-2023.8.4/s1282003_learn.egg-info/requires.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)       15 2023-08-04 06:46:17.000000 s1282003_learn-2023.8.4/s1282003_learn.egg-info/top_level.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)       38 2023-08-04 06:46:17.034265 s1282003_learn-2023.8.4/setup.cfg
--rw-r--r--   0 s1282003 (18588) uday      (1000)     1302 2023-08-04 06:45:40.000000 s1282003_learn-2023.8.4/setup.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)    35823 2023-08-04 06:01:52.000000 s1282003_learn-2023.8.5/LICENSE
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/PKG-INFO
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       16 2023-08-04 06:01:51.000000 s1282003_learn-2023.8.5/README.md
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:15.000000 s1282003_learn-2023.8.5/s1282003_learn/__init__.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/statistics/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5/s1282003_learn/statistics/__init__.py
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     2284 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5/s1282003_learn/statistics/frequenciesOfItems.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/visualization/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:33.000000 s1282003_learn-2023.8.5/s1282003_learn/visualization/__init__.py
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     4754 2023-08-04 06:46:00.000000 s1282003_learn-2023.8.5/s1282003_learn/visualization/heatMapItemsFrequencies.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn.egg-info/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/PKG-INFO
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      425 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        1 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      194 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/requires.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       15 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/top_level.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       38 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/setup.cfg
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     1302 2023-08-04 06:51:45.000000 s1282003_learn-2023.8.5/setup.py
```

### Comparing `s1282003_learn-2023.8.4/LICENSE` & `s1282003_learn-2023.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s1282003_learn-2023.8.4/PKG-INFO` & `s1282003_learn-2023.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s1282003_learn
-Version: 2023.8.4
+Version: 2023.8.5
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/angelitagozaly/s1282003_learn
 Author: Angelita Gozaly
 Author-email: s1282003@u-aizu.ac.jp
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s1282003_learn-2023.8.4/s1282003_learn/statistics/frequenciesOfItems.py` & `s1282003_learn-2023.8.5/s1282003_learn/statistics/frequenciesOfItems.py`

 * *Files identical despite different names*

### Comparing `s1282003_learn-2023.8.4/s1282003_learn/visualization/heatMapItemsFrequencies.py` & `s1282003_learn-2023.8.5/s1282003_learn/visualization/heatMapItemsFrequencies.py`

 * *Files identical despite different names*

### Comparing `s1282003_learn-2023.8.4/s1282003_learn.egg-info/PKG-INFO` & `s1282003_learn-2023.8.5/s1282003_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s1282003-learn
-Version: 2023.8.4
+Version: 2023.8.5
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/angelitagozaly/s1282003_learn
 Author: Angelita Gozaly
 Author-email: s1282003@u-aizu.ac.jp
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s1282003_learn-2023.8.4/setup.py` & `s1282003_learn-2023.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="s1282003_learn",
-    version="2023.08.04",
+    version="2023.08.05",
     author="Angelita Gozaly",
     author_email="s1282003@u-aizu.ac.jp",
     description="This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/angelitagozaly/s1282003_learn",
```

