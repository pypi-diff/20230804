# Comparing `tmp/thslt-1.0.1.tar.gz` & `tmp/thslt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thslt-1.0.1.tar", last modified: Fri Aug  4 16:22:37 2023, max compression
+gzip compressed data, was "thslt-1.0.2.tar", last modified: Fri Aug  4 16:31:44 2023, max compression
```

## Comparing `thslt-1.0.1.tar` & `thslt-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.483991 thslt-1.0.1/
--rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5663 2023-08-04 16:22:37.479992 thslt-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5167 2023-08-04 16:11:45.000000 thslt-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 16:22:37.483991 thslt-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-08-04 16:21:54.000000 thslt-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.472992 thslt-1.0.1/thslt.egg-info/
--rw-rw-rw-   0        0        0     5663 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 16:22:36.000000 thslt-1.0.1/thslt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 16:22:37.476992 thslt-1.0.1/thst/
--rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.1/thst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.017707 thslt-1.0.2/
+-rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5665 2023-08-04 16:31:44.016703 thslt-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5169 2023-08-04 16:30:05.000000 thslt-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 16:31:44.018705 thslt-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-08-04 16:31:11.000000 thslt-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.010704 thslt-1.0.2/thslt.egg-info/
+-rw-rw-rw-   0        0        0     5665 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 16:31:43.000000 thslt-1.0.2/thslt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 16:31:44.013705 thslt-1.0.2/thst/
+-rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.2/thst/__init__.py
```

### Comparing `thslt-1.0.1/LICENSE.txt` & `thslt-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thslt-1.0.1/PKG-INFO` & `thslt-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Thai sign language translator (ThSLT) hslt
+# Thai sign language translator (ThSLT)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
 
 ## Description 
 This is a Thai sign language library for python used for translating Thai sign language into plain Thai characters. This library is used with [Mediapipe](https://developers.google.com/mediapipe) and [OpenCV](https://opencv.org/), so you should install those libraries first to make ThSLT function properly. Although the code works about 90% of the time, there are a lot of factors that you need to consider such as background , lighting , camera quality , hardware qualities. To increase the accuracy, you can adjust the <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_tracking_confidence</span> and <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_detection_confidence</span> from the default values.
 
 
 ## Table of Contents
@@ -38,15 +38,15 @@
  - To install Mediapipe, use the following command
 ```
 pip install mediapipe
 ```
 ### Use the following method to install ThSLT
  - To install ThSLT, use the following command
 ```
-pip install thslt
+pip install thslt==1.0.2
 ```
 ## Usage
 ### Here's an example setup for ThSLT:
 ```
 import thslt , cv2 
 import mediapipe as mp
```

### Comparing `thslt-1.0.1/README.md` & `thslt-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Thai sign language translator (ThSLT) hslt
+# Thai sign language translator (ThSLT)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
 
 ## Description 
 This is a Thai sign language library for python used for translating Thai sign language into plain Thai characters. This library is used with [Mediapipe](https://developers.google.com/mediapipe) and [OpenCV](https://opencv.org/), so you should install those libraries first to make ThSLT function properly. Although the code works about 90% of the time, there are a lot of factors that you need to consider such as background , lighting , camera quality , hardware qualities. To increase the accuracy, you can adjust the <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_tracking_confidence</span> and <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_detection_confidence</span> from the default values.
 
 
 ## Table of Contents
@@ -25,15 +25,15 @@
  - To install Mediapipe, use the following command
 ```
 pip install mediapipe
 ```
 ### Use the following method to install ThSLT
  - To install ThSLT, use the following command
 ```
-pip install thslt
+pip install thslt==1.0.2
 ```
 ## Usage
 ### Here's an example setup for ThSLT:
 ```
 import thslt , cv2 
 import mediapipe as mp
```

### Comparing `thslt-1.0.1/setup.py` & `thslt-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="thslt",
-    version="1.0.1",
+    version="1.0.2",
     author="Papangkon Ninarundech",
     author_email="papangkonsk@gmail.com",
     description="A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `thslt-1.0.1/thslt.egg-info/PKG-INFO` & `thslt-1.0.2/thslt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
 Author: Papangkon Ninarundech
 Author-email: papangkonsk@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Thai sign language translator (ThSLT) hslt
+# Thai sign language translator (ThSLT)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](#license)
 
 ## Description 
 This is a Thai sign language library for python used for translating Thai sign language into plain Thai characters. This library is used with [Mediapipe](https://developers.google.com/mediapipe) and [OpenCV](https://opencv.org/), so you should install those libraries first to make ThSLT function properly. Although the code works about 90% of the time, there are a lot of factors that you need to consider such as background , lighting , camera quality , hardware qualities. To increase the accuracy, you can adjust the <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_tracking_confidence</span> and <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">min_detection_confidence</span> from the default values.
 
 
 ## Table of Contents
@@ -38,15 +38,15 @@
  - To install Mediapipe, use the following command
 ```
 pip install mediapipe
 ```
 ### Use the following method to install ThSLT
  - To install ThSLT, use the following command
 ```
-pip install thslt
+pip install thslt==1.0.2
 ```
 ## Usage
 ### Here's an example setup for ThSLT:
 ```
 import thslt , cv2 
 import mediapipe as mp
```

### Comparing `thslt-1.0.1/thst/__init__.py` & `thslt-1.0.2/thst/__init__.py`

 * *Files identical despite different names*

