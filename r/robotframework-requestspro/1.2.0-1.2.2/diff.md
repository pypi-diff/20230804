# Comparing `tmp/robotframework-requestspro-1.2.0.tar.gz` & `tmp/robotframework-requestspro-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.0.tar", last modified: Fri Aug  4 04:31:47 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.2.tar", last modified: Fri Aug  4 13:15:41 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.0.tar` & `robotframework-requestspro-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.725133 robotframework-requestspro-1.2.0/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 04:31:47.725015 robotframework-requestspro-1.2.0/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 04:31:47.725175 robotframework-requestspro-1.2.0/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.722440 robotframework-requestspro-1.2.0/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.724236 robotframework-requestspro-1.2.0/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2320 2023-08-04 04:30:58.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 04:31:35.000000 robotframework-requestspro-1.2.0/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 04:31:47.724846 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 04:31:47.000000 robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.702217 robotframework-requestspro-1.2.2/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:15:41.702106 robotframework-requestspro-1.2.2/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 13:15:41.702258 robotframework-requestspro-1.2.2/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.699768 robotframework-requestspro-1.2.2/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.701375 robotframework-requestspro-1.2.2/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2559 2023-08-04 13:15:21.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 13:15:28.000000 robotframework-requestspro-1.2.2/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 13:15:41.701945 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 13:15:41.000000 robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.0/LICENSE` & `robotframework-requestspro-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.0/PKG-INFO` & `robotframework-requestspro-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.0
+Version: 1.2.2
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.0/setup.py` & `robotframework-requestspro-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.0/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.2/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,25 @@
         `tags`: Tags to be associated with the test case (List of str).
         `kwname`: The keyword to call (str).
         `**kwargs`: Keyword arguments to pass to the keyword.
 
         Example:
         | Add Test Case | Example Test Case | This is a dynamic test case | ['smoke'] | Log Many | arg1=Hello | arg2=world | level=WARN |
         """
-        tc = self.current_suite.tests.create(name=name, doc=doc, tags=tags)
-        tc.keywords.create(name=kwname, assign=kwargs)
+        body = [
+            {
+                "keyword": kwname,
+                "args": [],
+                "assign": {f"${{{arg_name}}}": arg_value for arg_name, arg_value in kwargs.items()},
+                "type": "kw",
+                "match": "exact"
+            }
+        ]
+
+        tc = self.current_suite.tests.create(name=name, doc=doc, tags=tags, body=body)
         logger.info(f"Added test case '{name}' with keyword '{kwname}' and keyword arguments: {kwargs}")
 
     def read_test_data_and_add_test_cases(self, csv_file_path: str):
         """Reads test data from a CSV file and adds test cases dynamically.
 
         `csv_file_path`: The path to the CSV file containing test data.
```

### Comparing `robotframework-requestspro-1.2.0/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.2/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.0/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.2/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.0
+Version: 1.2.2
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.0/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.2/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

