# Comparing `tmp/pkoffice-0.0.1.tar.gz` & `tmp/pkoffice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkoffice-0.0.1.tar", last modified: Fri Aug  4 15:34:44 2023, max compression
+gzip compressed data, was "pkoffice-0.0.2.tar", last modified: Fri Aug  4 15:50:21 2023, max compression
```

## Comparing `pkoffice-0.0.1.tar` & `pkoffice-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 15:34:44.183703 pkoffice-0.0.1/
--rw-rw-rw-   0        0        0      588 2023-08-04 15:34:44.183703 pkoffice-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-08-04 15:20:45.000000 pkoffice-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 15:34:44.183703 pkoffice-0.0.1/pkoffice.egg-info/
--rw-rw-rw-   0        0        0      588 2023-08-04 15:34:44.000000 pkoffice-0.0.1/pkoffice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-08-04 15:34:44.000000 pkoffice-0.0.1/pkoffice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 15:34:44.000000 pkoffice-0.0.1/pkoffice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-04 15:34:44.000000 pkoffice-0.0.1/pkoffice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 15:34:44.000000 pkoffice-0.0.1/pkoffice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 15:34:44.183703 pkoffice-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-08-04 15:33:26.000000 pkoffice-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:50:21.608867 pkoffice-0.0.2/
+-rw-rw-rw-   0        0        0      588 2023-08-04 15:50:21.608867 pkoffice-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-04 15:20:45.000000 pkoffice-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 15:50:21.608867 pkoffice-0.0.2/pkoffice.egg-info/
+-rw-rw-rw-   0        0        0      588 2023-08-04 15:50:21.000000 pkoffice-0.0.2/pkoffice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-08-04 15:50:21.000000 pkoffice-0.0.2/pkoffice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 15:50:21.000000 pkoffice-0.0.2/pkoffice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 15:50:21.000000 pkoffice-0.0.2/pkoffice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 15:50:21.608867 pkoffice-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-08-04 15:50:14.000000 pkoffice-0.0.2/setup.py
```

### Comparing `pkoffice-0.0.1/PKG-INFO` & `pkoffice-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkoffice
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to manage office tools.
 Author: Piotr Kocemba
 Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,office,sql,excel,outlook
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pkoffice-0.0.1/pkoffice.egg-info/PKG-INFO` & `pkoffice-0.0.2/pkoffice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkoffice
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package to manage office tools.
 Author: Piotr Kocemba
 Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,office,sql,excel,outlook
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pkoffice-0.0.1/setup.py` & `pkoffice-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python package to manage office tools.'
 LONG_DESCRIPTION = '''Python package which will simplify usage of main office tools.
                    '''
 
 # Setting up
 setup(
     name="pkoffice",
     version=VERSION,
     author="Piotr Kocemba",
     author_email="<KocembaPiotr@gmail.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['sqlalchemy','pandas'],
+    install_requires=[],
     keywords=['python', 'office', 'sql', 'excel', 'outlook'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
```

