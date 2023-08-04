# Comparing `tmp/promptwatch-0.2.7.tar.gz` & `tmp/promptwatch-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.7.tar", last modified: Wed Jul 26 12:46:14 2023, max compression
+gzip compressed data, was "promptwatch-0.2.8.tar", last modified: Fri Aug  4 12:58:19 2023, max compression
```

## Comparing `promptwatch-0.2.7.tar` & `promptwatch-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.144037 promptwatch-0.2.7/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-26 12:46:14.143818 promptwatch-0.2.7/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.7/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.7/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-26 12:46:14.144087 promptwatch-0.2.7/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.7/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.133565 promptwatch-0.2.7/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.137215 promptwatch-0.2.7/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-26 12:43:06.000000 promptwatch-0.2.7/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-07-22 21:21:26.000000 promptwatch-0.2.7/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.7/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-07-14 21:49:02.000000 promptwatch-0.2.7/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.7/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.140639 promptwatch-0.2.7/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.7/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13202 2023-07-22 21:45:48.000000 promptwatch-0.2.7/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    31232 2023-07-25 15:13:47.000000 promptwatch-0.2.7/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    18116 2023-07-18 10:44:42.000000 promptwatch-0.2.7/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.142930 promptwatch-0.2.7/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.7/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.138965 promptwatch-0.2.7/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.7/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.255021 promptwatch-0.2.8/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-08-04 12:58:19.254832 promptwatch-0.2.8/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.8/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.8/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-08-04 12:58:19.255074 promptwatch-0.2.8/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.8/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.244933 promptwatch-0.2.8/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.249518 promptwatch-0.2.8/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-08-04 12:57:03.000000 promptwatch-0.2.8/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-07-22 21:21:26.000000 promptwatch-0.2.8/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.8/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.8/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-07-14 21:49:02.000000 promptwatch-0.2.8/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.8/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.252665 promptwatch-0.2.8/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.8/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13202 2023-07-22 21:45:48.000000 promptwatch-0.2.8/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    31232 2023-07-25 15:13:47.000000 promptwatch-0.2.8/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.8/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18116 2023-07-18 10:44:42.000000 promptwatch-0.2.8/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.254345 promptwatch-0.2.8/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.8/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13512 2023-07-27 08:01:44.000000 promptwatch-0.2.8/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.8/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13647 2023-08-04 12:50:12.000000 promptwatch-0.2.8/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.8/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-08-04 12:58:19.251296 promptwatch-0.2.8/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-08-04 12:58:19.000000 promptwatch-0.2.8/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-08-04 12:58:19.000000 promptwatch-0.2.8/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-08-04 12:58:19.000000 promptwatch-0.2.8/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.8/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-08-04 12:58:19.000000 promptwatch-0.2.8/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-08-04 12:58:19.000000 promptwatch-0.2.8/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.7/PKG-INFO` & `promptwatch-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.7
+Version: 0.2.8
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.7/README.md` & `promptwatch-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/setup.py` & `promptwatch-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/caching.py` & `promptwatch-0.2.8/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/client.py` & `promptwatch-0.2.8/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/data_model.py` & `promptwatch-0.2.8/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/decorators.py` & `promptwatch-0.2.8/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.8/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.8/src/promptwatch/langchain/langchain_support.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.8/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.8/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.8/src/promptwatch/unit_tests/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
             self.evaluate_result(generated)
         except Exception as e:
                 
             self.mark_as_failed(str(e))
             if "Missing some input keys:" in str(e):
                 # this is likely due to missing test memory...
-                raise Exception(f"Got exception {str(e)}. \nThis is likely due to missing test memory. Please see: docs.promptwatch.com/docs/unit_testing/unit_tests_reference_guide#langchain-test-memory")
+                raise Exception(f"Got exception {str(e)}. \nThis is likely due to missing test memory. Please see: docs.promptwatch.io/docs/unit_testing/unit_tests_reference_guide#langchain-test-memory")
             
             if not continue_on_error:
                 raise e
             
         self.iterations+=1
 
     def skip(self):
```

### Comparing `promptwatch-0.2.7/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.8/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.8/src/promptwatch/unit_tests/unit_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 
                 for line in f:
                     try:
                         data = json.loads(line)
                     except Exception as e:
                         raise Exception(f"Failed to parse line {line} in file {file_path}. Data are expected to be in json line format.\nError: {e}") 
                     
-                    test_case = TestCase(data)
+                    test_case = TestCase(**data)
                         
                     yield test_case
 
         self.test_cases_generator = iterate(file_path)
         self.conditions = PromptUnitTestConditions(for_test_cases_in_file=os.path.basename(file_path))
         return self
```

### Comparing `promptwatch-0.2.7/src/promptwatch/utils.py` & `promptwatch-0.2.8/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.7/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.8/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.7
+Version: 0.2.8
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.7/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.8/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

