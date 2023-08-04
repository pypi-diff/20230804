# Comparing `tmp/pyjt-0.4.3.tar.gz` & `tmp/pyjt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.4.3.tar", last modified: Fri Aug  4 12:13:15 2023, max compression
+gzip compressed data, was "pyjt-0.4.4.tar", last modified: Fri Aug  4 12:16:33 2023, max compression
```

## Comparing `pyjt-0.4.3.tar` & `pyjt-0.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:13:15.833027 pyjt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 12:12:42.000000 pyjt-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-04 12:13:15.833027 pyjt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-04 12:12:42.000000 pyjt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:13:15.833027 pyjt-0.4.3/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:13:15.833027 pyjt-0.4.3/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-04 12:13:15.000000 pyjt-0.4.3/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 12:13:15.000000 pyjt-0.4.3/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:13:15.000000 pyjt-0.4.3/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:13:15.000000 pyjt-0.4.3/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 12:13:15.000000 pyjt-0.4.3/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:12:42.000000 pyjt-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:13:15.833027 pyjt-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:13:15.833027 pyjt-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 12:12:42.000000 pyjt-0.4.3/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 12:12:42.000000 pyjt-0.4.3/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 12:12:42.000000 pyjt-0.4.3/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 12:12:42.000000 pyjt-0.4.3/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 12:12:42.000000 pyjt-0.4.3/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:16:33.357139 pyjt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 12:15:58.000000 pyjt-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-04 12:16:33.353139 pyjt-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-04 12:15:58.000000 pyjt-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:16:33.353139 pyjt-0.4.4/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:16:33.353139 pyjt-0.4.4/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-04 12:16:33.000000 pyjt-0.4.4/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-04 12:16:33.000000 pyjt-0.4.4/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:16:33.000000 pyjt-0.4.4/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:16:33.000000 pyjt-0.4.4/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 12:16:33.000000 pyjt-0.4.4/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:15:58.000000 pyjt-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:16:33.357139 pyjt-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:16:33.353139 pyjt-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 12:15:58.000000 pyjt-0.4.4/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 12:15:58.000000 pyjt-0.4.4/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 12:15:58.000000 pyjt-0.4.4/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 12:15:58.000000 pyjt-0.4.4/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 12:15:58.000000 pyjt-0.4.4/tests/test_textfield.py
```

### Comparing `pyjt-0.4.3/LICENSE` & `pyjt-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/README.md` & `pyjt-0.4.4/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-# pyjt - test java UI applications from python
+pyjt - test java UI applications from python
+============================================
 
 pyjt supports you testing java UI applications from python.
 
 Features:
 
 -   Thread safe call of java ui components
 -   Advanced locators to find ui compoments within the component tree
 -   Simulate real user interactions by mouse and keyboard
 
 This library makes use of **jpype** as the interface to the java
 virtual machine. It basicaly consists of helper functions to
 control the application from a test automation perspective.
 
-## Quickstart
+Quickstart
+----------
 
 -   Install pyjt
 
+.. code:: bash
+
         pip3 install pyjt
 
 -   Start testing your app
 
+.. code:: python
+
         import pyjt
 
         pyjt.start()
         
         from javax.swing import JButton
 
         # start your java application here, in this case, we start
@@ -39,10 +45,11 @@
 
         # Locate and fill text to an text field
         frame.locate(JTextField, name="textfield1").fill("John Smith")
 
         # Close the frame (application)
         frame.close()
 
-## Further documentation
+Further documentation
+---------------------
 
 Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.4.3/pyjt/ComponentFinder.py` & `pyjt-0.4.4/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/Fixture.py` & `pyjt-0.4.4/pyjt/Fixture.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/Frame.py` & `pyjt-0.4.4/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/Inspector.py` & `pyjt-0.4.4/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/Proxy.py` & `pyjt-0.4.4/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/Robot.py` & `pyjt-0.4.4/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyjt/__init__.py` & `pyjt-0.4.4/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/pyproject.toml` & `pyjt-0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.4.3"
+version = "0.4.4"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyjt-0.4.3/tests/test_locator.py` & `pyjt-0.4.4/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.3/tests/test_textfield.py` & `pyjt-0.4.4/tests/test_textfield.py`

 * *Files identical despite different names*

