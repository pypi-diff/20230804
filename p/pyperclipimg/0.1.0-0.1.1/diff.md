# Comparing `tmp/pyperclipimg-0.1.0.tar.gz` & `tmp/pyperclipimg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperclipimg-0.1.0.tar", last modified: Thu Aug  3 23:49:25 2023, max compression
+gzip compressed data, was "pyperclipimg-0.1.1.tar", last modified: Thu Aug  3 23:52:31 2023, max compression
```

## Comparing `pyperclipimg-0.1.0.tar` & `pyperclipimg-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 23:49:25.798457 pyperclipimg-0.1.0/
--rw-rw-rw-   0        0        0      657 2023-08-03 03:49:09.000000 pyperclipimg-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      903 2023-08-03 23:49:25.797465 pyperclipimg-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-08-03 03:47:51.000000 pyperclipimg-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 23:49:25.798457 pyperclipimg-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-08-03 22:54:09.000000 pyperclipimg-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 23:49:25.750162 pyperclipimg-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 23:49:25.764162 pyperclipimg-0.1.0/src/pyperclipimg/
--rw-rw-rw-   0        0        0     3685 2023-08-03 23:48:50.000000 pyperclipimg-0.1.0/src/pyperclipimg/__init__.py
--rw-rw-rw-   0        0        0       61 2023-08-03 03:49:09.000000 pyperclipimg-0.1.0/src/pyperclipimg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 23:49:25.789456 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/
--rw-rw-rw-   0        0        0      903 2023-08-03 23:49:25.000000 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-08-03 23:49:25.000000 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 23:49:25.000000 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-08-03 23:49:25.000000 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-03 23:49:25.000000 pyperclipimg-0.1.0/src/pyperclipimg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 23:49:25.794458 pyperclipimg-0.1.0/tests/
--rw-rw-rw-   0        0        0     2068 2023-08-03 23:42:46.000000 pyperclipimg-0.1.0/tests/test_pyperclipimg.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:52:31.480903 pyperclipimg-0.1.1/
+-rw-rw-rw-   0        0        0      657 2023-08-03 03:49:09.000000 pyperclipimg-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      903 2023-08-03 23:52:31.479918 pyperclipimg-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-08-03 03:47:51.000000 pyperclipimg-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 23:52:31.480903 pyperclipimg-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-08-03 23:52:02.000000 pyperclipimg-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:52:31.422894 pyperclipimg-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 23:52:31.436894 pyperclipimg-0.1.1/src/pyperclipimg/
+-rw-rw-rw-   0        0        0     3685 2023-08-03 23:52:24.000000 pyperclipimg-0.1.1/src/pyperclipimg/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-08-03 03:49:09.000000 pyperclipimg-0.1.1/src/pyperclipimg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 23:52:31.470915 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/
+-rw-rw-rw-   0        0        0      903 2023-08-03 23:52:31.000000 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-08-03 23:52:31.000000 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 23:52:31.000000 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-08-03 23:52:31.000000 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 23:52:31.000000 pyperclipimg-0.1.1/src/pyperclipimg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 23:52:31.476903 pyperclipimg-0.1.1/tests/
+-rw-rw-rw-   0        0        0     2068 2023-08-03 23:42:46.000000 pyperclipimg-0.1.1/tests/test_pyperclipimg.py
```

### Comparing `pyperclipimg-0.1.0/LICENSE` & `pyperclipimg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyperclipimg-0.1.0/PKG-INFO` & `pyperclipimg-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperclipimg
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cross-platform copy() and paste() Python functions for images.
 Home-page: https://github.com/asweigart/pyperclipimg
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyperclipimg-0.1.0/setup.py` & `pyperclipimg-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     description=("""Cross-platform copy() and paste() Python functions for images."""),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     test_suite="tests",
-    install_requires=['pyperclip',
-                      #'pillow>=9.4.0;platform_system=="Linux"',  # Linux is not yet supported.
+    install_requires=['pillow>=9.4.0;platform_system=="Linux"',
                       'pillow>=1.1.4;platform_system=="Windows"',
                       'pillow>=3.3.0;platform_system=="Darwin"',
                       'pyobjc-framework-quartz;platform_system=="Darwin"',
                       'pywin32;platform_system=="Windows"',
                       ],
     keywords="",
     classifiers=[
```

### Comparing `pyperclipimg-0.1.0/src/pyperclipimg/__init__.py` & `pyperclipimg-0.1.1/src/pyperclipimg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """pyperclipimg
 By Al Sweigart al@inventwithpython.com
 
 Cross-platform copy() and paste() Python functions for images."""
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import sys
 import subprocess
 import shutil
 import os
 import tempfile
 from pathlib import Path
```

### Comparing `pyperclipimg-0.1.0/src/pyperclipimg.egg-info/PKG-INFO` & `pyperclipimg-0.1.1/src/pyperclipimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperclipimg
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cross-platform copy() and paste() Python functions for images.
 Home-page: https://github.com/asweigart/pyperclipimg
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyperclipimg-0.1.0/tests/test_pyperclipimg.py` & `pyperclipimg-0.1.1/tests/test_pyperclipimg.py`

 * *Files identical despite different names*

