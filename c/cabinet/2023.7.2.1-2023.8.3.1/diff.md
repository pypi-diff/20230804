# Comparing `tmp/cabinet-2023.7.2.1.tar.gz` & `tmp/cabinet-2023.8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.7.2.1.tar", last modified: Mon Jul  3 04:10:58 2023, max compression
+gzip compressed data, was "cabinet-2023.8.3.1.tar", last modified: Fri Aug  4 04:55:23 2023, max compression
```

## Comparing `cabinet-2023.7.2.1.tar` & `cabinet-2023.8.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1090 2023-06-17 20:33:55.000000 cabinet-2023.7.2.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7338 2023-07-03 03:56:29.000000 cabinet-2023.7.2.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.7.2.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.973777 cabinet-2023.7.2.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.973777 cabinet-2023.7.2.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-25 04:32:18.000000 cabinet-2023.7.2.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-06-25 04:32:22.000000 cabinet-2023.7.2.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    34085 2023-07-03 04:10:25.000000 cabinet-2023.7.2.1/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2314 2023-07-03 03:56:29.000000 cabinet-2023.7.2.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.7.2.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5874 2023-06-25 05:21:17.000000 cabinet-2023.7.2.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1090 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7338 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    34440 2023-08-04 04:52:04.000000 cabinet-2023.8.3.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2474 2023-08-04 04:42:33.000000 cabinet-2023.8.3.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-08-04 04:55:23.000000 cabinet-2023.8.3.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2023-08-04 04:55:23.000000 cabinet-2023.8.3.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-08-04 04:55:23.000000 cabinet-2023.8.3.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-08-04 04:55:23.000000 cabinet-2023.8.3.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-08-04 04:55:23.000000 cabinet-2023.8.3.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-08-04 04:55:23.121076 cabinet-2023.8.3.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5874 2023-08-04 04:33:55.000000 cabinet-2023.8.3.1/test/test___init__.py
```

### Comparing `cabinet-2023.7.2.1/LICENSE` & `cabinet-2023.8.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.7.2.1/PKG-INFO` & `cabinet-2023.8.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.7.2.1
+Version: 2023.8.3.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.7.2.1/README.md` & `cabinet-2023.8.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2023.7.2.1/setup.cfg` & `cabinet-2023.8.3.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.07.02.1
+version = 2023.08.03.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.7.2.1/src/cabinet/cabinet.py` & `cabinet-2023.8.3.1/src/cabinet/cabinet.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,37 +10,39 @@
     cab = Cabinet()
     ```
 """
 import os
 import ast
 import sys
 import json
-import argparse
 import logging
-import importlib.metadata
 import getpass
 import pathlib
+import argparse
 import subprocess
-from datetime import date, datetime
+import importlib.metadata
 from typing import Optional
+from datetime import date, datetime
 import pymongo.errors
 from pymongo.mongo_client import MongoClient
 from pymongo.server_api import ServerApi
 from bson import json_util, ObjectId
 from .constants import (
     NEW_SETUP_MSG_INTRO,
     NEW_SETUP_MSG_MONGODB_INSTRUCTIONS,
     CONFIG_MONGODB_USERNAME,
     CONFIG_MONGODB_PASSWORD,
     CONFIG_MONGODB_CLUSTER_NAME,
     CONFIG_MONGODB_DB_NAME,
     CONFIG_PATH_CABINET,
     ERROR_CONFIG_MISSING_VALUES,
     ERROR_CONFIG_JSON_DECODE,
-    ERROR_CONFIG_FILE_INVALID
+    ERROR_CONFIG_FILE_INVALID,
+    ERROR_MONGODB_TIMEOUT,
+    ERROR_MONGODB_DNS
 )
 from .mail import Mail
 
 
 class Cabinet:
     """
     Cabinet class
@@ -251,16 +253,24 @@
                         f"@{self.mongodb_cluster_name}.1jxchnk.mongodb.net/"
                         f"{self.mongodb_db_name}?retryWrites=true&w=majority")
             self.client = MongoClient(self.uri, server_api=ServerApi('1'))
             self.database = self.client.cabinet
         except pymongo.errors.InvalidURI as error:
             print(ERROR_CONFIG_FILE_INVALID)
             print(error._message)
-
             sys.exit(-1)
+        except pymongo.errors.ServerSelectionTimeoutError as error:
+            print(ERROR_MONGODB_TIMEOUT)
+            print(error)
+            sys.exit(-1)
+        except pymongo.errors.ConfigurationError as error:
+            print(ERROR_MONGODB_DNS)
+            print(error)
+            sys.exit(-1)
+
 
         path_log = self.get('path', 'log') or '~/.cabinet/log'
 
         expanded_path = os.path.expanduser(path_log)
         directory_path = os.path.abspath(expanded_path)
         directory_path_with_slash = os.path.join(directory_path, '')
```

### Comparing `cabinet-2023.7.2.1/src/cabinet/constants.py` & `cabinet-2023.8.3.1/src/cabinet/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,8 +83,16 @@
 ERROR_CONFIG_JSON_DECODE = """
 The configuration file is not valid JSON.
 
 Do you want to replace it with an empty JSON file?
 This will reset your MongoDB credentials, but your data will be safe.
 
 (y/n)\n
+"""
+
+ERROR_MONGODB_TIMEOUT = """
+Timeout error: Could not connect to the MongoDB server:
+"""
+
+ERROR_MONGODB_DNS = """
+DNS resolution failed for MongoDB server:
 """
```

### Comparing `cabinet-2023.7.2.1/src/cabinet/mail.py` & `cabinet-2023.8.3.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.7.2.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.8.3.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.7.2.1
+Version: 2023.8.3.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.7.2.1/test/test___init__.py` & `cabinet-2023.8.3.1/test/test___init__.py`

 * *Files identical despite different names*

