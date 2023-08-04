# Comparing `tmp/IOmatchbox-0.2.tar.gz` & `tmp/IOmatchbox-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOmatchbox-0.2.tar", last modified: Fri Aug  4 14:18:37 2023, max compression
+gzip compressed data, was "IOmatchbox-0.21.tar", last modified: Fri Aug  4 14:25:41 2023, max compression
```

## Comparing `IOmatchbox-0.2.tar` & `IOmatchbox-0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:18:37.687335 IOmatchbox-0.2/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.2/LICENSE
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4101 2023-08-04 14:18:37.687335 IOmatchbox-0.2/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)     3195 2023-08-04 14:14:48.000000 IOmatchbox-0.2/README.md
--rw-r--r--   0 yfo       (1000) yfo       (1000)      950 2023-08-04 14:09:30.000000 IOmatchbox-0.2/pyproject.toml
--rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-04 14:18:37.687335 IOmatchbox-0.2/setup.cfg
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:18:37.685335 IOmatchbox-0.2/src/
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:18:37.686335 IOmatchbox-0.2/src/IOmatchbox/
--rw-r--r--   0 yfo       (1000) yfo       (1000)    15618 2023-08-04 14:07:41.000000 IOmatchbox-0.2/src/IOmatchbox/IOTEC.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)    24106 2023-08-04 13:51:01.000000 IOmatchbox-0.2/src/IOmatchbox/IOmatchbox.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 IOmatchbox-0.2/src/IOmatchbox/__init__.py
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:18:37.687335 IOmatchbox-0.2/src/IOmatchbox.egg-info/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4101 2023-08-04 14:18:37.000000 IOmatchbox-0.2/src/IOmatchbox.egg-info/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-04 14:18:37.000000 IOmatchbox-0.2/src/IOmatchbox.egg-info/SOURCES.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-04 14:18:37.000000 IOmatchbox-0.2/src/IOmatchbox.egg-info/dependency_links.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-04 14:18:37.000000 IOmatchbox-0.2/src/IOmatchbox.egg-info/top_level.txt
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.668922 IOmatchbox-0.21/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.21/LICENSE
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-04 14:25:41.668922 IOmatchbox-0.21/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     3195 2023-08-04 14:14:48.000000 IOmatchbox-0.21/README.md
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      951 2023-08-04 14:25:25.000000 IOmatchbox-0.21/pyproject.toml
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-04 14:25:41.668922 IOmatchbox-0.21/setup.cfg
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.666922 IOmatchbox-0.21/src/
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.667922 IOmatchbox-0.21/src/IOmatchbox/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    15624 2023-08-04 14:24:28.000000 IOmatchbox-0.21/src/IOmatchbox/IOTEC.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    24106 2023-08-04 13:51:01.000000 IOmatchbox-0.21/src/IOmatchbox/IOmatchbox.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 IOmatchbox-0.21/src/IOmatchbox/__init__.py
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.667922 IOmatchbox-0.21/src/IOmatchbox.egg-info/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/top_level.txt
```

### Comparing `IOmatchbox-0.2/LICENSE` & `IOmatchbox-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.2/PKG-INFO` & `IOmatchbox-0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.2
+Version: 0.21
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `IOmatchbox-0.2/README.md` & `IOmatchbox-0.21/README.md`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.2/pyproject.toml` & `IOmatchbox-0.21/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "IOmatchbox"
-version = "0.2"
+version = "0.21"
 authors = [
   { name="iancynk", email="ian.cynk@posteo.eu" },
 ]
 description = "Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `IOmatchbox-0.2/src/IOmatchbox/IOTEC.py` & `IOmatchbox-0.21/src/IOmatchbox/IOTEC.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             print('unknown reply:', reply)
         return
     
     
     # --------------------------------------------------------------------------
     # serial functions
     
-    def openTEC(port=''):
+    def openTEC(self, port=''):
         """create a serial connection with the recommended parameters
         if no port is given the function will try all available serial ports
         and check whether the connected device has an ID like an IO laser. 
         """
         self.ser = serial.Serial()
         self.ser.baudrate = 115200
         self.ser.bytesize = serial.EIGHTBITS
```

### Comparing `IOmatchbox-0.2/src/IOmatchbox/IOmatchbox.py` & `IOmatchbox-0.21/src/IOmatchbox/IOmatchbox.py`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.2/src/IOmatchbox.egg-info/PKG-INFO` & `IOmatchbox-0.21/src/IOmatchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.2
+Version: 0.21
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

