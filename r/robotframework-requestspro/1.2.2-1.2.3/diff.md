# Comparing `tmp/robotframework-requestspro-1.2.2.tar.gz` & `tmp/robotframework-requestspro-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.2.tar", last modified: Fri Aug  4 13:15:41 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.3.tar", last modified: Fri Aug  4 13:32:10 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.2.tar` & `robotframework-requestspro-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.702217 robotframework-requestspro-1.2.2/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:15:41.702106 robotframework-requestspro-1.2.2/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 13:15:41.702258 robotframework-requestspro-1.2.2/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.699768 robotframework-requestspro-1.2.2/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.701375 robotframework-requestspro-1.2.2/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2559 2023-08-04 13:15:21.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 13:15:28.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.701945 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456910 robotframework-requestspro-1.2.3/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:32:10.456795 robotframework-requestspro-1.2.3/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 13:32:10.456951 robotframework-requestspro-1.2.3/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.454405 robotframework-requestspro-1.2.3/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456001 robotframework-requestspro-1.2.3/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2818 2023-08-04 13:31:45.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 13:31:54.000000 robotframework-requestspro-1.2.3/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:32:10.456636 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 13:32:10.000000 robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.2/LICENSE` & `robotframework-requestspro-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.2/PKG-INFO` & `robotframework-requestspro-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.2
+Version: 1.2.3
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.2/setup.py` & `robotframework-requestspro-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.2/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.3/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 from robot.api import logger
 from typing import List
 
+
 class DynamicTestCases(object):
     """A Robot Framework test library to dynamically add test cases to the current suite."""
 
     ROBOT_LISTENER_API_VERSION = 3
     ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
 
     def __init__(self):
@@ -25,23 +26,32 @@
         `**kwargs`: Keyword arguments to pass to the keyword.
 
         Example:
         | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | Log Many | arg1=Hello | arg2=world | level=WARN |
         """
         body = [
             {
-                "keyword": kwname,
-                "args": [],
-                "assign": {f"${{{arg_name}}}": arg_value for arg_name, arg_value in kwargs.items()},
+                "keyword": "Set Test Variable",
+                "args": [f"${{{arg_name}}}", arg_value],
                 "type": "kw",
                 "match": "exact"
             }
+            for arg_name, arg_value in kwargs.items()
         ]
+        body.append({
+            "keyword": kwname,
+            "args": [],
+            "type": "kw",
+            "match": "exact"
+        })
+
+        tc = self.current_suite.tests.create(name=name, doc=doc, tags=tags)
+        for step in body:
+            tc.body.create_step(step['keyword'], *step['args'], type=step['type'], match=step['match'])
 
-        tc = self.current_suite.tests.create(name=name, doc=doc, tags=tags, body=body)
         logger.info(f"Added test case '{name}' with keyword '{kwname}' and keyword arguments: {kwargs}")
 
     def read_test_data_and_add_test_cases(self, csv_file_path: str):
         """Reads test data from a CSV file and adds test cases dynamically.
 
         `csv_file_path`: The path to the CSV file containing test data.
```

### Comparing `robotframework-requestspro-1.2.2/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.3/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.2/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.3/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.2
+Version: 1.2.3
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.3/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

