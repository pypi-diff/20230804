# Comparing `tmp/SudachiDict-small-20230110.tar.gz` & `tmp/SudachiDict-small-20230711rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SudachiDict-small-20230110.tar", last modified: Thu Jan 12 02:30:58 2023, max compression
+gzip compressed data, was "SudachiDict-small-20230711rc1.tar", last modified: Fri Aug  4 09:06:01 2023, max compression
```

## Comparing `SudachiDict-small-20230110.tar` & `SudachiDict-small-20230711rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arseny    (1000) arseny    (1000)        0 2023-01-12 02:30:58.849646 SudachiDict-small-20230110/
--rw-r--r--   0 arseny    (1000) arseny    (1000)       86 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/INFO.json
--rw-r--r--   0 arseny    (1000) arseny    (1000)     6037 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/LEGAL
--rw-r--r--   0 arseny    (1000) arseny    (1000)    11358 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/LICENSE-2.0.txt
--rw-r--r--   0 arseny    (1000) arseny    (1000)       84 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/MANIFEST.in
--rw-r--r--   0 arseny    (1000) arseny    (1000)     2433 2023-01-12 02:30:58.849646 SudachiDict-small-20230110/PKG-INFO
--rw-r--r--   0 arseny    (1000) arseny    (1000)     2097 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/README.md
-drwxr-xr-x   0 arseny    (1000) arseny    (1000)        0 2023-01-12 02:30:58.849646 SudachiDict-small-20230110/SudachiDict_small.egg-info/
--rw-r--r--   0 arseny    (1000) arseny    (1000)     2433 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/SudachiDict_small.egg-info/PKG-INFO
--rw-r--r--   0 arseny    (1000) arseny    (1000)      296 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/SudachiDict_small.egg-info/SOURCES.txt
--rw-r--r--   0 arseny    (1000) arseny    (1000)        1 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/SudachiDict_small.egg-info/dependency_links.txt
--rw-r--r--   0 arseny    (1000) arseny    (1000)       20 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/SudachiDict_small.egg-info/requires.txt
--rw-r--r--   0 arseny    (1000) arseny    (1000)       18 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/SudachiDict_small.egg-info/top_level.txt
--rw-r--r--   0 arseny    (1000) arseny    (1000)       38 2023-01-12 02:30:58.849646 SudachiDict-small-20230110/setup.cfg
--rw-r--r--   0 arseny    (1000) arseny    (1000)     2585 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/setup.py
-drwxr-xr-x   0 arseny    (1000) arseny    (1000)        0 2023-01-12 02:30:58.849646 SudachiDict-small-20230110/sudachidict_small/
--rw-r--r--   0 arseny    (1000) arseny    (1000)        0 2023-01-12 02:30:58.000000 SudachiDict-small-20230110/sudachidict_small/__init__.py
+drwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)        0 2023-08-04 09:06:01.203385 SudachiDict-small-20230711rc1/
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)       91 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/INFO.json
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)     6037 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/LEGAL
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)    11358 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/LICENSE-2.0.txt
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)       84 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/MANIFEST.in
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)     2456 2023-08-04 09:06:01.203385 SudachiDict-small-20230711rc1/PKG-INFO
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)     2097 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/README.md
+drwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)        0 2023-08-04 09:06:01.202384 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)     2456 2023-08-04 09:06:01.000000 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/PKG-INFO
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)      296 2023-08-04 09:06:01.000000 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/SOURCES.txt
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)        1 2023-08-04 09:06:01.000000 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/dependency_links.txt
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)       20 2023-08-04 09:06:01.000000 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/requires.txt
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)       18 2023-08-04 09:06:01.000000 SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/top_level.txt
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)       38 2023-08-04 09:06:01.203385 SudachiDict-small-20230711rc1/setup.cfg
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)     2543 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/setup.py
+drwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)        0 2023-08-04 09:06:01.202384 SudachiDict-small-20230711rc1/sudachidict_small/
+-rwxrwxrwx   0 eiennohito  (1000) eiennohito  (1000)        0 2023-08-04 09:05:55.000000 SudachiDict-small-20230711rc1/sudachidict_small/__init__.py
```

### Comparing `SudachiDict-small-20230110/LEGAL` & `SudachiDict-small-20230711rc1/LEGAL`

 * *Files identical despite different names*

### Comparing `SudachiDict-small-20230110/LICENSE-2.0.txt` & `SudachiDict-small-20230711rc1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `SudachiDict-small-20230110/PKG-INFO` & `SudachiDict-small-20230711rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: SudachiDict-small
-Version: 20230110
+Version: 20230711rc1
 Summary: Sudachi Dictionary for SudachiPy - Small Edition
 Home-page: https://github.com/WorksApplications/SudachiDict
 Author: Works Applications
 Author-email: sudachi@worksap.co.jp
 License: Apache-2.0
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE-2.0.txt
 
 # Sudachi Dictionary for SudachiPy
 
 - [WorksApplications/SudachiDict](https://github.com/WorksApplications/SudachiDict)
 - [WorksApplications/SudachiPy](https://github.com/WorksApplications/SudachiPy)
@@ -55,7 +56,9 @@
 
 In case you are using SudachiPy before v0.5.2, please visit the old SudachiPy documentation.
 
 - english
   - [https://github.com/WorksApplications/SudachiPy/tree/v0.5.1#dictionary-edition](https://github.com/WorksApplications/SudachiPy/tree/v0.5.1#dictionary-edition)
 - japanese
   - [https://github.com/WorksApplications/SudachiPy/blob/v0.5.1/docs/tutorial.md#%辞書の種類](https://github.com/WorksApplications/SudachiPy/blob/v0.5.1/docs/tutorial.md#%E8%BE%9E%E6%9B%B8%E3%81%AE%E7%A8%AE%E9%A1%9E)
+
+
```

