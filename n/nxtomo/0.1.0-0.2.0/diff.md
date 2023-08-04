# Comparing `tmp/nxtomo-0.1.0.tar.gz` & `tmp/nxtomo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxtomo-0.1.0.tar", last modified: Fri Aug  4 13:00:41 2023, max compression
+gzip compressed data, was "nxtomo-0.2.0.tar", last modified: Fri Aug  4 14:17:47 2023, max compression
```

## Comparing `nxtomo-0.1.0.tar` & `nxtomo-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.869856 nxtomo-0.1.0/
--rw-r--r--   0 payno     (1000) payno     (1000)     1266 2023-08-04 08:57:20.000000 nxtomo-0.1.0/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 13:00:41.869856 nxtomo-0.1.0/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      187 2023-08-04 12:40:29.000000 nxtomo-0.1.0/README.md
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo/
--rw-r--r--   0 payno     (1000) payno     (1000)      103 2023-08-04 12:59:35.000000 nxtomo-0.1.0/nxtomo/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo/application/
--rw-r--r--   0 payno     (1000) payno     (1000)    27566 2023-08-04 12:10:38.000000 nxtomo-0.1.0/nxtomo/application/nxtomo.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo/application/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    15705 2023-08-04 12:43:37.000000 nxtomo-0.1.0/nxtomo/application/test/test_nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8666 2023-08-04 12:27:55.000000 nxtomo-0.1.0/nxtomo/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo/nxobject/
--rw-r--r--   0 payno     (1000) payno     (1000)      224 2023-08-04 12:09:44.000000 nxtomo-0.1.0/nxtomo/nxobject/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    37499 2023-08-04 12:37:48.000000 nxtomo-0.1.0/nxtomo/nxobject/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7097 2023-08-04 12:18:01.000000 nxtomo-0.1.0/nxtomo/nxobject/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3391 2023-08-04 12:17:45.000000 nxtomo-0.1.0/nxtomo/nxobject/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12997 2023-08-04 12:37:48.000000 nxtomo-0.1.0/nxtomo/nxobject/nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9619 2023-08-04 12:15:33.000000 nxtomo-0.1.0/nxtomo/nxobject/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6243 2023-08-04 12:16:39.000000 nxtomo-0.1.0/nxtomo/nxobject/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9437 2023-08-04 12:17:10.000000 nxtomo-0.1.0/nxtomo/nxobject/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo/nxobject/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    14717 2023-08-04 12:10:45.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1336 2023-08-04 12:10:48.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1073 2023-08-04 12:10:51.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2705 2023-08-04 12:10:55.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2077 2023-08-04 12:10:58.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1128 2023-08-04 12:11:01.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5155 2023-08-04 12:11:04.000000 nxtomo-0.1.0/nxtomo/nxobject/test/test_nxtransformations.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3591 2023-08-04 12:37:48.000000 nxtomo-0.1.0/nxtomo/nxobject/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.869856 nxtomo-0.1.0/nxtomo/paths/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1242 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      481 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      319 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      826 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      343 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11848 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)      543 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.869856 nxtomo-0.1.0/nxtomo/paths/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     6691 2023-08-04 08:15:45.000000 nxtomo-0.1.0/nxtomo/paths/test/test_backward_compatibility.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.869856 nxtomo-0.1.0/nxtomo/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)       34 2023-08-04 12:05:19.000000 nxtomo-0.1.0/nxtomo/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15108 2023-08-04 12:37:48.000000 nxtomo-0.1.0/nxtomo/utils/frameappender.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1990 2023-08-04 12:27:23.000000 nxtomo-0.1.0/nxtomo/utils/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.869856 nxtomo-0.1.0/nxtomo/utils/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     7636 2023-08-04 08:15:53.000000 nxtomo-0.1.0/nxtomo/utils/test/test_transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20767 2023-08-04 12:21:10.000000 nxtomo-0.1.0/nxtomo/utils/transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4082 2023-08-04 12:21:27.000000 nxtomo-0.1.0/nxtomo/utils/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)       18 2023-08-04 12:59:59.000000 nxtomo-0.1.0/nxtomo/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 13:00:41.865856 nxtomo-0.1.0/nxtomo.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 13:00:41.000000 nxtomo-0.1.0/nxtomo.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     1286 2023-08-04 13:00:41.000000 nxtomo-0.1.0/nxtomo.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-04 13:00:41.000000 nxtomo-0.1.0/nxtomo.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-08-04 13:00:41.000000 nxtomo-0.1.0/nxtomo.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       11 2023-08-04 13:00:41.000000 nxtomo-0.1.0/nxtomo.egg-info/top_level.txt
--rw-r--r--   0 payno     (1000) payno     (1000)     2060 2023-08-04 12:59:55.000000 nxtomo-0.1.0/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 13:00:41.869856 nxtomo-0.1.0/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 12:40:53.000000 nxtomo-0.1.0/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1266 2023-08-04 08:57:20.000000 nxtomo-0.2.0/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 14:17:47.883110 nxtomo-0.2.0/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      187 2023-08-04 12:40:29.000000 nxtomo-0.2.0/README.md
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/
+-rw-r--r--   0 payno     (1000) payno     (1000)      103 2023-08-04 13:11:37.000000 nxtomo-0.2.0/nxtomo/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/application/
+-rw-r--r--   0 payno     (1000) payno     (1000)    27475 2023-08-04 13:11:48.000000 nxtomo-0.2.0/nxtomo/application/nxtomo.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/application/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    16816 2023-08-04 13:29:54.000000 nxtomo-0.2.0/nxtomo/application/test/test_nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8666 2023-08-04 12:27:55.000000 nxtomo-0.2.0/nxtomo/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/nxobject/
+-rw-r--r--   0 payno     (1000) payno     (1000)      224 2023-08-04 12:09:44.000000 nxtomo-0.2.0/nxtomo/nxobject/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    37631 2023-08-04 13:17:20.000000 nxtomo-0.2.0/nxtomo/nxobject/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7106 2023-08-04 13:13:10.000000 nxtomo-0.2.0/nxtomo/nxobject/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3391 2023-08-04 12:17:45.000000 nxtomo-0.2.0/nxtomo/nxobject/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12997 2023-08-04 12:37:48.000000 nxtomo-0.2.0/nxtomo/nxobject/nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9619 2023-08-04 12:15:33.000000 nxtomo-0.2.0/nxtomo/nxobject/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6252 2023-08-04 13:13:19.000000 nxtomo-0.2.0/nxtomo/nxobject/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9446 2023-08-04 13:13:26.000000 nxtomo-0.2.0/nxtomo/nxobject/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/nxobject/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    14678 2023-08-04 14:15:03.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1333 2023-08-04 13:34:34.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1077 2023-08-04 13:35:22.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2706 2023-08-04 13:15:03.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2076 2023-08-04 13:35:34.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1127 2023-08-04 13:35:43.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5146 2023-08-04 14:15:06.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxtransformations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3588 2023-08-04 13:35:20.000000 nxtomo-0.2.0/nxtomo/nxobject/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/paths/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1242 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      481 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      319 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      826 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      343 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11877 2023-08-04 13:36:04.000000 nxtomo-0.2.0/nxtomo/paths/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      543 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/paths/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     6676 2023-08-04 13:33:31.000000 nxtomo-0.2.0/nxtomo/paths/test/test_backward_compatibility.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)       34 2023-08-04 12:05:19.000000 nxtomo-0.2.0/nxtomo/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15108 2023-08-04 13:35:54.000000 nxtomo-0.2.0/nxtomo/utils/frameappender.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1990 2023-08-04 12:27:23.000000 nxtomo-0.2.0/nxtomo/utils/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/utils/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     7620 2023-08-04 14:15:09.000000 nxtomo-0.2.0/nxtomo/utils/test/test_transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20767 2023-08-04 12:21:10.000000 nxtomo-0.2.0/nxtomo/utils/transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3720 2023-08-04 13:05:11.000000 nxtomo-0.2.0/nxtomo/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       18 2023-08-04 14:16:59.000000 nxtomo-0.2.0/nxtomo/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     1286 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       22 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     2060 2023-08-04 12:59:55.000000 nxtomo-0.2.0/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 14:17:47.883110 nxtomo-0.2.0/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 12:40:53.000000 nxtomo-0.2.0/setup.py
```

### Comparing `nxtomo-0.1.0/LICENSE` & `nxtomo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/PKG-INFO` & `nxtomo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 0.1.0
+Version: 0.2.0
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-0.1.0/nxtomo/application/nxtomo.py` & `nxtomo-0.2.0/nxtomo/application/nxtomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,38 +6,30 @@
 from operator import is_not
 from typing import Optional, Union
 
 import h5py
 import numpy
 from silx.io.url import DataUrl
 from silx.utils.proxy import docstring
