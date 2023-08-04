# Comparing `tmp/pyjt-0.4.1.tar.gz` & `tmp/pyjt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.4.1.tar", last modified: Fri Aug  4 11:59:48 2023, max compression
+gzip compressed data, was "pyjt-0.4.2.tar", last modified: Fri Aug  4 12:02:54 2023, max compression
```

## Comparing `pyjt-0.4.1.tar` & `pyjt-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:59:48.682231 pyjt-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 11:59:15.000000 pyjt-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-04 11:59:48.682231 pyjt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-04 11:59:15.000000 pyjt-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:59:48.678231 pyjt-0.4.1/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:59:48.678231 pyjt-0.4.1/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-04 11:59:48.000000 pyjt-0.4.1/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 11:59:48.000000 pyjt-0.4.1/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:59:48.000000 pyjt-0.4.1/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 11:59:48.000000 pyjt-0.4.1/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 11:59:48.000000 pyjt-0.4.1/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 11:59:15.000000 pyjt-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:59:48.682231 pyjt-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:59:48.682231 pyjt-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 11:59:15.000000 pyjt-0.4.1/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 11:59:15.000000 pyjt-0.4.1/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 11:59:15.000000 pyjt-0.4.1/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 11:59:15.000000 pyjt-0.4.1/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 11:59:15.000000 pyjt-0.4.1/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:02:54.431875 pyjt-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 12:02:21.000000 pyjt-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-04 12:02:54.431875 pyjt-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-04 12:02:21.000000 pyjt-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:02:54.431875 pyjt-0.4.2/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:02:54.431875 pyjt-0.4.2/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-04 12:02:54.000000 pyjt-0.4.2/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 12:02:54.000000 pyjt-0.4.2/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:02:54.000000 pyjt-0.4.2/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:02:54.000000 pyjt-0.4.2/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 12:02:54.000000 pyjt-0.4.2/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:02:21.000000 pyjt-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:02:54.431875 pyjt-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:02:54.431875 pyjt-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 12:02:21.000000 pyjt-0.4.2/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 12:02:21.000000 pyjt-0.4.2/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 12:02:21.000000 pyjt-0.4.2/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 12:02:21.000000 pyjt-0.4.2/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 12:02:21.000000 pyjt-0.4.2/tests/test_textfield.py
```

### Comparing `pyjt-0.4.1/LICENSE` & `pyjt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/PKG-INFO` & `pyjt-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.4.1
+Version: 0.4.2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,20 @@
 
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
+-   Install pyjt
+
+    pip3 install pyjt
+
+-   Start testing your app
+
     import pyjt
 
     pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
```

### Comparing `pyjt-0.4.1/README.md` & `pyjt-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
+-   Install pyjt
+
+    pip3 install pyjt
+
+-   Start testing your app
+
     import pyjt
 
     pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
```

### Comparing `pyjt-0.4.1/pyjt/ComponentFinder.py` & `pyjt-0.4.2/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/Fixture.py` & `pyjt-0.4.2/pyjt/Fixture.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/Frame.py` & `pyjt-0.4.2/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/Inspector.py` & `pyjt-0.4.2/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/Proxy.py` & `pyjt-0.4.2/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/Robot.py` & `pyjt-0.4.2/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt/__init__.py` & `pyjt-0.4.2/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/pyjt.egg-info/PKG-INFO` & `pyjt-0.4.2/pyjt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.4.1
+Version: 0.4.2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,20 @@
 
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
 ## Quickstart
 
+-   Install pyjt
+
+    pip3 install pyjt
+
+-   Start testing your app
+
     import pyjt
 
     pyjt.start()
     
     from javax.swing import JButton
 
     # start your java application here, in this case, we start
```

### Comparing `pyjt-0.4.1/pyproject.toml` & `pyjt-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.4.1"
+version = "0.4.2"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyjt-0.4.1/tests/test_locator.py` & `pyjt-0.4.2/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.1/tests/test_textfield.py` & `pyjt-0.4.2/tests/test_textfield.py`

 * *Files identical despite different names*

