# Comparing `tmp/robotframework-requestspro-1.1.9.tar.gz` & `tmp/robotframework-requestspro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.1.9.tar", last modified: Fri Aug  4 03:55:32 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.0.tar", last modified: Fri Aug  4 04:31:47 2023, max compression
```

## Comparing `robotframework-requestspro-1.1.9.tar` & `robotframework-requestspro-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.797522 robotframework-requestspro-1.1.9/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 03:55:32.797394 robotframework-requestspro-1.1.9/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 03:55:32.797567 robotframework-requestspro-1.1.9/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.794977 robotframework-requestspro-1.1.9/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.796632 robotframework-requestspro-1.1.9/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2274 2023-08-04 03:48:18.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 03:33:25.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.797190 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.725133 robotframework-requestspro-1.2.0/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 04:31:47.725015 robotframework-requestspro-1.2.0/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 04:31:47.725175 robotframework-requestspro-1.2.0/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.722440 robotframework-requestspro-1.2.0/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.724236 robotframework-requestspro-1.2.0/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2320 2023-08-04 04:30:58.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 04:31:35.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.724846 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.1.9/LICENSE` & `robotframework-requestspro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.9/PKG-INFO` & `robotframework-requestspro-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.1.9
+Version: 1.2.0
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.1.9/setup.py` & `robotframework-requestspro-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.9/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.0/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import pandas as pd
 from robot.api import logger
 from typing import List
 
-
 class DynamicTestCases(object):
     """A Robot Framework test library to dynamically add test cases to the current suite."""
 
     ROBOT_LISTENER_API_VERSION = 3
     ROBOT_LIBRARY_SCOPE = 'TEST SUITE'
 
     def __init__(self):
         self.ROBOT_LIBRARY_LISTENER = self
 
     def _start_suite(self, suite, result):
         # Save current suite so that we can modify it later
         self.current_suite = suite
 
-    def add_test_case(self, name: str, doc: str, tags: List[str], kwname: str, *args):
+    def add_test_case(self, name: str, doc: str, tags: List[str], kwname: str, **kwargs):
         """Adds a test case to the current suite.
 
         `name`: The test case name (str).
         `doc`: The documentation for the test case (str).
         `tags`: Tags to be associated with the test case (List of str).
         `kwname`: The keyword to call (str).
-        `*args`: The arguments to pass to the keyword.
+        `**kwargs`: Keyword arguments to pass to the keyword.
 
         Example:
-        | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | Log Many | Hello | world | WARN |
+        | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | Log Many | arg1=Hello | arg2=world | level=WARN |
         """
         tc = self.current_suite.tests.create(name=name, doc=doc, tags=tags)
-        tc.keywords.create(name=kwname, args=args)
-        logger.info(f"Added test case '{name}' with keyword '{kwname}' and args: {args}")
+        tc.keywords.create(name=kwname, assign=kwargs)
+        logger.info(f"Added test case '{name}' with keyword '{kwname}' and keyword arguments: {kwargs}")
 
     def read_test_data_and_add_test_cases(self, csv_file_path: str):
         """Reads test data from a CSV file and adds test cases dynamically.
 
         `csv_file_path`: The path to the CSV file containing test data.
 
         Example:
@@ -43,12 +42,12 @@
         try:
             df = pd.read_csv(csv_file_path)
             for _, row in df.iterrows():
                 name = row.get('test_name', '')
                 doc = row.get('test_scenario', '')
                 tags = row.get('test_tags', '').split(',')
                 kwname = row.get('keyword', '')
-                args = [row.get(param, '') for param in row.index if param.endswith('_v')]
-                self.add_test_case(name=name, doc=doc, tags=tags, kwname=kwname, *args)
+                kwargs = {col[:-2]: row[col] for col in df.columns if col.endswith('_v')}
+                self.add_test_case(name=name, doc=doc, tags=tags, kwname=kwname, **kwargs)
             logger.info(f"Successfully added test cases from '{csv_file_path}'.")
         except Exception as e:
             logger.error(f"Error occurred while reading test data from '{csv_file_path}': {e}")
```

### Comparing `robotframework-requestspro-1.1.9/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.0/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.9/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.0/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.1.9
+Version: 1.2.0
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

