# Comparing `tmp/ientc_cognito_jwt-0.3.tar.gz` & `tmp/ientc_cognito_jwt-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ientc_cognito_jwt-0.3.tar", last modified: Fri Aug  4 16:13:18 2023, max compression
+gzip compressed data, was "ientc_cognito_jwt-0.4.tar", last modified: Fri Aug  4 16:22:31 2023, max compression
```

## Comparing `ientc_cognito_jwt-0.3.tar` & `ientc_cognito_jwt-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:13:18.863767 ientc_cognito_jwt-0.3/
--rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:13:18.863628 ientc_cognito_jwt-0.3/PKG-INFO
--rw-r--r--   0 jesuscc29   (501) staff       (20)      168 2023-08-04 15:46:38.000000 ientc_cognito_jwt-0.3/README.md
--rw-r--r--   0 jesuscc29   (501) staff       (20)     2750 2023-08-04 16:02:36.000000 ientc_cognito_jwt-0.3/cognito_jwt_utils.py
-drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:13:18.863446 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/
--rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:13:18.000000 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/PKG-INFO
--rw-r--r--   0 jesuscc29   (501) staff       (20)      243 2023-08-04 16:13:18.000000 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 16:13:18.000000 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)       18 2023-08-04 16:13:18.000000 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/requires.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 16:13:18.000000 ientc_cognito_jwt-0.3/ientc_cognito_jwt.egg-info/top_level.txt
--rw-r--r--   0 jesuscc29   (501) staff       (20)       38 2023-08-04 16:13:18.863814 ientc_cognito_jwt-0.3/setup.cfg
--rw-r--r--   0 jesuscc29   (501) staff       (20)      481 2023-08-04 16:11:49.000000 ientc_cognito_jwt-0.3/setup.py
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:22:31.952078 ientc_cognito_jwt-0.4/
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:22:31.951940 ientc_cognito_jwt-0.4/PKG-INFO
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      168 2023-08-04 15:46:38.000000 ientc_cognito_jwt-0.4/README.md
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       38 2023-08-04 16:22:31.952139 ientc_cognito_jwt-0.4/setup.cfg
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      483 2023-08-04 16:20:12.000000 ientc_cognito_jwt-0.4/setup.py
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:22:31.950095 ientc_cognito_jwt-0.4/src/
+drwxr-xr-x   0 jesuscc29   (501) staff       (20)        0 2023-08-04 16:22:31.951722 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      389 2023-08-04 16:22:31.000000 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 jesuscc29   (501) staff       (20)      242 2023-08-04 16:22:31.000000 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 16:22:31.000000 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)       18 2023-08-04 16:22:31.000000 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/requires.txt
+-rw-r--r--   0 jesuscc29   (501) staff       (20)        1 2023-08-04 16:22:31.000000 ientc_cognito_jwt-0.4/src/ientc_cognito_jwt.egg-info/top_level.txt
```

