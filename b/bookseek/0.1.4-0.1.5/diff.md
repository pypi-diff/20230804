# Comparing `tmp/bookseek-0.1.4.tar.gz` & `tmp/bookseek-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookseek-0.1.4.tar", last modified: Fri Aug  4 13:36:08 2023, max compression
+gzip compressed data, was "bookseek-0.1.5.tar", last modified: Fri Aug  4 13:37:37 2023, max compression
```

## Comparing `bookseek-0.1.4.tar` & `bookseek-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:36:08.893772 bookseek-0.1.4/
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:36:08.893772 bookseek-0.1.4/PKG-INFO
-drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:36:08.893772 bookseek-0.1.4/bookseek.egg-info/
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/PKG-INFO
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      202 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/SOURCES.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/dependency_links.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       43 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/entry_points.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       39 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/requires.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:36:08.000000 bookseek-0.1.4/bookseek.egg-info/top_level.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       38 2023-08-04 13:36:08.893772 bookseek-0.1.4/setup.cfg
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      871 2023-08-04 13:34:57.000000 bookseek-0.1.4/setup.py
+drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:37:37.502056 bookseek-0.1.5/
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:37:37.502056 bookseek-0.1.5/PKG-INFO
+drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:37:37.498056 bookseek-0.1.5/bookseek.egg-info/
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/PKG-INFO
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      202 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/SOURCES.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/dependency_links.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       52 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/entry_points.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       39 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/requires.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:37:37.000000 bookseek-0.1.5/bookseek.egg-info/top_level.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       38 2023-08-04 13:37:37.502056 bookseek-0.1.5/setup.cfg
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      880 2023-08-04 13:37:26.000000 bookseek-0.1.5/setup.py
```

