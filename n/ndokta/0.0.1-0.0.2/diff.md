# Comparing `tmp/ndokta-0.0.1.tar.gz` & `tmp/ndokta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndokta-0.0.1.tar", last modified: Fri Aug  4 19:49:40 2023, max compression
+gzip compressed data, was "ndokta-0.0.2.tar", last modified: Fri Aug  4 20:33:29 2023, max compression
```

## Comparing `ndokta-0.0.1.tar` & `ndokta-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 kmarcini   (503) staff       (20)        0 2023-08-04 19:49:40.229026 ndokta-0.0.1/
--rw-r--r--   0 kmarcini   (503) staff       (20)      551 2023-08-04 19:49:40.228913 ndokta-0.0.1/PKG-INFO
-drwxr-xr-x   0 kmarcini   (503) staff       (20)        0 2023-08-04 19:49:40.228750 ndokta-0.0.1/ndokta.egg-info/
--rw-r--r--   0 kmarcini   (503) staff       (20)      551 2023-08-04 19:49:40.000000 ndokta-0.0.1/ndokta.egg-info/PKG-INFO
--rw-r--r--   0 kmarcini   (503) staff       (20)      157 2023-08-04 19:49:40.000000 ndokta-0.0.1/ndokta.egg-info/SOURCES.txt
--rw-r--r--   0 kmarcini   (503) staff       (20)        1 2023-08-04 19:49:40.000000 ndokta-0.0.1/ndokta.egg-info/dependency_links.txt
--rw-r--r--   0 kmarcini   (503) staff       (20)       32 2023-08-04 19:49:40.000000 ndokta-0.0.1/ndokta.egg-info/requires.txt
--rw-r--r--   0 kmarcini   (503) staff       (20)        1 2023-08-04 19:49:40.000000 ndokta-0.0.1/ndokta.egg-info/top_level.txt
--rw-r--r--   0 kmarcini   (503) staff       (20)       38 2023-08-04 19:49:40.229066 ndokta-0.0.1/setup.cfg
--rw-r--r--   0 kmarcini   (503) staff       (20)     1053 2023-08-04 19:49:07.000000 ndokta-0.0.1/setup.py
+drwxr-xr-x   0 kmarcini   (503) staff       (20)        0 2023-08-04 20:33:29.004026 ndokta-0.0.2/
+-rw-r--r--   0 kmarcini   (503) staff       (20)      551 2023-08-04 20:33:29.003911 ndokta-0.0.2/PKG-INFO
+drwxr-xr-x   0 kmarcini   (503) staff       (20)        0 2023-08-04 20:33:29.003736 ndokta-0.0.2/ndokta.egg-info/
+-rw-r--r--   0 kmarcini   (503) staff       (20)      551 2023-08-04 20:33:28.000000 ndokta-0.0.2/ndokta.egg-info/PKG-INFO
+-rw-r--r--   0 kmarcini   (503) staff       (20)      157 2023-08-04 20:33:28.000000 ndokta-0.0.2/ndokta.egg-info/SOURCES.txt
+-rw-r--r--   0 kmarcini   (503) staff       (20)        1 2023-08-04 20:33:28.000000 ndokta-0.0.2/ndokta.egg-info/dependency_links.txt
+-rw-r--r--   0 kmarcini   (503) staff       (20)       38 2023-08-04 20:33:28.000000 ndokta-0.0.2/ndokta.egg-info/requires.txt
+-rw-r--r--   0 kmarcini   (503) staff       (20)        1 2023-08-04 20:33:28.000000 ndokta-0.0.2/ndokta.egg-info/top_level.txt
+-rw-r--r--   0 kmarcini   (503) staff       (20)       38 2023-08-04 20:33:29.004072 ndokta-0.0.2/setup.cfg
+-rw-r--r--   0 kmarcini   (503) staff       (20)     1059 2023-08-04 20:32:05.000000 ndokta-0.0.2/setup.py
```

### Comparing `ndokta-0.0.1/PKG-INFO` & `ndokta-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndokta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Notre Dame Okta
 Home-page: UNKNOWN
 Author: Ken Marciniak
 Author-email: kmarcini@nd.edu
 License: UNKNOWN
 Keywords: python,okta,Notre Dame
 Platform: UNKNOWN
```

### Comparing `ndokta-0.0.1/ndokta.egg-info/PKG-INFO` & `ndokta-0.0.2/ndokta.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndokta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Notre Dame Okta
 Home-page: UNKNOWN
 Author: Ken Marciniak
 Author-email: kmarcini@nd.edu
 License: UNKNOWN
 Keywords: python,okta,Notre Dame
 Platform: UNKNOWN
```

### Comparing `ndokta-0.0.1/setup.py` & `ndokta-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Notre Dame Okta'
 LONG_DESCRIPTION = 'Wrapper calls for Okta API specific to Notre Dame'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ndokta", 
         version=VERSION,
         author="Ken Marciniak",
         author_email="kmarcini@nd.edu",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['requests','urllib3','boto3','botocore'], # add any additional packages that 
+        install_requires=['requests','urllib3<=1.27','boto3','botocore'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'okta', 'Notre Dame'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

