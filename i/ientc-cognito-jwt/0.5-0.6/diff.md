# Comparing `tmp/ientc_cognito_jwt-0.5.tar.gz` & `tmp/ientc_cognito_jwt-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ientc_cognito_jwt-0.5.tar", last modified: Fri Aug  4 16:57:10 2023, max compression
+gzip compressed data, was "ientc_cognito_jwt-0.6.tar", last modified: Fri Aug  4 17:06:13 2023, max compression
```

## Comparing `ientc_cognito_jwt-0.5.tar` & `ientc_cognito_jwt-0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:57:10.577668 ientc_cognito_jwt-0.5/
--rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:57:10.577537 ientc_cognito_jwt-0.5/PKG-INFO
--rw-r--r--   0 jesuscc29   (501) staff       (20)      168 2023-08-04 15:46:38.000000 ientc_cognito_jwt-0.5/README.md
-drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:57:10.576826 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/
--rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:57:10.000000 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/PKG-INFO
--rw-r--r--   0 jesuscc29   (501) staff       (20)      263 2023-08-04 16:57:10.000000 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 16:57:10.000000 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)       18 2023-08-04 16:57:10.000000 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/requires.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)        4 2023-08-04 16:57:10.000000 ientc_cognito_jwt-0.5/ientc_cognito_jwt.egg-info/top_level.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)       38 2023-08-04 16:57:10.577721 ientc_cognito_jwt-0.5/setup.cfg
--rw-r--r--   0 jesuscc29   (501) staff       (20)      509 2023-08-04 16:56:23.000000 ientc_cognito_jwt-0.5/setup.py
-drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:57:10.577158 ientc_cognito_jwt-0.5/src/
--rw-r--r--   0 jesuscc29   (501) staff       (20)       53 2023-08-04 16:56:37.000000 ientc_cognito_jwt-0.5/src/__init__.py
--rw-r--r--   0 jesuscc29   (501) staff       (20)     2750 2023-08-04 16:02:36.000000 ientc_cognito_jwt-0.5/src/cognito_jwt_utils.py
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 17:06:13.813796 ientc_cognito_jwt-0.6/
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      426 2023-08-04 17:06:13.812744 ientc_cognito_jwt-0.6/PKG-INFO
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      168 2023-08-04 15:46:38.000000 ientc_cognito_jwt-0.6/README.md
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       38 2023-08-04 17:06:13.814064 ientc_cognito_jwt-0.6/setup.cfg
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      483 2023-08-04 17:05:30.000000 ientc_cognito_jwt-0.6/setup.py
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 17:06:13.808429 ientc_cognito_jwt-0.6/src/
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 17:06:13.809726 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt/
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       53 2023-08-04 17:05:35.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt/__init__.py
+-rw-r--r--   0 jesuscc29   (501) staff       (20)     2750 2023-08-04 16:02:36.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt/cognito_jwt_utils.py
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 17:06:13.812170 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      426 2023-08-04 17:06:13.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      319 2023-08-04 17:06:13.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 17:06:13.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       18 2023-08-04 17:06:13.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/requires.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       18 2023-08-04 17:06:13.000000 ientc_cognito_jwt-0.6/src/ientc_cognito_jwt.egg-info/top_level.txt
```

### Comparing `ientc_cognito_jwt-0.5/src/cognito_jwt_utils.py` & `ientc_cognito_jwt-0.6/src/ientc_cognito_jwt/cognito_jwt_utils.py`

 * *Files identical despite different names*

