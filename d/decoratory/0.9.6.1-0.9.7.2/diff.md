# Comparing `tmp/decoratory-0.9.6.1.tar.gz` & `tmp/decoratory-0.9.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.6.1.tar", last modified: Tue Jul 18 17:55:12 2023, max compression
+gzip compressed data, was "decoratory-0.9.7.2.tar", last modified: Thu Aug  3 22:50:47 2023, max compression
```

## Comparing `decoratory-0.9.6.1.tar` & `decoratory-0.9.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.706859 decoratory-0.9.6.1/
--rw-rw-rw-   0        0        0     1262 2023-07-18 17:13:50.000000 decoratory-0.9.6.1/License.txt
--rw-rw-rw-   0        0        0    48576 2023-07-18 17:55:12.705803 decoratory-0.9.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    46879 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.6.1/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 17:55:11.821074 decoratory-0.9.6.1/Sources/
-drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.251697 decoratory-0.9.6.1/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.6.1/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7627 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5893 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    19694 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12476 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36921 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     8187 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10871 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.336816 decoratory-0.9.6.1/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    48576 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.640119 decoratory-0.9.6.1/Unittest/
--rw-rw-rw-   0        0        0    28998 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23872 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40073 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10743 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10207 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-07-18 17:55:12.707861 decoratory-0.9.6.1/setup.cfg
--rw-rw-rw-   0        0        0     4715 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:50:47.302423 decoratory-0.9.7.2/
+-rw-rw-rw-   0        0        0     1265 2023-07-28 17:31:04.000000 decoratory-0.9.7.2/License.txt
+-rw-rw-rw-   0        0        0    48644 2023-08-03 22:50:47.302423 decoratory-0.9.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    46895 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.7.2/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 22:50:46.692354 decoratory-0.9.7.2/Sources/
+drwxrwxrwx   0        0        0        0 2023-08-03 22:50:46.992443 decoratory-0.9.7.2/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.7.2/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7633 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5899 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    19700 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12482 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36927 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     8193 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10877 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:50:47.042437 decoratory-0.9.7.2/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48644 2023-08-03 22:50:46.000000 decoratory-0.9.7.2/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-08-03 22:50:46.000000 decoratory-0.9.7.2/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:50:46.000000 decoratory-0.9.7.2/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 22:50:46.000000 decoratory-0.9.7.2/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 22:50:47.252413 decoratory-0.9.7.2/Unittest/
+-rw-rw-rw-   0        0        0    29004 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23878 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40079 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10749 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10213 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 22:50:47.302423 decoratory-0.9.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     4760 2023-08-03 22:50:10.000000 decoratory-0.9.7.2/setup.py
```

### Comparing `decoratory-0.9.6.1/License.txt` & `decoratory-0.9.7.2/License.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============================================================================
 MIT License
 ===============================================================================
 
-Copyright 2020-2023, Martin Abel, eVation
+© Copyright 2020-2023, Martin Abel, eVation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoratory-0.9.6.1/PKG-INFO` & `decoratory-0.9.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.6.1
-Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/index.html
-Download-URL: http://evation.eu/Section/Download.html
+Version: 0.9.7.2
+Summary: Decorators: Singleton, SemiSingleton, Multiton, Observer, Observable, generic Wrapper.
+Home-page: https://decoratory.app/index.html
+Download-URL: https://decoratory.app/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://decoratory.de/index.html
-Project-URL: Release Notes, http://evation.eu/Section/ReleaseNotes.html
-Project-URL: Download, http://evation.eu/Section/Download.html
-Keywords: decorator singleton multiton observer observable wrapper
+Project-URL: Projekt, https://decoratory.app/index.html
+Project-URL: Release Notes, https://decoratory.app/Section/ReleaseNotes.html
+Project-URL: Download, https://decoratory.app/Section/Download.html
+Keywords: decorator semi-singleton singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -39,27 +39,27 @@
 
 
 .. _top:
 
 ..  --------------------------------------------------------------------------
     Documentation for the decoratory package
     --------------------------------------------------------------------------
-    __title__ = "Readme"
+    __title__ = "Decoratory"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+    __url__ = "https://decoratory.app"
+    __copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
     __created__ = "2020-01-01"
-    __version__ = "0.9.6.1"
-    __date__ = "2023-07-18"
-    __time__ = "19:54:26"
+    __version__ = "0.9.7.2"
+    __date__ = "2023-08-04"
+    __time__ = "00:50:09"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1174,14 +1174,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://decoratory.de/
+.. _project homepage: https://decoratory.app/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://decoratory.de/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://decoratory.de/Section/Decorators.html
+.. _Decorator Arguments Template: https://decoratory.app/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: https://decoratory.app/Section/Decorators.html
```

### Comparing `decoratory-0.9.6.1/Readme.rst` & `decoratory-0.9.7.2/Readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 .. _top:
 
 ..  --------------------------------------------------------------------------
     Documentation for the decoratory package
     --------------------------------------------------------------------------
