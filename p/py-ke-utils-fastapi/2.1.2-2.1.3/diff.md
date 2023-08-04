# Comparing `tmp/py-ke-utils-fastapi-2.1.2.tar.gz` & `tmp/py-ke-utils-fastapi-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ke-utils-fastapi-2.1.2.tar", last modified: Fri Aug  4 09:54:53 2023, max compression
+gzip compressed data, was "py-ke-utils-fastapi-2.1.3.tar", last modified: Fri Aug  4 09:56:36 2023, max compression
```

## Comparing `py-ke-utils-fastapi-2.1.2.tar` & `py-ke-utils-fastapi-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6383 2023-04-11 16:05:08.000000 py-ke-utils-fastapi-2.1.2/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:54:53.000000 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      415 2023-08-04 09:54:53.000000 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 09:54:53.000000 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       43 2023-08-04 09:54:53.000000 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 09:54:53.000000 py-ke-utils-fastapi-2.1.2/py_ke_utils_fastapi.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:13:01.000000 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/keycloak/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       76 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/keycloak/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3223 2023-08-04 09:54:44.000000 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/keycloak/_keycloak_auth.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/redis/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       49 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/redis/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     5056 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/redis/_auth_deco.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 09:54:53.161508 py-ke-utils-fastapi-2.1.2/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      728 2023-08-04 09:54:51.000000 py-ke-utils-fastapi-2.1.2/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6383 2023-04-11 16:05:08.000000 py-ke-utils-fastapi-2.1.3/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      415 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       43 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:13:01.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       76 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3220 2023-08-04 09:56:26.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/_keycloak_auth.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       49 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     5056 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/_auth_deco.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      728 2023-08-04 09:56:29.000000 py-ke-utils-fastapi-2.1.3/setup.py
```

### Comparing `py-ke-utils-fastapi-2.1.2/README.md` & `py-ke-utils-fastapi-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/keycloak/_keycloak_auth.py` & `py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/_keycloak_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from typing import Annotated
 
 import requests
-from fastapi.responses import JSONResponse
 from fastapi import Header, Depends, HTTPException
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 from keycloak import KeycloakOpenID, KeycloakError
 from requests import HTTPError
 
 security = HTTPBearer()
 
@@ -87,8 +86,10 @@
             logging.info(
                 f"Successfully checked permissions. Response - {response.json()}"
             )
         except HTTPError as err:
             logging.error(
                 f"Error: {err.response.json()} Status code: {err.response.status_code}"
             )
-            raise JSONResponse(content=err.response.json(), status_code=err.response.status_code)
+            raise HTTPException(
+                status_code=err.response.status_code, detail=err.response.json()
+            ) from err
```

### Comparing `py-ke-utils-fastapi-2.1.2/pykeutilsfastapi/redis/_auth_deco.py` & `py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/_auth_deco.py`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-2.1.2/setup.py` & `py-ke-utils-fastapi-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "2.1.2"
+VERSION = "2.1.3"
 DESCRIPTION = "Utilities for FastAPI"
 
 # Setting up
 setup(
     name="py-ke-utils-fastapi",
     version=VERSION,
     author="KE",
```

