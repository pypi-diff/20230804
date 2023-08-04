# Comparing `tmp/http_backuper-0.1.2.tar.gz` & `tmp/http_backuper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_backuper-0.1.2.tar", last modified: Thu Aug  3 17:18:23 2023, max compression
+gzip compressed data, was "http_backuper-0.1.3.tar", last modified: Thu Aug  3 17:19:24 2023, max compression
```

## Comparing `http_backuper-0.1.2.tar` & `http_backuper-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:18:23.929284 http_backuper-0.1.2/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1069 2023-08-03 16:49:27.000000 http_backuper-0.1.2/LICENSE
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:18:23.929284 http_backuper-0.1.2/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     2077 2023-08-03 17:10:09.000000 http_backuper-0.1.2/README.md
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:18:23.925284 http_backuper-0.1.2/http_backuper/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:19.000000 http_backuper-0.1.2/http_backuper/__init__.py
--rwxrwxr-x   0 djbios    (1000) djbios    (1000)     9215 2023-08-03 17:18:08.000000 http_backuper-0.1.2/http_backuper/backuper.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1130 2023-08-03 11:49:11.000000 http_backuper-0.1.2/http_backuper/models.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:18:23.929284 http_backuper-0.1.2/http_backuper.egg-info/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      359 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/SOURCES.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        1 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/dependency_links.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      101 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/entry_points.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       59 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/requires.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       20 2023-08-03 17:18:23.000000 http_backuper-0.1.2/http_backuper.egg-info/top_level.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       38 2023-08-03 17:18:23.929284 http_backuper-0.1.2/setup.cfg
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      698 2023-08-03 17:18:21.000000 http_backuper-0.1.2/setup.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:18:23.929284 http_backuper-0.1.2/tests/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:44.000000 http_backuper-0.1.2/tests/__init__.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     8600 2023-08-03 17:01:17.000000 http_backuper-0.1.2/tests/tests.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     1069 2023-08-03 16:49:27.000000 http_backuper-0.1.3/LICENSE
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:19:24.353480 http_backuper-0.1.3/PKG-INFO
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     2077 2023-08-03 17:10:09.000000 http_backuper-0.1.3/README.md
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/http_backuper/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:19.000000 http_backuper-0.1.3/http_backuper/__init__.py
+-rwxrwxr-x   0 djbios    (1000) djbios    (1000)     9228 2023-08-03 17:19:09.000000 http_backuper-0.1.3/http_backuper/backuper.py
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     1130 2023-08-03 11:49:11.000000 http_backuper-0.1.3/http_backuper/models.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/http_backuper.egg-info/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/PKG-INFO
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      359 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/SOURCES.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        1 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/dependency_links.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      101 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/entry_points.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       59 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/requires.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       20 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/top_level.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       38 2023-08-03 17:19:24.353480 http_backuper-0.1.3/setup.cfg
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      698 2023-08-03 17:19:12.000000 http_backuper-0.1.3/setup.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/tests/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:44.000000 http_backuper-0.1.3/tests/__init__.py
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     8600 2023-08-03 17:01:17.000000 http_backuper-0.1.3/tests/tests.py
```

### Comparing `http_backuper-0.1.2/LICENSE` & `http_backuper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.2/README.md` & `http_backuper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.2/http_backuper/backuper.py` & `http_backuper-0.1.3/http_backuper/backuper.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import requests
 import schedule
 import yaml
 from docker import DockerClient
 from healthchecks_io import Client, CheckCreate
 from pydantic import ValidationError
 
-from .models import Config, GeneralSection, BackupSection
+from http_backuper.models import Config, GeneralSection, BackupSection
 
 def setup_logging():
     # Create a custom logger
     logger = logging.getLogger('http_backuper')
 
     # Set the threshold of logger to DEBUG
     logger.setLevel(logging.DEBUG)
```

### Comparing `http_backuper-0.1.2/http_backuper/models.py` & `http_backuper-0.1.3/http_backuper/models.py`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.2/setup.py` & `http_backuper-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='http_backuper',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/djbios/http_backuper',
     author='djbios',
     author_email='dorandval@gmail.com',
     description='A simple backup solution',
     packages=find_packages(),
     install_requires=[
         'pydantic<2', 'requests', 'schedule', 'docker', 'healthchecks_io', 'PyYAML'
```

### Comparing `http_backuper-0.1.2/tests/tests.py` & `http_backuper-0.1.3/tests/tests.py`

 * *Files identical despite different names*

