# Comparing `tmp/py-worksdone-utils-1.0.2.tar.gz` & `tmp/py-worksdone-utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-worksdone-utils-1.0.2.tar", last modified: Fri Aug  4 06:45:38 2023, max compression
+gzip compressed data, was "py-worksdone-utils-1.0.3.tar", last modified: Fri Aug  4 06:57:22 2023, max compression
```

## Comparing `py-worksdone-utils-1.0.2.tar` & `py-worksdone-utils-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-04 06:07:10.000000 py-worksdone-utils-1.0.2/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:45:38.000000 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      385 2023-08-04 06:45:38.000000 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 06:45:38.000000 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       23 2023-08-04 06:45:38.000000 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 06:45:38.000000 py-worksdone-utils-1.0.2/py_worksdone_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/pyworksdoneutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        2 2023-08-04 06:45:17.000000 py-worksdone-utils-1.0.2/pyworksdoneutils/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/flask/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       80 2023-08-04 06:45:37.000000 py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/flask/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3875 2023-08-04 06:37:33.000000 py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/flask/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 06:45:38.961508 py-worksdone-utils-1.0.2/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      647 2023-08-04 06:45:37.000000 py-worksdone-utils-1.0.2/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-04 06:07:10.000000 py-worksdone-utils-1.0.3/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      420 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      385 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       23 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 06:57:22.000000 py-worksdone-utils-1.0.3/py_worksdone_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        2 2023-08-04 06:45:17.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:08:21.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       81 2023-08-04 06:57:10.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3932 2023-08-04 06:56:52.000000 py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 06:57:22.601508 py-worksdone-utils-1.0.3/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      647 2023-08-04 06:57:21.000000 py-worksdone-utils-1.0.3/setup.py
```

### Comparing `py-worksdone-utils-1.0.2/README.md` & `py-worksdone-utils-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.2/pyworksdoneutils/keycloak/flask/_decorators.py` & `py-worksdone-utils-1.0.3/pyworksdoneutils/keycloak/flask/_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                     server_url=server_url,
                     client_id=client_id,
                     realm_name=subdomain,
                     client_secret_key=client_secret_key,
                 )
                 token = token.replace("Bearer ", "")
                 oidc.userinfo(token)
+                logging.info("Successfully authorized")
                 return org_function(*args, **kwargs)
             except KeycloakError as e:
                 logging.error(f"Error: {e.__doc__} Status code: {e.response_code}")
                 return {
                     "statusCode": e.response_code,
                     "message": e.__doc__,
                 }, e.response_code
```

### Comparing `py-worksdone-utils-1.0.2/setup.py` & `py-worksdone-utils-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="py-worksdone-utils",
-    version="1.0.2",
+    version="1.0.3",
     author="KE",
     author_email="",
     description="Utilities with Keycloak",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["python-keycloak==3.3.0"],
     keywords=["python", "decorator", "token", "keycloak"],
```

