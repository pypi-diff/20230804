# Comparing `tmp/pyloggor-1.1.4.tar.gz` & `tmp/pyloggor-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggor-1.1.4.tar", last modified: Sun Jun  4 19:46:17 2023, max compression
+gzip compressed data, was "pyloggor-1.1.5.tar", last modified: Fri Aug  4 21:17:28 2023, max compression
```

## Comparing `pyloggor-1.1.4.tar` & `pyloggor-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.266557 pyloggor-1.1.4/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-06-04 19:46:17.265771 pyloggor-1.1.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.258958 pyloggor-1.1.4/pyloggor/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.4/pyloggor/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7408 2023-06-04 19:45:36.000000 pyloggor-1.1.4/pyloggor/pyloggor.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.264333 pyloggor-1.1.4/pyloggor.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      196 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-04 19:46:17.266877 pyloggor-1.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      609 2023-06-04 19:45:11.000000 pyloggor-1.1.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 21:17:28.437269 pyloggor-1.1.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-08-04 21:17:28.436874 pyloggor-1.1.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.5/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 21:17:28.433821 pyloggor-1.1.5/pyloggor/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.5/pyloggor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7586 2023-08-04 21:07:37.000000 pyloggor-1.1.5/pyloggor/pyloggor.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 21:17:28.435928 pyloggor-1.1.5/pyloggor.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-08-04 21:17:28.000000 pyloggor-1.1.5/pyloggor.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      196 2023-08-04 21:17:28.000000 pyloggor-1.1.5/pyloggor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-08-04 21:17:28.000000 pyloggor-1.1.5/pyloggor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-08-04 21:17:28.000000 pyloggor-1.1.5/pyloggor.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-08-04 21:17:28.437527 pyloggor-1.1.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      609 2023-08-04 21:17:15.000000 pyloggor-1.1.5/setup.py
```

### Comparing `pyloggor-1.1.4/LICENSE` & `pyloggor-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.4/PKG-INFO` & `pyloggor-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.4
+Version: 1.1.5
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.4/README.md` & `pyloggor-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.4/pyloggor/pyloggor.py` & `pyloggor-1.1.5/pyloggor/pyloggor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 import os
 import threading
 import time
 from datetime import datetime
 from typing import Literal, Optional
+import os
 
 
 class FileHandler:
     def __init__(self, fn, log_freq):
         self.log_freq = log_freq
         self.fn = fn
         self.cache = []
@@ -99,14 +100,19 @@
             "DEBUG": 0,
             "INFO": 1,
             "WARNING": 2,
             "ERROR": 3,
             "CRITICAL": 4,
             "NOLOG": 5,
         }
+        if os.name == "nt":
+            import ctypes
+
+            kernel32 = ctypes.windll.kernel32
+            kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), 7)
 
     def extras_builder(self, extras):
         h = []
         for key, value in extras.items():
             h.append(f"{key}={value}")
         return f" {self.delim} ".join(h)
```

### Comparing `pyloggor-1.1.4/pyloggor.egg-info/PKG-INFO` & `pyloggor-1.1.5/pyloggor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.4
+Version: 1.1.5
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.4/setup.py` & `pyloggor-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name="pyloggor",
-    version="1.1.4",
+    version="1.1.5",
     description="An incredibly versatile yet simple logging system.",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/pyloggor",
     license="MIT",
     packages=["pyloggor"],
     long_description=open("README.md").read(),
```