-from silx.utils.enum import Enum as _Enum
+
+from pyunitsystem.energysystem import EnergySI
+
 from nxtomo.io import HDF5File
 from nxtomo.paths.nxtomo import LATEST_VERSION as LATEST_NXTOMO_VERSION
 from nxtomo.paths.nxtomo import get_paths as get_nexus_paths
 from nxtomo.nxobject.nxmonitor import NXmonitor
-
-from pyunitsystem.energysystem import EnergySI
-
-from ..nxobject.nxinstrument import NXinstrument
-from ..nxobject.nxobject import ElementWithUnit, NXobject
-from ..nxobject.nxsample import NXsample
-from ..nxobject.utils import get_data, get_data_and_unit
+from nxtomo.nxobject.nxdetector import ImageKey
+from nxtomo.nxobject.nxinstrument import NXinstrument
+from nxtomo.nxobject.nxobject import ElementWithUnit, NXobject
+from nxtomo.nxobject.nxsample import NXsample
+from nxtomo.nxobject.utils import get_data, get_data_and_unit
 
 _logger = logging.getLogger(__name__)
 
 
-class ImageKey(_Enum):
-    ALIGNMENT = -1
-    PROJECTION = 0
-    FLAT_FIELD = 1
-    DARK_FIELD = 2
-    INVALID = 3
-
-
 class NXtomo(NXobject):
     """
     Class defining an NXTomo.
     His final goal is to save data to disk.
 
     :param str node_name: node_name is used by the NXobject parent to order children when dumping it to file.
                           has NXtomo is expected to be the highest object in the hierachy. node_name will only be used for saving if no `data_path` is provided when calling 'save' function.
```

### Comparing `nxtomo-0.1.0/nxtomo/application/test/test_nxtomo.py` & `nxtomo-0.2.0/nxtomo/application/test/test_nxtomo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 from datetime import datetime
 from tempfile import TemporaryDirectory
 import numpy
 
 import pytest
 from silx.io.url import DataUrl
-from tomoscan.esrf import HDF5TomoScan
-from tomoscan.validator import ReconstructionValidator
 
-from nxtomo.application.nxtomo import NXtomo, concatenate, ImageKey
-from nxtomo.nxobject.nxdetector import FieldOfView
+from nxtomo.application.nxtomo import NXtomo
+from nxtomo.nxobject.nxdetector import FieldOfView, ImageKey
+from nxtomo.nxobject.utils import concatenate
 
 
 nexus_path_versions = (1.1, 1.0, None)
 
 
 @pytest.mark.parametrize("nexus_path_version", nexus_path_versions)
 def test_nx_tomo(nexus_path_version):
@@ -133,41 +132,78 @@
         nx_tomo.save(
             file_path=file_path,
             data_path="entry",
             nexus_path_version=nexus_path_version,
         )
         assert os.path.exists(file_path)
 
-        # insure we can read it from tomoscan
-        scan = HDF5TomoScan(file_path, entry="entry")
-        assert len(scan.flats) == 4
-        assert len(scan.darks) == 3
-        assert len(scan.projections) == 8
-        assert len(scan.alignment_projections) == 1
-        assert scan.energy == 12.3
-        assert scan.pixel_size == 1e-7
-        assert scan.distance == 0.2
-        assert scan.field_of_view == FieldOfView.HALF
-        assert scan.sample_name == "my sample"
+        # insure we can read it back
+        scan = NXtomo().load(file_path, data_path="entry")
         assert (
-            len(scan.x_translation)
-            == len(scan.y_translation)
-            == len(scan.z_translation)
+            len(
+                tuple(
+                    filter(
+                        lambda image_key: image_key is ImageKey.FLAT_FIELD,
+                        scan.instrument.detector.image_key_control,
+                    )
+                )
+            )
+            == 4
+        )
+        assert (
+            len(
+                tuple(
+                    filter(
+                        lambda image_key: image_key is ImageKey.DARK_FIELD,
+                        scan.instrument.detector.image_key_control,
+                    )
+                )
+            )
+            == 3
+        )
+        assert (
+            len(
+                tuple(
+                    filter(
+                        lambda image_key: image_key is ImageKey.PROJECTION,
+                        scan.instrument.detector.image_key_control,
+                    )
+                )
+            )
+            == 8
+        )
+        assert (
+            len(
+                tuple(
+                    filter(
+                        lambda image_key: image_key is ImageKey.ALIGNMENT,
+                        scan.instrument.detector.image_key_control,
+                    )
+                )
+            )
+            == 1
+        )
+        assert scan.energy.value == 12.3
+        assert scan.instrument.detector.x_pixel_size.value == 1e-7
+        assert scan.instrument.detector.y_pixel_size.value == 1e-7
+        assert scan.instrument.detector.distance.value == 0.2
+        assert scan.instrument.detector.field_of_view == FieldOfView.HALF
+        assert scan.sample.name == "my sample"
+        assert (
+            len(scan.sample.x_translation.value)
+            == len(scan.sample.y_translation.value)
+            == len(scan.sample.z_translation.value)
             == n_frames
         )
-        assert scan.x_translation[0] == 0.6
-        assert scan.y_translation[0] == 0.2
-        assert scan.z_translation[0] == 0.1
+        assert scan.sample.x_translation.value[0] == 0.6
+        assert scan.sample.y_translation.value[0] == 0.2
+        assert scan.sample.z_translation.value[0] == 0.1
         if nexus_path_version != 1.0:
-            assert scan.source_name is not None
-            assert scan.source_type is not None
-
-        # check values validity using the validator
-        validator = ReconstructionValidator(scan=scan)
-        assert validator.is_valid()
+            assert scan.instrument.source.name is not None
+            assert scan.instrument.source.type is not None
 
         # try to load it from the disk
         loaded_nx_tomo = NXtomo("test").load(file_path=file_path, data_path="entry")
         assert isinstance(loaded_nx_tomo, NXtomo)
         assert loaded_nx_tomo.energy.value == nx_tomo.energy.value
         assert loaded_nx_tomo.energy.unit == nx_tomo.energy.unit
         assert loaded_nx_tomo.start_time == nx_tomo.start_time
```

### Comparing `nxtomo-0.1.0/nxtomo/io.py` & `nxtomo-0.2.0/nxtomo/io.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxdetector.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxdetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 import h5py
 from h5py import h5s as h5py_h5s
 from h5py import VirtualSource
 
 from silx.io.url import DataUrl
 from silx.utils.proxy import docstring
 from silx.utils.deprecation import deprecated_warning
+from silx.utils.enum import Enum as _Enum
 
 from nxtomo.utils.frameappender import FrameAppender
 from nxtomo.io import from_virtual_source_to_data_url
-from nxtomo.application.nxtomo import ImageKey
 from nxtomo.io import HDF5File
 from nxtomo.paths.nxtomo import get_paths as get_nexus_path
-from nxtomo.utils import cast_and_check_array_1D, get_data, get_data_and_unit
-from nxtomo.utils.transformation import (
-    LRDetTransformation,
-    UDDetTransformation,
-)
 from nxtomo.nxobject.nxobject import ElementWithUnit, NXobject
 from nxtomo.nxobject.nxtransformations import (
     NXtransformations,
     get_lr_flip,
     get_ud_flip,
 )
+from nxtomo.utils import cast_and_check_array_1D, get_data, get_data_and_unit
+from nxtomo.utils.transformation import (
+    LRDetTransformation,
+    UDDetTransformation,
+)
 
 from pyunitsystem import TimeSystem, Unit
 from pyunitsystem.metricsystem import MetricSystem
 
 
 try:
     from h5py._hl.vds import VDSmap
@@ -56,14 +56,25 @@
 
         return super().from_value(value)
 
     FULL = "Full"
     HALF = "Half"
 
 
+FieldOfView = FOV
+
+
+class ImageKey(_Enum):
+    ALIGNMENT = -1
+    PROJECTION = 0
+    FLAT_FIELD = 1
+    DARK_FIELD = 2
+    INVALID = 3
+
+
 class NXdetector(NXobject):
     def __init__(
         self,
         node_name="detector",
         parent=None,
         field_of_view=None,
         expected_dim: Optional[tuple] = None,
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxinstrument.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxinstrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from silx.utils.proxy import docstring
 from nxtomo.io import HDF5File
 from pyunitsystem.voltagesystem import VoltageSystem
 
 from nxtomo.paths.nxtomo import get_paths as get_nexus_paths
 from nxtomo.nxobject.nxdetector import NXdetector, NXdetectorWithUnit
 from nxtomo.nxobject.nxsource import DefaultESRFSource, NXsource
-from nxtomo.nxobject import NXobject
+from nxtomo.nxobject.nxobject import NXobject
 from nxtomo.utils import get_data
 
 _logger = logging.getLogger(__name__)
 
 
 class NXinstrument(NXobject):
     def __init__(
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxmonitor.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxobject.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxobject.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxsample.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxsource.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxsource.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from functools import partial
 from operator import is_not
 from typing import Optional, Union
 
 import numpy
 from silx.utils.enum import Enum as _Enum
 from silx.utils.proxy import docstring
-from nxtomo.paths.nxtomo import get_paths as get_nexus_paths
 
-from nxtomo.nxobject import NXobject
+from nxtomo.paths.nxtomo import get_paths as get_nexus_paths
+from nxtomo.nxobject.nxobject import NXobject
 from nxtomo.utils import get_data
 
 _logger = logging.getLogger(__name__)
 
 
 class SourceType(_Enum):
     SPALLATION_NEUTRON = "Spallation Neutron Source"
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/nxtransformations.py` & `nxtomo-0.2.0/nxtomo/nxobject/nxtransformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 from copy import deepcopy
 
 from silx.utils.proxy import docstring
 from silx.io.dictdump import nxtodict
 
-from nxtomo.nxobject import NXobject
+from nxtomo.nxobject.nxobject import NXobject
 from nxtomo.io import HDF5File
 from nxtomo.utils.transformation import (
     Transformation,
     GravityTransformation,
     get_lr_flip as _get_lr_flip,
     get_ud_flip as _get_ud_flip,
 )
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxdetector.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxdetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 import tempfile
 
 import h5py
 import numpy.random
 import pytest
 from silx.io.url import DataUrl
-from tomoscan.esrf.scan.utils import cwd_context
-from tomoscan.unitsystem.voltagesystem import VoltageSystem
-from tomoscan.nexus.utils.transformation import TransformationAxis
+from nxtomo.io import cwd_context
+from pyunitsystem.voltagesystem import VoltageSystem
+from nxtomo.utils.transformation import TransformationAxis
 
-from nxtomomill.nexus.nxtransformations import Transformation
-from nxtomomill.nexus.nxdetector import FieldOfView, NXdetector, NXdetectorWithUnit
-from nxtomomill.utils import ImageKey
+from nxtomo.nxobject.nxtransformations import Transformation
+from nxtomo.nxobject.nxdetector import (
+    FieldOfView,
+    NXdetector,
+    NXdetectorWithUnit,
+    ImageKey,
+)
 
 
 def test_nx_detector():
     """test creation and saving of an nxdetector"""
     nx_detector = NXdetector(expected_dim=(2, 3))
 
     # check data
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxinstrument.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxinstrument.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
-from nxtomomill.nexus.nxdetector import NXdetector
-from nxtomomill.nexus.nxinstrument import NXinstrument
-from nxtomomill.nexus.nxsource import DefaultESRFSource, NXsource
+from nxtomo.nxobject.nxdetector import NXdetector
+from nxtomo.nxobject.nxinstrument import NXinstrument
+from nxtomo.nxobject.nxsource import DefaultESRFSource, NXsource
 
 
 def test_nx_instrument():
     """test creation and saving of an nxinstrument"""
     nx_instrument = NXinstrument()
 
     # check data
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxmonitor.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxmonitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy
 import pytest
 
-from nxtomomill.nexus import concatenate
-from nxtomomill.nexus.nxmonitor import NXmonitor
+from nxtomo.nxobject.utils import concatenate
+from nxtomo.nxobject.nxmonitor import NXmonitor
 
 
 def test_nx_sample():
     """test creation and saving of an nxsource"""
     nx_monitor = NXmonitor()
     # check name
     with pytest.raises(TypeError):
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxobject.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from tempfile import TemporaryDirectory
 from typing import Optional
 
 import numpy
 import pytest
-from tomoscan import unitsystem
+import pyunitsystem as unitsystem
 
-from nxtomomill.nexus.nxobject import ElementWithUnit, NXobject
+from nxtomo.nxobject.nxobject import ElementWithUnit, NXobject
 
 
 class test_nx_object:
     """Tets API of the nx object"""
 
     with pytest.raises(TypeError):
         NXobject(node_name=12)
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxsample.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy
 import pytest
 
-from nxtomomill.nexus.nxsample import NXsample
+from nxtomo.nxobject.nxsample import NXsample
 
 
 def test_nx_sample():
     """test creation and saving of an nxsource"""
     nx_sample = NXsample()
     # check name
     with pytest.raises(TypeError):
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxsource.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from nxtomomill.nexus.nxsource import NXsource
+from nxtomo.nxobject.nxsource import NXsource
 
 
 def test_nx_source():
     """test creation and saving of an nxsource"""
     nx_source = NXsource()
     with pytest.raises(TypeError):
         nx_source.name = 12
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/test/test_nxtransformations.py` & `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxtransformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy
 import pytest
 
-from nxtomomill.nexus.nxtransformations import NXtransformations
-from tomoscan.nexus.utils.transformation import (
+from nxtomo.nxobject.nxtransformations import NXtransformations
+from nxtomo.utils.transformation import (
     Transformation,
     TransformationAxis,
 )
 
 
 def test_nx_transforamtions(tmp_path):
     """test creation and saving of an NXtransformations"""
```

### Comparing `nxtomo-0.1.0/nxtomo/nxobject/utils.py` & `nxtomo-0.2.0/nxtomo/nxobject/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable
 
 import h5py
 from silx.io.utils import h5py_read_dataset
-from tomoscan.io import HDF5File
 
-from nxtomomill.nexus.nxobject import NXobject
+from nxtomo.io import HDF5File
+from nxtomo.nxobject.nxobject import NXobject
 
 
 def create_nx_data_group(file_path: str, entry_path: str, axis_scale: list):
     """
     Create the 'Nxdata' group at entry level with soft links on the NXDetector
     and NXsample.
