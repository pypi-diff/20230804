# Comparing `tmp/loguru-logging-intercept-0.1.1.tar.gz` & `tmp/loguru-logging-intercept-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loguru-logging-intercept-0.1.1.tar", last modified: Sat Apr 10 21:55:33 2021, max compression
+gzip compressed data, was "loguru-logging-intercept-0.1.2.tar", last modified: Fri Aug  4 04:25:30 2023, max compression
```

## Comparing `loguru-logging-intercept-0.1.1.tar` & `loguru-logging-intercept-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2021-04-10 21:55:33.593371 loguru-logging-intercept-0.1.1/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      660 2021-04-10 21:55:33.593371 loguru-logging-intercept-0.1.1/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1079 2021-01-29 16:01:01.000000 loguru-logging-intercept-0.1.1/README.md
-drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2021-04-10 21:55:33.593371 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/
--rw-r--r--   0 matthew   (1000) matthew   (1000)      660 2021-04-10 21:55:33.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/PKG-INFO
--rw-r--r--   0 matthew   (1000) matthew   (1000)      285 2021-04-10 21:55:33.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/SOURCES.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2021-04-10 21:55:33.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/dependency_links.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)        7 2021-04-10 21:55:33.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/requires.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)       25 2021-04-10 21:55:33.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/top_level.txt
--rw-r--r--   0 matthew   (1000) matthew   (1000)     1096 2021-04-10 21:54:54.000000 loguru-logging-intercept-0.1.1/loguru_logging_intercept.py
--rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2021-04-10 21:55:33.593371 loguru-logging-intercept-0.1.1/setup.cfg
--rw-r--r--   0 matthew   (1000) matthew   (1000)      774 2021-04-10 21:55:03.000000 loguru-logging-intercept-0.1.1/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-08-04 04:25:30.236888 loguru-logging-intercept-0.1.2/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-08-04 04:23:26.000000 loguru-logging-intercept-0.1.2/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      626 2023-08-04 04:25:30.236888 loguru-logging-intercept-0.1.2/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1079 2023-08-04 04:23:26.000000 loguru-logging-intercept-0.1.2/README.md
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-08-04 04:25:30.236888 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      626 2023-08-04 04:25:30.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      293 2023-08-04 04:25:30.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-08-04 04:25:30.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-08-04 04:25:30.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       25 2023-08-04 04:25:30.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1114 2023-08-04 04:23:48.000000 loguru-logging-intercept-0.1.2/loguru_logging_intercept.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-08-04 04:25:30.236888 loguru-logging-intercept-0.1.2/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      774 2023-08-04 04:24:03.000000 loguru-logging-intercept-0.1.2/setup.py
```

### Comparing `loguru-logging-intercept-0.1.1/PKG-INFO` & `loguru-logging-intercept-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: loguru-logging-intercept
-Version: 0.1.1
+Version: 0.1.2
 Summary: Code to integrate Loguru with Python's standard logging module
 Home-page: https://github.com/MatthewScholefield/loguru-logging-intercept
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: loguru logging intercept
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

### Comparing `loguru-logging-intercept-0.1.1/README.md` & `loguru-logging-intercept-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `loguru-logging-intercept-0.1.1/loguru_logging_intercept.egg-info/PKG-INFO` & `loguru-logging-intercept-0.1.2/loguru_logging_intercept.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: loguru-logging-intercept
-Version: 0.1.1
+Version: 0.1.2
 Summary: Code to integrate Loguru with Python's standard logging module
 Home-page: https://github.com/MatthewScholefield/loguru-logging-intercept
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: loguru logging intercept
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
```

### Comparing `loguru-logging-intercept-0.1.1/loguru_logging_intercept.py` & `loguru-logging-intercept-0.1.2/loguru_logging_intercept.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         frame, depth = logging.currentframe(), 2
         while frame.f_code.co_filename == logging.__file__:  # noqa: WPS609
             frame = cast(FrameType, frame.f_back)
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(
             level,
+            "{}",
             record.getMessage(),
         )
 
 
 def setup_loguru_logging_intercept(
     level=logging.DEBUG, modules=()
 ):
```

### Comparing `loguru-logging-intercept-0.1.1/setup.py` & `loguru-logging-intercept-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='loguru-logging-intercept',
-    version='0.1.1',
+    version='0.1.2',
     description='Code to integrate Loguru with Python\'s standard logging module',
     url='https://github.com/MatthewScholefield/loguru-logging-intercept',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