### Comparing `SudachiDict-small-20230110/README.md` & `SudachiDict-small-20230711rc1/README.md`

 * *Files identical despite different names*

### Comparing `SudachiDict-small-20230110/SudachiDict_small.egg-info/PKG-INFO` & `SudachiDict-small-20230711rc1/SudachiDict_small.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: SudachiDict-small
-Version: 20230110
+Version: 20230711rc1
 Summary: Sudachi Dictionary for SudachiPy - Small Edition
 Home-page: https://github.com/WorksApplications/SudachiDict
 Author: Works Applications
 Author-email: sudachi@worksap.co.jp
 License: Apache-2.0
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE-2.0.txt
 
 # Sudachi Dictionary for SudachiPy
 
 - [WorksApplications/SudachiDict](https://github.com/WorksApplications/SudachiDict)
 - [WorksApplications/SudachiPy](https://github.com/WorksApplications/SudachiPy)
@@ -55,7 +56,9 @@
 
 In case you are using SudachiPy before v0.5.2, please visit the old SudachiPy documentation.
 
 - english
   - [https://github.com/WorksApplications/SudachiPy/tree/v0.5.1#dictionary-edition](https://github.com/WorksApplications/SudachiPy/tree/v0.5.1#dictionary-edition)
 - japanese
   - [https://github.com/WorksApplications/SudachiPy/blob/v0.5.1/docs/tutorial.md#%辞書の種類](https://github.com/WorksApplications/SudachiPy/blob/v0.5.1/docs/tutorial.md#%E8%BE%9E%E6%9B%B8%E3%81%AE%E7%A8%AE%E9%A1%9E)
+
+
```

### Comparing `SudachiDict-small-20230110/setup.py` & `SudachiDict-small-20230711rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Works Applications Co., Ltd.
+# Copyright (c) 2020-2023 Works Applications Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,48 +11,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 import os
 import json
-from logging import getLogger
+import sys
 from urllib.parse import urlparse
 from urllib.request import urlretrieve
 from zipfile import ZipFile
 
-
 with open("INFO.json") as fh:
     dict_info = json.load(fh)
 PKG_VERSION = dict_info["version"]
 DICT_VERSION = dict_info["dict_version"]
 DICT_EDITION = dict_info["edition"]
 
-ZIP_URL = "http://sudachi.s3-website-ap-northeast-1.amazonaws.com/sudachidict/"\
+ZIP_URL = "https://d2ej7fkh96fzlu.cloudfront.net/sudachidict/" \
           "sudachi-dictionary-{}-{}.zip".format(DICT_VERSION, DICT_EDITION)
 ZIP_NAME = urlparse(ZIP_URL).path.split("/")[-1]
 UNZIP_NAME = "sudachi-dictionary-{}".format(DICT_VERSION)
 PKG_DIR = "sudachidict_{}".format(DICT_EDITION)
 RESOURCE_DIR = os.path.join(PKG_DIR, "resources")
 BINARY_NAME = "system_{}.dic".format(DICT_EDITION)
 
-
-logger = getLogger(__name__)
-
 # Download and place the dictionary file
 if not os.path.exists(RESOURCE_DIR):
-    logger.warning("Downloading the Sudachi dictionary (It may take a while) ...")
+    print("Downloading the binary Sudachi dictionary (it may take some time) ...", file=sys.stderr)
     _, _msg = urlretrieve(ZIP_URL, ZIP_NAME)
     with ZipFile(ZIP_NAME) as z:
         z.extractall()
     os.rename(UNZIP_NAME, RESOURCE_DIR)
     os.rename(os.path.join(RESOURCE_DIR, BINARY_NAME),
               os.path.join(RESOURCE_DIR, "system.dic"))
     os.remove(ZIP_NAME)
-    logger.warning("... downloaded and placed the dictionary at `{}`.".format(RESOURCE_DIR))
+    print("downloaded and extracted dictionary to `{}`.".format(RESOURCE_DIR), file=sys.stderr)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SudachiDict-{}".format(DICT_EDITION),
     version=PKG_VERSION,
```