```

### Comparing `nxtomo-0.1.0/nxtomo/paths/nxdetector.py` & `nxtomo-0.2.0/nxtomo/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/paths/nxsample.py` & `nxtomo-0.2.0/nxtomo/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/paths/nxtomo.py` & `nxtomo-0.2.0/nxtomo/paths/nxtomo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import logging
 from typing import Optional
 
 from silx.utils.deprecation import deprecated
 
-import tomoscan
-
-from . import nxdetector, nxinstrument, nxmonitor, nxsample, nxsource, nxtransformations
+import nxtomo
+from nxtomo.paths import (
+    nxdetector,
+    nxinstrument,
+    nxmonitor,
+    nxsample,
+    nxsource,
+    nxtransformations,
+)
 
 _logger = logging.getLogger(__name__)
 
 
 LATEST_VERSION = 1.3
 
 
 class NXtomo_PATH:
-    # list all path that can be used by an nxtomo entry and read by tomoscan.
+    # list all path that can be used by an nxtomo entry and read by nxtomo.
     # this is also used by nxtomomill to know were to save data
 
     _NX_DETECTOR_PATHS = None
     _NX_INSTRUMENT_PATHS = None
     _NX_SAMPLE_PATHS = None
     _NX_SOURCE_PATHS = None
     _NX_CONTROL_PATHS = None
