# Comparing `tmp/py-worksdone-utils-1.0.0.tar.gz` & `tmp/py-worksdone-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-worksdone-utils-1.0.0.tar", last modified: Fri Aug  4 06:37:42 2023, max compression
+gzip compressed data, was "py-worksdone-utils-1.0.1.tar", last modified: Fri Aug  4 06:41:01 2023, max compression
```

## Comparing `py-worksdone-utils-1.0.0.tar` & `py-worksdone-utils-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-04 06:07:10.000000 py-worksdone-utils-1.0.0/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:37:42.000000 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      385 2023-08-04 06:37:42.000000 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 06:37:42.000000 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       23 2023-08-04 06:37:42.000000 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 06:37:42.000000 py-worksdone-utils-1.0.0/py_worksdone_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/pyworksdoneutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      129 2023-08-04 06:34:02.000000 py-worksdone-utils-1.0.0/pyworksdoneutils/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/flask/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/flask/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3875 2023-08-04 06:37:33.000000 py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/flask/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 06:37:42.171508 py-worksdone-utils-1.0.0/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      647 2023-08-04 06:37:31.000000 py-worksdone-utils-1.0.0/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-04 06:07:10.000000 py-worksdone-utils-1.0.1/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:41:01.000000 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      385 2023-08-04 06:41:01.000000 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 06:41:01.000000 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       23 2023-08-04 06:41:01.000000 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 06:41:01.000000 py-worksdone-utils-1.0.1/py_worksdone_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/pyworksdoneutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:40:55.000000 py-worksdone-utils-1.0.1/pyworksdoneutils/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/flask/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       79 2023-08-04 06:40:55.000000 py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/flask/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3875 2023-08-04 06:37:33.000000 py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/flask/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 06:41:01.471508 py-worksdone-utils-1.0.1/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      647 2023-08-04 06:40:55.000000 py-worksdone-utils-1.0.1/setup.py
```

### Comparing `py-worksdone-utils-1.0.0/README.md` & `py-worksdone-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.0/pyworksdoneutils/keycloak/flask/_decorators.py` & `py-worksdone-utils-1.0.1/pyworksdoneutils/keycloak/flask/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.0/setup.py` & `py-worksdone-utils-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="py-worksdone-utils",
-    version="1.0.0",
+    version="1.0.1",
     author="KE",
     author_email="",
     description="Utilities with Keycloak",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["python-keycloak==3.3.0"],
     keywords=["python", "decorator", "token", "keycloak"],
```

