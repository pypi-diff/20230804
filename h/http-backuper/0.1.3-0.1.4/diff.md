# Comparing `tmp/http_backuper-0.1.3.tar.gz` & `tmp/http_backuper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_backuper-0.1.3.tar", last modified: Thu Aug  3 17:19:24 2023, max compression
+gzip compressed data, was "http_backuper-0.1.4.tar", last modified: Fri Aug  4 15:44:37 2023, max compression
```

## Comparing `http_backuper-0.1.3.tar` & `http_backuper-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1069 2023-08-03 16:49:27.000000 http_backuper-0.1.3/LICENSE
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:19:24.353480 http_backuper-0.1.3/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     2077 2023-08-03 17:10:09.000000 http_backuper-0.1.3/README.md
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/http_backuper/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:19.000000 http_backuper-0.1.3/http_backuper/__init__.py
--rwxrwxr-x   0 djbios    (1000) djbios    (1000)     9228 2023-08-03 17:19:09.000000 http_backuper-0.1.3/http_backuper/backuper.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1130 2023-08-03 11:49:11.000000 http_backuper-0.1.3/http_backuper/models.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/http_backuper.egg-info/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      312 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      359 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/SOURCES.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        1 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/dependency_links.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      101 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/entry_points.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       59 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/requires.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       20 2023-08-03 17:19:24.000000 http_backuper-0.1.3/http_backuper.egg-info/top_level.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       38 2023-08-03 17:19:24.353480 http_backuper-0.1.3/setup.cfg
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      698 2023-08-03 17:19:12.000000 http_backuper-0.1.3/setup.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-03 17:19:24.353480 http_backuper-0.1.3/tests/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:44.000000 http_backuper-0.1.3/tests/__init__.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     8600 2023-08-03 17:01:17.000000 http_backuper-0.1.3/tests/tests.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:44:37.639207 http_backuper-0.1.4/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     1069 2023-08-03 16:49:27.000000 http_backuper-0.1.4/LICENSE
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      311 2023-08-04 15:44:37.639207 http_backuper-0.1.4/PKG-INFO
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     2077 2023-08-03 17:10:09.000000 http_backuper-0.1.4/README.md
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:44:37.639207 http_backuper-0.1.4/http_backuper/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:19.000000 http_backuper-0.1.4/http_backuper/__init__.py
+-rwxrwxr-x   0 djbios    (1000) djbios    (1000)     9232 2023-08-04 15:41:57.000000 http_backuper-0.1.4/http_backuper/backuper.py
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     1136 2023-08-04 15:40:06.000000 http_backuper-0.1.4/http_backuper/models.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:44:37.639207 http_backuper-0.1.4/http_backuper.egg-info/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      311 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/PKG-INFO
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      359 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/SOURCES.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        1 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/dependency_links.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      101 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/entry_points.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       59 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/requires.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       20 2023-08-04 15:44:37.000000 http_backuper-0.1.4/http_backuper.egg-info/top_level.txt
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)       38 2023-08-04 15:44:37.639207 http_backuper-0.1.4/setup.cfg
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)      698 2023-08-04 15:43:15.000000 http_backuper-0.1.4/setup.py
+drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:44:37.639207 http_backuper-0.1.4/tests/
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:44.000000 http_backuper-0.1.4/tests/__init__.py
+-rw-rw-r--   0 djbios    (1000) djbios    (1000)     8600 2023-08-03 17:01:17.000000 http_backuper-0.1.4/tests/tests.py
```

### Comparing `http_backuper-0.1.3/LICENSE` & `http_backuper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.3/README.md` & `http_backuper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.3/http_backuper/backuper.py` & `http_backuper-0.1.4/http_backuper/backuper.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import yaml
 from docker import DockerClient
 from healthchecks_io import Client, CheckCreate
 from pydantic import ValidationError
 
 from http_backuper.models import Config, GeneralSection, BackupSection
 
+
 def setup_logging():
     # Create a custom logger
     logger = logging.getLogger('http_backuper')
 
     # Set the threshold of logger to DEBUG
     logger.setLevel(logging.DEBUG)
 
@@ -91,14 +92,17 @@
                 tar.addfile(tarinfo, fileobj=f)
 
     logger.info(
         f"Successfully added container {container_name} path {source} to tar file"
     )
 
 
+
+
+
 def run_command_in_container(
     client: DockerClient,
     container_name: str,
     command: str,
     tar: tarfile.TarFile,
     filename: str,
 ):
```

### Comparing `http_backuper-0.1.3/http_backuper/models.py` & `http_backuper-0.1.4/http_backuper/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List
+from typing import List, Dict
 from typing import Optional
 
 from pydantic import BaseModel, HttpUrl, validator, AnyUrl
 
 
 class HttpMethod(Enum):
     GET = "GET"
@@ -37,15 +37,15 @@
     schedule: Frequency
     sources: List[Source]
 
 
 class GeneralSection(BaseModel):
     url: AnyUrl
     http_verb: HttpMethod
-    requests_properties: Optional[dict[str, str]]
+    requests_properties: Optional[Dict[str, str]]
     healthchecks_io_api_key: Optional[str]
     file_field_name: Optional[str] = "file"
 
 
 class Config(BaseModel):
     general: GeneralSection
     backups: List[BackupSection]
```

### Comparing `http_backuper-0.1.3/setup.py` & `http_backuper-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='http_backuper',
-    version='0.1.3',
+    version='0.1.4',
     url='https://github.com/djbios/http_backuper',
     author='djbios',
     author_email='dorandval@gmail.com',
     description='A simple backup solution',
     packages=find_packages(),
     install_requires=[
-        'pydantic<2', 'requests', 'schedule', 'docker', 'healthchecks_io', 'PyYAML'
+        'pydantic<2', 'requests', 'schedule', 'docker', 'healthchecks_io', 'PyYAML',
     ],
     entry_points={
         'console_scripts': [
             'http_backuper=http_backuper.backuper:main',
             'backuper=http_backuper.backuper:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.8',
     ],
 )
```

### Comparing `http_backuper-0.1.3/tests/tests.py` & `http_backuper-0.1.4/tests/tests.py`

 * *Files identical despite different names*