@@ -413,25 +419,25 @@
     if version is None:
         version = LATEST_VERSION
         _logger.warning(
             f"version of the NXtomo not found. Will take the latest one ({LATEST_VERSION})"
         )
     versions_dict = {
         # Ensure compatibility with "old" datasets (acquired before Dec. 2021).
-        # Tomoscan can still parse them provided that nx_version=1.0 is forced at init.
+        # nxtomo can still parse them provided that nx_version=1.0 is forced at init.
         0.0: nx_tomo_path_v_1_0,
         0.1: nx_tomo_path_v_1_0,
         #
         1.0: nx_tomo_path_v_1_0,
         1.1: nx_tomo_path_v_1_1,
         1.2: nx_tomo_path_v_1_2,
         1.3: nx_tomo_path_v_1_3,
     }
     if version not in versions_dict:
         if int(version) == 1:
             _logger.warning(
-                f"nexus path {version} requested but unknow from this version of tomoscan {tomoscan.__version__}. Pick latest one of this major version. You might miss some information"
+                f"nexus path {version} requested but unknow from this version of nxtomo {nxtomo.__version__}. Pick latest one of this major version. You might miss some information"
             )
             version = LATEST_VERSION
         else:
             raise ValueError(f"Unknow major version of the nexus path ({version})")
     return versions_dict[version]
