# Comparing `tmp/py-worksdone-utils-1.0.3.tar.gz` & `tmp/py-worksdone-utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-worksdone-utils-1.0.3.tar", last modified: Fri Aug  4 06:57:22 2023, max compression
+gzip compressed data, was "py-worksdone-utils-1.0.4.tar", last modified: Fri Aug  4 12:26:21 2023, max compression
```

## Comparing `py-worksdone-utils-1.0.3.tar` & `py-worksdone-utils-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-04 06:07:10.000000 py-worksdone-utils-1.0.3/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      385 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       23 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        2 2023-08-04 06:45:17.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       81 2023-08-04 06:57:10.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3932 2023-08-04 06:56:52.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      647 2023-08-04 06:57:21.000000 py-worksdone-utils-1.0.3/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-worksdone-utils-1.0.4/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:26:21.000000 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      520 2023-08-04 12:26:21.000000 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-08-04 12:26:21.000000 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       23 2023-08-04 12:26:21.000000 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-08-04 12:26:21.000000 py-worksdone-utils-1.0.4/py_worksdone_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/pyworksdoneutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)        2 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       82 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     3932 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/flask/_decorators.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/pyworksdoneutils/sqlalchemy/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:57.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/sqlalchemy/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/pyworksdoneutils/sqlalchemy/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       37 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/sqlalchemy/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     1181 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.4/pyworksdoneutils/sqlalchemy/flask/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-08-04 12:26:21.778524 py-worksdone-utils-1.0.4/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      647 2023-08-04 12:26:09.000000 py-worksdone-utils-1.0.4/setup.py
```

### Comparing `py-worksdone-utils-1.0.3/README.md` & `py-worksdone-utils-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/_decorators.py` & `py-worksdone-utils-1.0.4/pyworksdoneutils/keycloak/flask/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.3/setup.py` & `py-worksdone-utils-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="py-worksdone-utils",
-    version="1.0.3",
+    version="1.0.4",
     author="KE",
     author_email="",
     description="Utilities with Keycloak",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["python-keycloak==3.3.0"],
     keywords=["python", "decorator", "token", "keycloak"],
```

