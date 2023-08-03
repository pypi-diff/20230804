# Comparing `tmp/table-out-0.0.1.tar.gz` & `tmp/table-out-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "table-out-0.0.1.tar", last modified: Thu Aug  3 21:42:29 2023, max compression
+gzip compressed data, was "table-out-0.0.2.tar", last modified: Thu Aug  3 22:01:40 2023, max compression
```

## Comparing `table-out-0.0.1.tar` & `table-out-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 21:42:29.883168 table-out-0.0.1/
--rw-rw-rw-   0        0        0      699 2023-08-03 21:42:29.883168 table-out-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 21:42:29.884168 table-out-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1150 2023-08-03 21:41:45.000000 table-out-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 21:42:29.872168 table-out-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 21:37:44.000000 table-out-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-08-03 21:31:26.000000 table-out-0.0.1/src/create_table.py
-drwxrwxrwx   0        0        0        0 2023-08-03 21:42:29.882168 table-out-0.0.1/table_out.egg-info/
--rw-rw-rw-   0        0        0      699 2023-08-03 21:42:29.000000 table-out-0.0.1/table_out.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-08-03 21:42:29.000000 table-out-0.0.1/table_out.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 21:42:29.000000 table-out-0.0.1/table_out.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-03 21:42:29.000000 table-out-0.0.1/table_out.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 22:01:40.993909 table-out-0.0.2/
+-rw-rw-rw-   0        0        0      642 2023-08-03 22:01:40.993909 table-out-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 22:01:40.993909 table-out-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-08-03 22:01:36.000000 table-out-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:01:40.982910 table-out-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 21:37:44.000000 table-out-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-08-03 21:31:26.000000 table-out-0.0.2/src/create_table.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:01:40.992908 table-out-0.0.2/table_out.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-08-03 22:01:40.000000 table-out-0.0.2/table_out.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-03 22:01:40.000000 table-out-0.0.2/table_out.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:01:40.000000 table-out-0.0.2/table_out.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 22:01:40.000000 table-out-0.0.2/table_out.egg-info/top_level.txt
```

### Comparing `table-out-0.0.1/setup.py` & `table-out-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Python package to create a table in the command line interface'
 LONG_DESCRIPTION = 'Table-Out is a Python package that allows you to create a table with values and display it in the command line interface. The package also allows the user to apply formatting to the table.'
 
 # Setting up
 setup(
         name="table-out", 
         version=VERSION,
@@ -15,14 +15,13 @@
         packages=find_packages(),
         install_requires=[], # add any additional packages that 
         # needs to be installed along with your package.
         
         keywords=['python', 'table-out'],
         classifiers= [
             "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
+            "Intended Audience :: Developers",
+            "License :: OSI Approved :: MIT License",
+            "Programming Language :: Python",
+            "Operating System :: OS Independent",
         ]
 )
```

### Comparing `table-out-0.0.1/src/create_table.py` & `table-out-0.0.2/src/create_table.py`

 * *Files identical despite different names*

