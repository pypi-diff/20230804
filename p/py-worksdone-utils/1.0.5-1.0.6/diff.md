# Comparing `tmp/py-worksdone-utils-1.0.5.tar.gz` & `tmp/py-worksdone-utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-worksdone-utils-1.0.5.tar", last modified: Fri Aug  4 12:53:59 2023, max compression
+gzip compressed data, was "py-worksdone-utils-1.0.6.tar", last modified: Fri Aug  4 12:57:10 2023, max compression
```

## Comparing `py-worksdone-utils-1.0.5.tar` & `py-worksdone-utils-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/
--rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-worksdone-utils-1.0.5/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:53:59.000000 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      520 2023-08-04 12:53:59.000000 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-08-04 12:53:59.000000 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       23 2023-08-04 12:53:59.000000 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-08-04 12:53:59.000000 py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/pyworksdoneutils/
--rw-r--r--   0 erne      (1000) erne      (1000)        2 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/
--rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/flask/
--rw-r--r--   0 erne      (1000) erne      (1000)       82 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/flask/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     3932 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/flask/_decorators.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/pyworksdoneutils/sqlalchemy/
--rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:57.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/sqlalchemy/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/pyworksdoneutils/sqlalchemy/flask/
--rw-r--r--   0 erne      (1000) erne      (1000)       37 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/sqlalchemy/flask/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     1226 2023-08-04 12:52:31.000000 py-worksdone-utils-1.0.5/pyworksdoneutils/sqlalchemy/flask/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-08-04 12:53:59.438512 py-worksdone-utils-1.0.5/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      647 2023-08-04 12:53:55.000000 py-worksdone-utils-1.0.5/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-worksdone-utils-1.0.6/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 12:57:10.000000 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      520 2023-08-04 12:57:10.000000 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-08-04 12:57:10.000000 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       23 2023-08-04 12:57:10.000000 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-08-04 12:57:10.000000 py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/pyworksdoneutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)        2 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       82 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     3932 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/flask/_decorators.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/pyworksdoneutils/sqlalchemy/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:57.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/sqlalchemy/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/pyworksdoneutils/sqlalchemy/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       37 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/sqlalchemy/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     1173 2023-08-04 12:55:57.000000 py-worksdone-utils-1.0.6/pyworksdoneutils/sqlalchemy/flask/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-08-04 12:57:10.078519 py-worksdone-utils-1.0.6/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      647 2023-08-04 12:57:02.000000 py-worksdone-utils-1.0.6/setup.py
```

### Comparing `py-worksdone-utils-1.0.5/README.md` & `py-worksdone-utils-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.5/py_worksdone_utils.egg-info/SOURCES.txt` & `py-worksdone-utils-1.0.6/py_worksdone_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.5/pyworksdoneutils/keycloak/flask/_decorators.py` & `py-worksdone-utils-1.0.6/pyworksdoneutils/keycloak/flask/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.5/setup.py` & `py-worksdone-utils-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="py-worksdone-utils",
-    version="1.0.5",
+    version="1.0.6",
     author="KE",
     author_email="",
     description="Utilities with Keycloak",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["python-keycloak==3.3.0"],
     keywords=["python", "decorator", "token", "keycloak"],
```

