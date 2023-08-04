# Comparing `tmp/RWAPIMicroservicePython-2.0.0.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-2.0.0.tar", last modified: Thu Jan 19 05:58:54 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0rc2.tar", last modified: Fri Aug  4 10:34:22 2023, max compression
```

## Comparing `RWAPIMicroservicePython-2.0.0.tar` & `RWAPIMicroservicePython-3.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-2.0.0/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      274 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2321 2021-06-24 15:27:40.000000 RWAPIMicroservicePython-2.0.0/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2554 2021-06-15 15:48:01.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      243 2019-10-28 16:32:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/errors.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      274 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      376 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      206 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      844 2023-01-19 05:30:39.000000 RWAPIMicroservicePython-2.0.0/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 10:34:22.013671 RWAPIMicroservicePython-3.0.0rc2/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0rc2/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 10:34:22.013671 RWAPIMicroservicePython-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     5996 2023-08-04 09:48:11.000000 RWAPIMicroservicePython-3.0.0rc2/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 10:34:22.010337 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     7070 2023-08-04 10:29:47.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/main.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2079 2023-08-03 13:19:32.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython/test_utils.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 10:34:22.013671 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 10:34:22.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-04 10:34:22.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-04 10:34:22.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-04 10:34:22.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-04 10:34:22.000000 RWAPIMicroservicePython-3.0.0rc2/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-04 10:34:22.013671 RWAPIMicroservicePython-3.0.0rc2/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      886 2023-08-04 10:34:01.000000 RWAPIMicroservicePython-3.0.0rc2/setup.py
```

### Comparing `RWAPIMicroservicePython-2.0.0/LICENSE` & `RWAPIMicroservicePython-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

