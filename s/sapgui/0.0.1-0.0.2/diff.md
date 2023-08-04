# Comparing `tmp/sapgui-0.0.1.tar.gz` & `tmp/sapgui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapgui-0.0.1.tar", last modified: Fri Jul 28 09:55:07 2023, max compression
+gzip compressed data, was "sapgui-0.0.2.tar", last modified: Fri Aug  4 14:46:53 2023, max compression
```

## Comparing `sapgui-0.0.1.tar` & `sapgui-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:55:07.183031 sapgui-0.0.1/
--rw-rw-rw-   0        0        0      624 2023-07-28 09:55:07.183031 sapgui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-07-24 15:37:04.000000 sapgui-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 09:55:07.183031 sapgui-0.0.1/sapgui/
--rw-rw-rw-   0        0        0       60 2023-07-28 09:51:21.000000 sapgui-0.0.1/sapgui/__init__.py
--rw-rw-rw-   0        0        0     2864 2023-07-24 16:25:15.000000 sapgui-0.0.1/sapgui/sapgui.py
--rw-rw-rw-   0        0        0      947 2023-07-24 16:17:48.000000 sapgui-0.0.1/sapgui/sapguicode.py
-drwxrwxrwx   0        0        0        0 2023-07-28 09:55:07.183031 sapgui-0.0.1/sapgui.egg-info/
--rw-rw-rw-   0        0        0      624 2023-07-28 09:55:07.000000 sapgui-0.0.1/sapgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-28 09:55:07.000000 sapgui-0.0.1/sapgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:55:07.000000 sapgui-0.0.1/sapgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 09:55:07.000000 sapgui-0.0.1/sapgui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 09:55:07.198655 sapgui-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-07-28 09:54:04.000000 sapgui-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:53.915643 sapgui-0.0.2/
+-rw-rw-rw-   0        0        0      623 2023-08-04 14:46:53.915643 sapgui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-07-24 15:37:04.000000 sapgui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:53.905135 sapgui-0.0.2/sapgui/
+-rw-rw-rw-   0        0        0       60 2023-07-28 09:51:21.000000 sapgui-0.0.2/sapgui/__init__.py
+-rw-rw-rw-   0        0        0     3513 2023-07-28 16:23:28.000000 sapgui-0.0.2/sapgui/sapgui.py
+-rw-rw-rw-   0        0        0     1664 2023-07-28 15:37:25.000000 sapgui-0.0.2/sapgui/sapguicode.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:53.915643 sapgui-0.0.2/sapgui.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-08-04 14:46:53.000000 sapgui-0.0.2/sapgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-08-04 14:46:53.000000 sapgui-0.0.2/sapgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:46:53.000000 sapgui-0.0.2/sapgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 14:46:53.000000 sapgui-0.0.2/sapgui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:46:53.915643 sapgui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1068 2023-08-04 14:45:44.000000 sapgui-0.0.2/setup.py
```

### Comparing `sapgui-0.0.1/PKG-INFO` & `sapgui-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sapgui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to control SAP GUI scripting.
 Author: Piotr Kocemba
-Author-email: <kocembaPiotr@gmmail.com>
+Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sapgui-0.0.1/sapgui.egg-info/PKG-INFO` & `sapgui-0.0.2/sapgui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sapgui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to control SAP GUI scripting.
 Author: Piotr Kocemba
-Author-email: <kocembaPiotr@gmmail.com>
+Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sapgui-0.0.1/setup.py` & `sapgui-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python package to control SAP GUI scripting.'
 LONG_DESCRIPTION = '''Python package which gives user possibility to build his own
                       RPA base on SAP GUI.
                    '''
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="sapgui",
     version=VERSION,
     author="Piotr Kocemba",
-    author_email="<kocembaPiotr@gmmail.com>",
+    author_email="<KocembaPiotr@gmail.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'first package'],
```

