# Comparing `tmp/pomodoro-calculator-1.0.3.tar.gz` & `tmp/pomodoro-calculator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomodoro-calculator-1.0.3.tar", last modified: Fri Aug  4 11:47:46 2023, max compression
+gzip compressed data, was "pomodoro-calculator-1.0.4.tar", last modified: Fri Aug  4 11:50:55 2023, max compression
```

## Comparing `pomodoro-calculator-1.0.3.tar` & `pomodoro-calculator-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/
--rw-r--r--   0 matt      (1000) users      (985)      219 2018-09-13 07:34:42.000000 pomodoro-calculator-1.0.3/CONTRIBUTORS.txt
--rw-r--r--   0 matt      (1000) users      (985)      745 2023-08-04 11:42:18.000000 pomodoro-calculator-1.0.3/LICENCE
--rw-r--r--   0 matt      (1000) users      (985)       76 2014-06-11 23:56:28.000000 pomodoro-calculator-1.0.3/MANIFEST.in
--rw-r--r--   0 matt      (1000) users      (985)     3152 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)     2071 2023-08-04 11:41:44.000000 pomodoro-calculator-1.0.3/README.md
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/pomodoro_calculator/
--rw-r--r--   0 matt      (1000) users      (985)     6013 2023-08-04 11:45:40.000000 pomodoro-calculator-1.0.3/pomodoro_calculator/__init__.py
--rw-r--r--   0 matt      (1000) users      (985)     4846 2018-09-13 07:34:42.000000 pomodoro-calculator-1.0.3/pomodoro_calculator/main.py
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/pomodoro_calculator/test/
--rw-r--r--   0 matt      (1000) users      (985)        0 2014-06-10 13:37:09.000000 pomodoro-calculator-1.0.3/pomodoro_calculator/test/__init__.py
--rw-r--r--   0 matt      (1000) users      (985)    12540 2018-09-13 07:35:01.000000 pomodoro-calculator-1.0.3/pomodoro_calculator/test/test_main.py
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/
--rw-r--r--   0 matt      (1000) users      (985)     3152 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)      460 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) users      (985)        1 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) users      (985)       63 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) users      (985)       30 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) users      (985)       20 2023-08-04 11:47:46.000000 pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) users      (985)       67 2023-08-04 11:47:46.203408 pomodoro-calculator-1.0.3/setup.cfg
--rw-r--r--   0 matt      (1000) users      (985)     1651 2023-08-04 11:44:27.000000 pomodoro-calculator-1.0.3/setup.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/
+-rw-r--r--   0 matt      (1000) users      (985)      219 2018-09-13 07:34:42.000000 pomodoro-calculator-1.0.4/CONTRIBUTORS.txt
+-rw-r--r--   0 matt      (1000) users      (985)      745 2023-08-04 11:42:18.000000 pomodoro-calculator-1.0.4/LICENCE
+-rw-r--r--   0 matt      (1000) users      (985)       76 2014-06-11 23:56:28.000000 pomodoro-calculator-1.0.4/MANIFEST.in
+-rw-r--r--   0 matt      (1000) users      (985)     3156 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)     2075 2023-08-04 11:49:10.000000 pomodoro-calculator-1.0.4/README.md
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/pomodoro_calculator/
+-rw-r--r--   0 matt      (1000) users      (985)     6013 2023-08-04 11:50:02.000000 pomodoro-calculator-1.0.4/pomodoro_calculator/__init__.py
+-rw-r--r--   0 matt      (1000) users      (985)     4846 2018-09-13 07:34:42.000000 pomodoro-calculator-1.0.4/pomodoro_calculator/main.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/pomodoro_calculator/test/
+-rw-r--r--   0 matt      (1000) users      (985)        0 2014-06-10 13:37:09.000000 pomodoro-calculator-1.0.4/pomodoro_calculator/test/__init__.py
+-rw-r--r--   0 matt      (1000) users      (985)    12540 2018-09-13 07:35:01.000000 pomodoro-calculator-1.0.4/pomodoro_calculator/test/test_main.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/
+-rw-r--r--   0 matt      (1000) users      (985)     3156 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)      460 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) users      (985)       63 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) users      (985)       30 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) users      (985)       20 2023-08-04 11:50:55.000000 pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) users      (985)       67 2023-08-04 11:50:55.509148 pomodoro-calculator-1.0.4/setup.cfg
+-rw-r--r--   0 matt      (1000) users      (985)     1651 2023-08-04 11:44:27.000000 pomodoro-calculator-1.0.4/setup.py
```

### Comparing `pomodoro-calculator-1.0.3/LICENCE` & `pomodoro-calculator-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pomodoro-calculator-1.0.3/PKG-INFO` & `pomodoro-calculator-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomodoro-calculator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pretty command line tool to calculate the number of Pomodori available between two points in time.
 Home-page: https://codeberg.org/Dokana/Pomodoro-Calculator
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: ISC
 Keywords: pomodoro productivity timer freelance freelancing
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 points in time.
 
 ![Pomodoro Calculator screenshot](https://codeberg.org/Dokana/Pomodoro-Calculator/raw/branch/trunk/screenshot.png)
 
 
 ## Installation
 
-You can install the **Name of Thrones** using pip:
+You can install the **Pomodoro Calculator** using pip:
 
 ```console
     $ pip install pomodoro-calculator
 ```
 
 
 ## Usage
```

### Comparing `pomodoro-calculator-1.0.3/README.md` & `pomodoro-calculator-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 points in time.
 
 ![Pomodoro Calculator screenshot](https://codeberg.org/Dokana/Pomodoro-Calculator/raw/branch/trunk/screenshot.png)
 
 
 ## Installation
 
-You can install the **Name of Thrones** using pip:
+You can install the **Pomodoro Calculator** using pip:
 
 ```console
     $ pip install pomodoro-calculator
 ```
 
 
 ## Usage
```

### Comparing `pomodoro-calculator-1.0.3/pomodoro_calculator/__init__.py` & `pomodoro-calculator-1.0.4/pomodoro_calculator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A pretty command line tool to calculate the number
 of Pomodori available between two points in time.
 """
 __author__ = 'Matt Deacalion Stevens'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 import datetime
 from itertools import cycle
 
 
 class PomodoroCalculator:
     """
```

### Comparing `pomodoro-calculator-1.0.3/pomodoro_calculator/main.py` & `pomodoro-calculator-1.0.4/pomodoro_calculator/main.py`

 * *Files identical despite different names*

### Comparing `pomodoro-calculator-1.0.3/pomodoro_calculator/test/test_main.py` & `pomodoro-calculator-1.0.4/pomodoro_calculator/test/test_main.py`

 * *Files identical despite different names*

### Comparing `pomodoro-calculator-1.0.3/pomodoro_calculator.egg-info/PKG-INFO` & `pomodoro-calculator-1.0.4/pomodoro_calculator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomodoro-calculator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pretty command line tool to calculate the number of Pomodori available between two points in time.
 Home-page: https://codeberg.org/Dokana/Pomodoro-Calculator
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: ISC
 Keywords: pomodoro productivity timer freelance freelancing
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 points in time.
 
 ![Pomodoro Calculator screenshot](https://codeberg.org/Dokana/Pomodoro-Calculator/raw/branch/trunk/screenshot.png)
 
 
 ## Installation
 
-You can install the **Name of Thrones** using pip:
+You can install the **Pomodoro Calculator** using pip:
 
 ```console
     $ pip install pomodoro-calculator
 ```
 
 
 ## Usage
```

### Comparing `pomodoro-calculator-1.0.3/setup.py` & `pomodoro-calculator-1.0.4/setup.py`

 * *Files identical despite different names*

