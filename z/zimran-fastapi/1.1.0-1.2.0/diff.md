# Comparing `tmp/zimran-fastapi-1.1.0.tar.gz` & `tmp/zimran-fastapi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-fastapi-1.1.0.tar", last modified: Tue Aug  1 19:36:32 2023, max compression
+gzip compressed data, was "zimran-fastapi-1.2.0.tar", last modified: Fri Aug  4 09:16:07 2023, max compression
```

## Comparing `zimran-fastapi-1.1.0.tar` & `zimran-fastapi-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/tests/test_check_trailing_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/tests/test_get_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/tests/test_health_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:36:32.342045 zimran-fastapi-1.1.0/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/zimran/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/zimran/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 19:36:23.000000 zimran-fastapi-1.1.0/zimran/fastapi/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:36:32.346045 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 19:36:32.000000 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-01 19:36:32.000000 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:36:32.000000 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 19:36:32.000000 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 19:36:32.000000 zimran-fastapi-1.1.0/zimran_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:16:07.308550 zimran-fastapi-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 09:16:07.308550 zimran-fastapi-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:16:07.308550 zimran-fastapi-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:16:07.304550 zimran-fastapi-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/tests/test_check_trailing_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/tests/test_get_application_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/tests/test_get_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/tests/test_health_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:16:07.304550 zimran-fastapi-1.2.0/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:16:07.304550 zimran-fastapi-1.2.0/zimran/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/zimran/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 09:15:58.000000 zimran-fastapi-1.2.0/zimran/fastapi/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:16:07.308550 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 09:16:07.000000 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-04 09:16:07.000000 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:16:07.000000 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 09:16:07.000000 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 09:16:07.000000 zimran-fastapi-1.2.0/zimran_fastapi.egg-info/top_level.txt
```

### Comparing `zimran-fastapi-1.1.0/setup.py` & `zimran-fastapi-1.2.0/setup.py`

 * *Files identical despite different names*

