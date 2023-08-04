# Comparing `tmp/robotframework-requestspro-1.1.8.tar.gz` & `tmp/robotframework-requestspro-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotframework-requestspro-1.1.8.tar", last modified: Sat Feb 27 08:07:24 2021, max compression
+gzip compressed data, was "robotframework-requestspro-1.1.9.tar", last modified: Fri Aug  4 03:55:32 2023, max compression
```

## Comparing `robotframework-requestspro-1.1.8.tar` & `robotframework-requestspro-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2021-02-27 08:07:24.040617 robotframework-requestspro-1.1.8/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2020-12-03 08:08:58.000000 robotframework-requestspro-1.1.8/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      702 2021-02-27 08:07:24.039855 robotframework-requestspro-1.1.8/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2020-12-03 08:08:58.000000 robotframework-requestspro-1.1.8/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2020-12-20 04:48:41.000000 robotframework-requestspro-1.1.8/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2021-02-27 08:07:24.040846 robotframework-requestspro-1.1.8/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2020-12-19 22:51:28.000000 robotframework-requestspro-1.1.8/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2021-02-27 08:07:24.028413 robotframework-requestspro-1.1.8/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2021-02-27 08:07:24.035346 robotframework-requestspro-1.1.8/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1169 2021-02-27 08:06:12.000000 robotframework-requestspro-1.1.8/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2020-12-20 21:29:02.000000 robotframework-requestspro-1.1.8/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2020-12-03 08:08:58.000000 robotframework-requestspro-1.1.8/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2020-12-03 08:08:58.000000 robotframework-requestspro-1.1.8/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2021-02-27 08:05:20.000000 robotframework-requestspro-1.1.8/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2021-02-27 08:07:24.038755 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      702 2021-02-27 08:07:23.000000 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      507 2021-02-27 08:07:23.000000 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2021-02-27 08:07:23.000000 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2021-02-27 08:07:23.000000 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2021-02-27 08:07:23.000000 robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.797522 robotframework-requestspro-1.1.9/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 03:55:32.797394 robotframework-requestspro-1.1.9/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-04 03:55:32.797567 robotframework-requestspro-1.1.9/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.794977 robotframework-requestspro-1.1.9/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.796632 robotframework-requestspro-1.1.9/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2274 2023-08-04 03:48:18.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-04 03:33:25.000000 robotframework-requestspro-1.1.9/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-04 03:55:32.797190 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-04 03:55:32.000000 robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.1.8/PKG-INFO` & `robotframework-requestspro-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.1.8
+Version: 1.1.9
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
-Description: Robot Framework keyword library wrapper around the HTTP client library requests.
 Keywords: robotframework testing test automation http client requests
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
+License-File: LICENSE
+
+Robot Framework keyword library wrapper around the HTTP client library requests.
+
```

### Comparing `robotframework-requestspro-1.1.8/setup.py` & `robotframework-requestspro-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.8/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.1.9/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.8/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.1.9/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.1.8/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.1.9/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.1.8
+Version: 1.1.9
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
-Description: Robot Framework keyword library wrapper around the HTTP client library requests.
 Keywords: robotframework testing test automation http client requests
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
+License-File: LICENSE
+
+Robot Framework keyword library wrapper around the HTTP client library requests.
+
```