-    __title__ = "Readme"
+    __title__ = "Decoratory"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+    __url__ = "https://decoratory.app"
+    __copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
     __created__ = "2020-01-01"
-    __version__ = "0.9.6.1"
-    __date__ = "2023-07-18"
-    __time__ = "19:54:26"
+    __version__ = "0.9.7.2"
+    __date__ = "2023-08-04"
+    __time__ = "00:50:09"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1135,14 +1135,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://decoratory.de/
+.. _project homepage: https://decoratory.app/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://decoratory.de/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://decoratory.de/Section/Decorators.html
+.. _Decorator Arguments Template: https://decoratory.app/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: https://decoratory.app/Section/Decorators.html
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/__main__.py` & `decoratory-0.9.7.2/Sources/decoratory/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Decoratory"
 __module__ = "__main__.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/banner.py` & `decoratory-0.9.7.2/Sources/decoratory/banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Banner"
 __module__ = "banner.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/basic.py` & `decoratory-0.9.7.2/Sources/decoratory/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,20 @@
 __title__ = "Basic"
 __module__ = "basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X", "BaseDecorator"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/multiton.py` & `decoratory-0.9.7.2/Sources/decoratory/multiton.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,20 +122,20 @@
 __title__ = "Multiton"
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/observer.py` & `decoratory-0.9.7.2/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,20 +404,20 @@
 __title__ = "Observer"
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/singleton.py` & `decoratory-0.9.7.2/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 __title__ = "Singleton"
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory/wrapper.py` & `decoratory-0.9.7.2/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,20 @@
 __title__ = "Wrapper"
 __module__ = "wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.7.2/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.6.1
-Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu/index.html
-Download-URL: http://evation.eu/Section/Download.html
+Version: 0.9.7.2
+Summary: Decorators: Singleton, SemiSingleton, Multiton, Observer, Observable, generic Wrapper.
+Home-page: https://decoratory.app/index.html
+Download-URL: https://decoratory.app/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
-Project-URL: Projekt, http://decoratory.de/index.html
-Project-URL: Release Notes, http://evation.eu/Section/ReleaseNotes.html
-Project-URL: Download, http://evation.eu/Section/Download.html
-Keywords: decorator singleton multiton observer observable wrapper
+Project-URL: Projekt, https://decoratory.app/index.html
+Project-URL: Release Notes, https://decoratory.app/Section/ReleaseNotes.html
+Project-URL: Download, https://decoratory.app/Section/Download.html
+Keywords: decorator semi-singleton singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -39,27 +39,27 @@
 
 
 .. _top:
 
 ..  --------------------------------------------------------------------------
     Documentation for the decoratory package
     --------------------------------------------------------------------------
-    __title__ = "Readme"
+    __title__ = "Decoratory"
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
-    __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+    __url__ = "https://decoratory.app"
+    __copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
     __created__ = "2020-01-01"
-    __version__ = "0.9.6.1"
-    __date__ = "2023-07-18"
-    __time__ = "19:54:26"
+    __version__ = "0.9.7.2"
+    __date__ = "2023-08-04"
+    __time__ = "00:50:09"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -1174,14 +1174,14 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://decoratory.de/
+.. _project homepage: https://decoratory.app/
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://decoratory.de/Section/ArgumentsTemplate.html
-.. _Decorator Implementations: http://decoratory.de/Section/Decorators.html
+.. _Decorator Arguments Template: https://decoratory.app/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: https://decoratory.app/Section/Decorators.html
```

### Comparing `decoratory-0.9.6.1/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.7.2/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.6.1/Unittest/test_basic.py` & `decoratory-0.9.7.2/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test_Basic"
 __module__ = "test_basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.6.1/Unittest/test_multiton.py` & `decoratory-0.9.7.2/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Multiton"
 __module__ = "test_multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.6.1/Unittest/test_observer.py` & `decoratory-0.9.7.2/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Observer"
 __module__ = "test_observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.6.1/Unittest/test_singleton.py` & `decoratory-0.9.7.2/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Singleton"
 __module__ = "test_singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.6.1/Unittest/test_wrapper.py` & `decoratory-0.9.7.2/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 __title__ = "Test Wrapper"
 __module__ = "test_wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.6.1/setup.py` & `decoratory-0.9.7.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 __title__ = "decoratory"
 __module__ = "setup.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