```

### Comparing `nxtomo-0.1.0/nxtomo/paths/nxtransformations.py` & `nxtomo-0.2.0/nxtomo/paths/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/paths/test/test_backward_compatibility.py` & `nxtomo-0.2.0/nxtomo/paths/test/test_backward_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 __authors__ = ["H.Payno"]
 __license__ = "MIT"
 __date__ = "10/02/2022"
 
 
 import pytest
 
-from tomoscan.nexus.paths.nxtomo import get_paths as new_get_paths
-from tomoscan.nexus.paths.nxtomo import nx_tomo_path_latest
+from nxtomo.paths.nxtomo import get_paths as new_get_paths
+from nxtomo.paths.nxtomo import nx_tomo_path_latest
 
 
-# classes which wre previously defining path to save data as NXtomo from tomoscan.esrf.scan.nxtomoscan.py file
+# classes which were previously defining path to save data as NXtomo from tomoscan.esrf.scan.nxtomoscan.py file
 class _NEXUS_PATHS:
     """Register path to NXtomo
     The raw data are the one of the initial version.
     If the value is None then the path was not existing originally.
     """
 
     PROJ_PATH = "instrument/detector/data"
```

### Comparing `nxtomo-0.1.0/nxtomo/utils/frameappender.py` & `nxtomo-0.2.0/nxtomo/utils/frameappender.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/utils/io.py` & `nxtomo-0.2.0/nxtomo/utils/io.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/utils/test/test_transformation.py` & `nxtomo-0.2.0/nxtomo/utils/test/test_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 import numpy
-from tomoscan.nexus.utils.transformation import (
+from nxtomo.utils.transformation import (
     Transformation,
     TransformationAxis,
     TransformationType,
     UDDetTransformation,
     LRDetTransformation,
     GravityTransformation,
     get_lr_flip,
     get_ud_flip,
     build_matrix,
 )
-from tomoscan.nexus.paths.nxtransformations import NEXUS_TRANSFORMATIONS_PATH
+from nxtomo.paths.nxtransformations import NEXUS_TRANSFORMATIONS_PATH
 
 
 def test_Transformation():
     """
     test Transformation class
     """
     transformation_translation = Transformation(
```

### Comparing `nxtomo-0.1.0/nxtomo/utils/transformation.py` & `nxtomo-0.2.0/nxtomo/utils/transformation.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/nxtomo/utils/utils.py` & `nxtomo-0.2.0/nxtomo/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Iterable
 import h5py
 import numpy
 from silx.io.utils import h5py_read_dataset
 
 from nxtomo.io import HDF5File
-from nxtomo.nxobject import NXobject
 
 
 def cast_and_check_array_1D(array, array_name):
     if not isinstance(array, (type(None), numpy.ndarray, Iterable)):
         raise TypeError(
             f"{array_name} is expected to be None, or an Iterable. Not {type(array)}"
         )
@@ -102,16 +101,7 @@
 
 def get_data(file_path, data_path):
     with HDF5File(file_path, mode="r") as h5f:
         if data_path in h5f:
             return h5py_read_dataset(h5f[data_path])
         else:
             return None
-
-
-def concatenate(nx_objects: Iterable, **kwargs):
-    if len(nx_objects) == 0:
-        return None
-    else:
-        if not isinstance(nx_objects[0], NXobject):
-            raise TypeError("nx_objects are expected to be instances of NXobject")
-        return type(nx_objects[0]).concatenate(nx_objects=nx_objects, **kwargs)
```

### Comparing `nxtomo-0.1.0/nxtomo.egg-info/PKG-INFO` & `nxtomo-0.2.0/nxtomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 0.1.0
+Version: 0.2.0
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-0.1.0/nxtomo.egg-info/SOURCES.txt` & `nxtomo-0.2.0/nxtomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxtomo-0.1.0/pyproject.toml` & `nxtomo-0.2.0/pyproject.toml`

 * *Files identical despite different names*

