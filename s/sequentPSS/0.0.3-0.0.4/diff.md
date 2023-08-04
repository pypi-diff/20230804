# Comparing `tmp/sequentPSS-0.0.3.tar.gz` & `tmp/sequentPSS-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentPSS-0.0.3.tar", last modified: Thu Aug  3 22:32:25 2023, max compression
+gzip compressed data, was "sequentPSS-0.0.4.tar", last modified: Thu Aug  3 23:56:58 2023, max compression
```

## Comparing `sequentPSS-0.0.3.tar` & `sequentPSS-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 22:32:25.457002 sequentPSS-0.0.3/
--rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-08-03 22:32:25.456004 sequentPSS-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 22:32:25.417110 sequentPSS-0.0.3/sequentPSS/
--rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.3/sequentPSS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:32:25.450021 sequentPSS-0.0.3/sequentPSS/sampleData/
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.3/sequentPSS/sampleData/O1.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.3/sequentPSS/sampleData/O2.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.3/sequentPSS/sampleData/O3.txt
--rw-rw-rw-   0        0        0   946401 2023-08-03 22:13:09.000000 sequentPSS-0.0.3/sequentPSS/sampleData/concatenated_df.csv
--rw-rw-rw-   0        0        0     4056 2023-08-03 22:30:40.000000 sequentPSS-0.0.3/sequentPSS/sequentPSS.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:32:25.439049 sequentPSS-0.0.3/sequentPSS.egg-info/
--rw-rw-rw-   0        0        0      274 2023-08-03 22:32:24.000000 sequentPSS-0.0.3/sequentPSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-08-03 22:32:25.000000 sequentPSS-0.0.3/sequentPSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 22:32:24.000000 sequentPSS-0.0.3/sequentPSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 22:32:25.000000 sequentPSS-0.0.3/sequentPSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 22:32:25.000000 sequentPSS-0.0.3/sequentPSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 22:32:25.458001 sequentPSS-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1439 2023-08-03 22:32:15.000000 sequentPSS-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:56:58.803660 sequentPSS-0.0.4/
+-rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-08-03 23:56:58.802663 sequentPSS-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 23:56:58.755788 sequentPSS-0.0.4/sequentPSS/
+-rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.4/sequentPSS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:56:58.797677 sequentPSS-0.0.4/sequentPSS/sampleData/
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.4/sequentPSS/sampleData/O1.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.4/sequentPSS/sampleData/O2.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.4/sequentPSS/sampleData/O3.txt
+-rw-rw-rw-   0        0        0   946401 2023-08-03 22:13:09.000000 sequentPSS-0.0.4/sequentPSS/sampleData/concatenated_df.csv
+-rw-rw-rw-   0        0        0     6837 2023-08-03 23:56:26.000000 sequentPSS-0.0.4/sequentPSS/sequentPSS.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:56:58.786706 sequentPSS-0.0.4/sequentPSS.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-08-03 23:56:57.000000 sequentPSS-0.0.4/sequentPSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-08-03 23:56:58.000000 sequentPSS-0.0.4/sequentPSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 23:56:57.000000 sequentPSS-0.0.4/sequentPSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 23:56:58.000000 sequentPSS-0.0.4/sequentPSS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 23:56:58.000000 sequentPSS-0.0.4/sequentPSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 23:56:58.804658 sequentPSS-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2023-08-03 22:42:15.000000 sequentPSS-0.0.4/setup.py
```

### Comparing `sequentPSS-0.0.3/sequentPSS/sampleData/O1.txt` & `sequentPSS-0.0.4/sequentPSS/sampleData/O1.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.3/sequentPSS/sampleData/O2.txt` & `sequentPSS-0.0.4/sequentPSS/sampleData/O2.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.3/sequentPSS/sampleData/O3.txt` & `sequentPSS-0.0.4/sequentPSS/sampleData/O3.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.3/sequentPSS/sampleData/concatenated_df.csv` & `sequentPSS-0.0.4/sequentPSS/sampleData/concatenated_df.csv`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.3/setup.py` & `sequentPSS-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sequentPSS',
-    version = '0.0.3',
+    version = '0.0.4',
     description = "algorithm for sequential parameter searching with GSA",
     url = 'https://github.com/MG-Choi/sequentPSS',
     author = 'MoongiChoi',
     author_email = 'u1316663@utah.edu',
     packages = find_packages(),
     package_data = {'sequentPSS': ['sampleData/concatenated_df.csv', 'sampleData/O1.txt', 'sampleData/O2.txt', 'sampleData/O3.txt']},
     include_package_data = True,
```

