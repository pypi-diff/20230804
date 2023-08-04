# Comparing `tmp/SageLogger-1.5.tar.gz` & `tmp/SageLogger-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SageLogger-1.5.tar", last modified: Wed Aug  2 08:57:26 2023, max compression
+gzip compressed data, was "SageLogger-1.6.tar", last modified: Fri Aug  4 07:27:05 2023, max compression
```

## Comparing `SageLogger-1.5.tar` & `SageLogger-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:57:26.013739 SageLogger-1.5/
--rw-rw-rw-   0        0        0    12915 2023-08-02 08:57:26.013739 SageLogger-1.5/PKG-INFO
--rw-rw-rw-   0        0        0    12205 2023-08-02 08:54:53.000000 SageLogger-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 08:57:25.983862 SageLogger-1.5/SageLogger/
--rw-rw-rw-   0        0        0    13645 2023-08-02 08:53:19.000000 SageLogger-1.5/SageLogger/Logger.py
--rw-rw-rw-   0        0        0     1062 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/SageException.py
--rw-rw-rw-   0        0        0     3060 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/SageFactory.py
--rw-rw-rw-   0        0        0       15 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:57:25.987674 SageLogger-1.5/SageLogger.egg-info/
--rw-rw-rw-   0        0        0    12915 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 08:57:26.013739 SageLogger-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-08-02 08:55:39.000000 SageLogger-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:27:05.222589 SageLogger-1.6/
+-rw-rw-rw-   0        0        0    13042 2023-08-04 07:27:05.221570 SageLogger-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12328 2023-08-04 07:26:22.000000 SageLogger-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 07:27:05.188649 SageLogger-1.6/SageLogger/
+-rw-rw-rw-   0        0        0    13713 2023-08-02 09:35:01.000000 SageLogger-1.6/SageLogger/Logger.py
+-rw-rw-rw-   0        0        0     1062 2023-08-02 08:48:59.000000 SageLogger-1.6/SageLogger/SageException.py
+-rw-rw-rw-   0        0        0     3086 2023-08-02 09:31:47.000000 SageLogger-1.6/SageLogger/SageFactory.py
+-rw-rw-rw-   0        0        0       17 2023-08-02 09:34:16.000000 SageLogger-1.6/SageLogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:27:05.203601 SageLogger-1.6/SageLogger.egg-info/
+-rw-rw-rw-   0        0        0    13042 2023-08-04 07:27:04.000000 SageLogger-1.6/SageLogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-08-04 07:27:04.000000 SageLogger-1.6/SageLogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:27:04.000000 SageLogger-1.6/SageLogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 07:27:04.000000 SageLogger-1.6/SageLogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 07:27:04.000000 SageLogger-1.6/SageLogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:27:05.222589 SageLogger-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-08-04 07:26:41.000000 SageLogger-1.6/setup.py
```

### Comparing `SageLogger-1.5/PKG-INFO` & `SageLogger-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SageLogger
-Version: 1.5
+Version: 1.6
 Summary: Yet another python logger, or is it like any other?
 Home-page: https://github.com/PanSageYT/SageLogger
 Author: PanSageYT
 Author-email: pansage@hugedick.fyi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,18 @@
 ### Changelogs:
 v1.0 - Initial version
 v1.1 - Skipped as of a fail in version naming :(
 v1.2 - Skipped as of a fail in version naming :(
 v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
 v1.4 - Forced release because I forgot to change sample code from README.md
 v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
+v1.6 - Fixed ANSI coloring, removed auto name showing
+
+# Common errors:
+No colors just ANSI symbols? Use logger.fix_ansi()
 
 # -------------------------
 # SageLogger Documentation:
 # -------------------------
 #
 # SageFactory.py
```

### Comparing `SageLogger-1.5/README.md` & `SageLogger-1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 ### Changelogs:
 v1.0 - Initial version
 v1.1 - Skipped as of a fail in version naming :(
 v1.2 - Skipped as of a fail in version naming :(
 v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
 v1.4 - Forced release because I forgot to change sample code from README.md
 v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
+v1.6 - Fixed ANSI coloring, removed auto name showing
+
+# Common errors:
+No colors just ANSI symbols? Use logger.fix_ansi()
 
 # -------------------------
 # SageLogger Documentation:
 # -------------------------
 #
 # SageFactory.py
```

### Comparing `SageLogger-1.5/SageLogger/Logger.py` & `SageLogger-1.6/SageLogger/Logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import colorama
 import datetime
 import requests
 from typing import Union
 from enum import Enum
 import os
 from . import SageException, SageFactory
+from colorama import init
 
 thislogger = None
 
 class DynamicType:
     @staticmethod
     def fromChar(logger, char) -> tuple[int, str, bool]:
         #if len(char) != 1:
@@ -117,29 +118,33 @@
     customization : xxCustomization = None # type: ignore
     DynamicType = DynamicType()
     
     name = ""
     logfile = ""
     savetofile = True
     Type = xxType()
+
+    def fix_ansi(self):
+        init()
+
     def __init__(self, name : str = "", savetofile : bool = False, logfile : str = "log"):
         global thislogger
         if thislogger == None:
             thislogger = self
         self.customization = xxCustomization(logger=thislogger)
         self.Type.refresh(customization=self.customization)
         self.name = name
         self.logfile = logfile
         self.savetofile = savetofile
         if savetofile:
             with open(self.name + "." + self.logfile, "a") as wr:
                 wr.write(("-" * 16) + " " + datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S") + " " + ("-" * 16) + "\n")
                 wr.close()
     
-    def log(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET, showname : bool = True, ending : str = "\n"):
+    def log(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET, showname : bool = False, ending : str = "\n"):
         typefinish = None
         if(isinstance(type, xxPartType)):
             typefinish = (type.Id, type.customization, type.enabled)
         else:
             typefinish = type
         if not typefinish[2]:
             return
```

### Comparing `SageLogger-1.5/SageLogger/SageException.py` & `SageLogger-1.6/SageLogger/SageException.py`

 * *Files identical despite different names*

### Comparing `SageLogger-1.5/SageLogger/SageFactory.py` & `SageLogger-1.6/SageLogger/SageFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import Logger
 from typing import Union
+from colorama import init
 
 loggers = []
 
 def getLoggerByName(name: str) -> Union[Logger.SageConsoleLogger, Logger.SageRemoteLogger]:
     """
     Returns a logger object by name.
     :param name: The name of the logger to retrieve.
```

### Comparing `SageLogger-1.5/SageLogger.egg-info/PKG-INFO` & `SageLogger-1.6/SageLogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SageLogger
-Version: 1.5
+Version: 1.6
 Summary: Yet another python logger, or is it like any other?
 Home-page: https://github.com/PanSageYT/SageLogger
 Author: PanSageYT
 Author-email: pansage@hugedick.fyi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,18 @@
 ### Changelogs:
 v1.0 - Initial version
 v1.1 - Skipped as of a fail in version naming :(
 v1.2 - Skipped as of a fail in version naming :(
 v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
 v1.4 - Forced release because I forgot to change sample code from README.md
 v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
+v1.6 - Fixed ANSI coloring, removed auto name showing
+
+# Common errors:
+No colors just ANSI symbols? Use logger.fix_ansi()
 
 # -------------------------
 # SageLogger Documentation:
 # -------------------------
 #
 # SageFactory.py
```

### Comparing `SageLogger-1.5/setup.py` & `SageLogger-1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Dane projektu
 project_name = "SageLogger"
-project_version = "1.5"
+project_version = "1.6"
 project_description = "Yet another python logger, or is it like any other?"
 project_author = "PanSageYT"
 project_author_email = "pansage@hugedick.fyi"
 
 # Zależności
 dependencies = [
     "colorama",
```