-__url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
+__url__ = "https://decoratory.app"
+__copyright__ = f"(c) Copyright 2020-2023, {__author__}, {__company__}."
 __created__ = "2020-01-01"
-__version__ = "0.9.6.1"
-__date__ = "2023-07-18"
-__time__ = "19:54:26"
+__version__ = "0.9.7.2"
+__date__ = "2023-08-04"
+__time__ = "00:50:09"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -30,97 +30,107 @@
 
 # -----------------------------------------------------------------------------
 # Parameters
 src = "Sources"
 dta = join("lib", "site-packages", __title__, "data")
 tst = join("lib", "site-packages", __title__, "tests")
 
-with open("Readme.rst", "r") as f:
+with open("Readme.rst") as f:
     description = f.read()
 
-with open("Requirements.txt", "r") as f:
+with open("Requirements.txt") as f:
     requirements = [str(req) for req in f.read().splitlines() if req]
 
 
 def version_check():
     """Keep versions in sync"""
     try:
         # noinspection PyProtectedMember
         from Sources.decoratory.__main__ import __version__ as version
+
         assert version == __version__, (
             f"\n\n{'':=^79s}\n"
             f"{' Version problem: __main__.version != setup.version ':=^79s}\n"
-            f"{'':=^79s}")
+            f"{'':=^79s}"
+        )
     except (ModuleNotFoundError, ImportError):
         pass  # Let the AssertionError pass...
 
 
 # -----------------------------------------------------------------------------
 # Excecute
 setupargs = dict(
     # General
     name=__title__,
     version=__version__,
     author=__author__,
-    author_email=f'{__author__} <{__email__}>',
-    maintainer=f'{__author__}',
-    maintainer_email=f'{__author__} <{__email__}>',
+    author_email=f"{__author__} <{__email__}>",
+    maintainer=f"{__author__}",
+    maintainer_email=f"{__author__} <{__email__}>",
     url="/".join([__url__, "index.html"]),
     download_url="/".join([__url__, "Section", "Download.html"]),
-    description=('Decorators: Singleton, Multiton, Observer, Observable, '
-                 'generic Wrapper.'),
+    description=(
+        "Decorators: Singleton, SemiSingleton, Multiton, Observer, "
+        "Observable, generic Wrapper."
+    ),
     long_description=description,
-    long_description_content_type='text/x-rst',
+    long_description_content_type="text/x-rst",
     project_urls={
-        'Projekt': "/".join(["http://decoratory.de", "index.html"]),
-        'Release Notes': "/".join(
-            [__url__, "Section", "ReleaseNotes.html"]),
-        'Download': "/".join(
-            [__url__, "Section", "Download.html"])},
-    keywords='decorator singleton multiton observer observable wrapper',
+        "Projekt": "/".join(["https://decoratory.app", "index.html"]),
+        "Release Notes": "/".join([__url__, "Section", "ReleaseNotes.html"]),
+        "Download": "/".join([__url__, "Section", "Download.html"]),
+    },
+    keywords="decorator semi-singleton singleton multiton "
+    "observer observable wrapper",
     # Technical
     license=__license__,
-    platforms=['Operating System :: OS Independent'],
+    platforms=["Operating System :: OS Independent"],
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Information Technology',
-        'Natural Language :: English',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Education',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Utilities'],
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Information Technology",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Education",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Utilities",
+    ],
     # Modules, Files and Data
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
     packages=find_packages(where=src),
     package_dir={"": src},
     package_data={},
     py_modules=[],
-    data_files=[(dta, ["License.txt",
-                       "Readme.rst",
-                       "Requirements.txt"]),
-                (tst, ["Unittest/test_basic.py",
-                       "Unittest/test_singleton.py",
-                       "Unittest/test_multiton.py",
-                       "Unittest/test_wrapper.py",
-                       "Unittest/test_observer.py"])],
+    data_files=[
+        (dta, ["License.txt", "Readme.rst", "Requirements.txt"]),
+        (
+            tst,
+            [
+                "Unittest/test_basic.py",
+                "Unittest/test_singleton.py",
+                "Unittest/test_multiton.py",
+                "Unittest/test_wrapper.py",
+                "Unittest/test_observer.py",
+            ],
+        ),
+    ],
     entry_points={},
     # Dependencies
-    python_requires='>=3.7',
+    python_requires=">=3.7",
     setup_requires=[],
     install_requires=requirements,
     # Post install
     # cmdclass={'install': CustomInstall},
 )
 setup(**setupargs)
```

