# Comparing `tmp/hugg-0.1.6.tar.gz` & `tmp/hugg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.1.6.tar", last modified: Thu Aug  3 17:32:53 2023, max compression
+gzip compressed data, was "hugg-0.1.7.tar", last modified: Thu Aug  3 17:43:58 2023, max compression
```

## Comparing `hugg-0.1.6.tar` & `hugg-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:32:53.126700 hugg-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 17:32:39.000000 hugg-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:32:53.126700 hugg-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 17:32:39.000000 hugg-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:32:53.122700 hugg-0.1.6/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    43126 2023-08-03 17:32:39.000000 hugg-0.1.6/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:32:53.126700 hugg-0.1.6/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:32:53.000000 hugg-0.1.6/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 17:32:53.000000 hugg-0.1.6/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:32:53.000000 hugg-0.1.6/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 17:32:53.000000 hugg-0.1.6/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 17:32:53.000000 hugg-0.1.6/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:32:53.126700 hugg-0.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 17:32:39.000000 hugg-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:43:58.440466 hugg-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 17:43:46.000000 hugg-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:43:58.440466 hugg-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 17:43:46.000000 hugg-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:43:58.436466 hugg-0.1.7/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    43125 2023-08-03 17:43:46.000000 hugg-0.1.7/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:43:58.440466 hugg-0.1.7/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 17:43:58.000000 hugg-0.1.7/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 17:43:58.000000 hugg-0.1.7/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:43:58.000000 hugg-0.1.7/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 17:43:58.000000 hugg-0.1.7/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 17:43:58.000000 hugg-0.1.7/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:43:58.440466 hugg-0.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-08-03 17:43:46.000000 hugg-0.1.7/setup.py
```

### Comparing `hugg-0.1.6/LICENSE` & `hugg-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.1.6/hugg/__init__.py` & `hugg-0.1.7/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import os,sys,types,importlib.machinery,shutil,mystring
-from copy import deepcopy as dc
+import os,sys,types,importlib.machinery,shutil
 import threading as thread
 from pathlib import Path
 from abc import ABC, abstractmethod
 if sys.version_info[0] < 3: 
     from StringIO import StringIO
 else:
     from io import StringIO
@@ -85,14 +84,15 @@
 
         if self.dowraplambda(download_to) is True:
             download_to = self.unwrap(download_to)
         
         return download_to
 
     def upload(self, path=None,path_in_repo=None):
+        from copy import deepcopy as dc
         og_path,og_path_in_repo = dc(path),dc(path_in_repo)
         if self.dowraplambda(path) is True:
             try:
                 path = self.wrap(path)
                 path_in_repo += ".nosj"
             except:
                 path,path_in_repo = og_path,og_path_in_repo
```

### Comparing `hugg-0.1.6/setup.py` & `hugg-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

