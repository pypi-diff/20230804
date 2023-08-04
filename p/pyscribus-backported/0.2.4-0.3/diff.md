# Comparing `tmp/pyscribus-backported-0.2.4.tar.gz` & `tmp/pyscribus-backported-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscribus-backported-0.2.4.tar", last modified: Thu Mar 16 19:21:23 2023, max compression
+gzip compressed data, was "pyscribus-backported-0.3.tar", last modified: Fri Aug  4 17:00:00 2023, max compression
```

## Comparing `pyscribus-backported-0.2.4.tar` & `pyscribus-backported-0.3.tar`

### file list

```diff
@@ -1,50 +1,61 @@
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.637041 pyscribus-backported-0.2.4/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-backported-0.2.4/LICENSE
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1424 2023-03-16 19:21:23.637041 pyscribus-backported-0.2.4/PKG-INFO
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.629042 pyscribus-backported-0.2.4/pyscribus/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-03-16 19:17:29.000000 pyscribus-backported-0.2.4/pyscribus/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    18332 2023-03-16 17:58:03.000000 pyscribus-backported-0.2.4/pyscribus/colors.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.629042 pyscribus-backported-0.2.4/pyscribus/common/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-03-11 18:35:21.000000 pyscribus-backported-0.2.4/pyscribus/common/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2502 2023-03-16 19:14:28.000000 pyscribus-backported-0.2.4/pyscribus/common/math.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    12795 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/common/xml.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35584 2023-03-16 18:04:38.000000 pyscribus-backported-0.2.4/pyscribus/dimensions.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    56869 2023-03-16 19:15:52.000000 pyscribus-backported-0.2.4/pyscribus/document.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3495 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/exceptions.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.633041 pyscribus-backported-0.2.4/pyscribus/extra/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-03-11 18:35:21.000000 pyscribus-backported-0.2.4/pyscribus/extra/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14464 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/extra/wireframe.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.633041 pyscribus-backported-0.2.4/pyscribus/headless/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3506 2023-03-16 17:52:37.000000 pyscribus-backported-0.2.4/pyscribus/headless/__init__.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.633041 pyscribus-backported-0.2.4/pyscribus/headless/scripts/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:52:37.000000 pyscribus-backported-0.2.4/pyscribus/headless/scripts/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1192 2023-03-16 17:52:37.000000 pyscribus-backported-0.2.4/pyscribus/headless/scripts/topdf.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5037 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/itemattribute.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5591 2023-03-16 17:55:23.000000 pyscribus-backported-0.2.4/pyscribus/layers.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1639 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/logs.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     9736 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/marks.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7131 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/notes.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)   104044 2023-03-16 18:13:13.000000 pyscribus-backported-0.2.4/pyscribus/pageobjects.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35245 2023-03-16 19:10:12.000000 pyscribus-backported-0.2.4/pyscribus/pages.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.637041 pyscribus-backported-0.2.4/pyscribus/papers/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-03-11 18:35:23.000000 pyscribus-backported-0.2.4/pyscribus/papers/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3758 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/papers/afnor.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2209 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/papers/ansi.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3235 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/papers/iso216.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1738 2023-03-11 18:35:23.000000 pyscribus-backported-0.2.4/pyscribus/papers/iso217.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2333 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/papers/iso269.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1609 2023-03-16 17:52:19.000000 pyscribus-backported-0.2.4/pyscribus/papers/newspaper.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5667 2023-03-16 18:18:52.000000 pyscribus-backported-0.2.4/pyscribus/patterns.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    17027 2023-03-16 17:55:23.000000 pyscribus-backported-0.2.4/pyscribus/printing.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8969 2023-03-16 17:52:20.000000 pyscribus-backported-0.2.4/pyscribus/sla.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    38817 2023-03-16 17:52:20.000000 pyscribus-backported-0.2.4/pyscribus/stories.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    75422 2023-03-16 19:15:54.000000 pyscribus-backported-0.2.4/pyscribus/styles.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7861 2023-03-16 17:52:20.000000 pyscribus-backported-0.2.4/pyscribus/toc.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 19:21:23.637041 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1424 2023-03-16 19:21:21.000000 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1045 2023-03-16 19:21:21.000000 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/SOURCES.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-03-16 19:21:21.000000 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/dependency_links.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-03-16 19:21:21.000000 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/requires.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-03-16 19:21:21.000000 pyscribus-backported-0.2.4/pyscribus_backported.egg-info/top_level.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-03-16 19:21:23.637041 pyscribus-backported-0.2.4/setup.cfg
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1347 2023-03-16 19:17:29.000000 pyscribus-backported-0.2.4/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-backported-0.3/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1564 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/PKG-INFO
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.343303 pyscribus-backported-0.3/pyscribus/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      916 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.343303 pyscribus-backported-0.3/pyscribus/file/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13484 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3538 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/file/colors.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    10602 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/document.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2479 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/exceptions.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8368 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/hyphenation.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20239 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/pageobjects.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    11505 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/file/stories.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20151 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/file/ui.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    21019 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/colors.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/common/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/common/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5006 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/common/math.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13845 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/common/xml.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    36326 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/dimensions.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    81970 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/document.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3648 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/exceptions.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/extra/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/extra/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14402 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/extra/wireframe.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/headless/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3512 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/headless/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/headless/scripts/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/headless/scripts/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1198 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/headless/scripts/topdf.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5190 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/itemattribute.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5609 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/layers.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1715 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/logs.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    11127 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/marks.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8656 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/notes.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)   110484 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/pageobjects.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35746 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/pages.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus/model/papers/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3789 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/afnor.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2222 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/ansi.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3265 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/iso216.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1744 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/iso217.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2353 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/iso269.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1621 2023-08-04 15:48:35.000000 pyscribus-backported-0.3/pyscribus/model/papers/newspaper.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5685 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/patterns.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    24254 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/printing.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     6154 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/sla.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    44007 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/stories.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    61005 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/styles.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7643 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/pyscribus/model/toc.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/pyscribus_backported.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1564 2023-08-04 17:00:00.000000 pyscribus-backported-0.3/pyscribus_backported.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1480 2023-08-04 17:00:00.000000 pyscribus-backported-0.3/pyscribus_backported.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-08-04 17:00:00.000000 pyscribus-backported-0.3/pyscribus_backported.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-08-04 17:00:00.000000 pyscribus-backported-0.3/pyscribus_backported.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-08-04 17:00:00.000000 pyscribus-backported-0.3/pyscribus_backported.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-08-04 17:00:00.347303 pyscribus-backported-0.3/setup.cfg
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1351 2023-08-04 16:55:57.000000 pyscribus-backported-0.3/setup.py
```

### Comparing `pyscribus-backported-0.2.4/LICENSE` & `pyscribus-backported-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscribus-backported-0.2.4/PKG-INFO` & `pyscribus-backported-0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: pyscribus-backported
-Version: 0.2.4
+Version: 0.3
 Summary: Read, create and update Scribus .sla files. (Python < 3.8 version)
 Author: Étienne Nadji
 Author-email: etnadji@eml.cc
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://etnadji.fr/pyscribus
-Project-URL: Source Code, https://framagit.org/etnadji/pyscribus/-/tree/backported
+Project-URL: Source Code, https://framagit.org/etnadji/pyscribus/-/tree/backported-model
 Project-URL: Issue tracker, https://framagit.org/etnadji/pyscribus/-/issues
 Keywords: scribus,sla
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Intended Audience :: Developers
 Requires-Python: <=3.7.9
 License-File: LICENSE
 
-######################
-PyScribus (backported)
-######################
+.. image:: https://etnadji.fr/pyscribus/_static/logo-300.png
+    :alt: PyScribus logo
+    :align: center
 
-A Python library to read, generate and update Scribus documents (SLA).
+A library aiming to read, generate and update Scribus documents (SLA).
 
-For Python versions newer than 3.7.9, see the main **pyscribus** package.
+----
 
-Prerequisites
-=============
+.. image:: https://nogithub.codeberg.page/badge.svg
+    :alt: Please don't upload to GitHub
+    :target: https://nogithub.codeberg.page
+.. image:: https://img.shields.io/pypi/v/pyscribus.svg?label=latest%20version
+    :alt: PyPi Latest Version
+    :target: https://pypi.python.org/pypi/pyscribus
 
-* `lxml <https://lxml.de/>`_
-* `svg.path <https://pypi.org/project/svg.path/>`_
+----
 
-Optional (for extra features)
------------------------------
+For Python versions newer than 3.8, see the main 
+`pyscribus <https://pypi.org/project/pyscribus>`_ package.
 
-* `Pillow <https://python-pillow.org/>`_ for ``extra.wireframe`` module
+- `Quickstart <https://etnadji.fr/pyscribus/guide/en/quickstart.html>`_
 
-Documentation
-=============
-
-`PyScribus <https://etnadji.fr/pyscribus>`_
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/__init__.py` & `pyscribus-backported-0.3/pyscribus/model/papers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
-PyScribus
+PyScribus submodule for paper sizes
 """
 
-from pyscribus.sla import SLA
-
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
-__version__ = "0.2.4"
+__version__ = "0.1"
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/colors.py` & `pyscribus-backported-0.3/pyscribus/model/colors.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,28 +19,36 @@
 
 """
 PyScribus classes for colors and gradients.
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+from typing import Union, NoReturn, Literal, List
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as pmath
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as pmath
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
+ColorSpace = Literal["cmyk", "rgb"]
+
 # Classes ===============================================================#
 
+
 class Color(xmlc.PyScribusElement):
     """
     SLA Color (COLOR)
 
     :type kwargs: dict
     :param kwargs: Quick setting (see kwargs table)
 
@@ -49,84 +57,88 @@
     +============+=================================+===========+
     | default    | Equivalent to a ``fromdefault`` | boolean   |
     |            | call.                           | or string |
     |            |                                 |           |
     |            | Value being True or the name of |           |
     |            | the default set.                |           |
     +------------+---------------------------------+-----------+
+    | name       | Color name                      | string    |
+    +------------+---------------------------------+-----------+
+    | space      | Color space.                    | string    |
+    |            |                                 |           |
+    |            | Either "rgb" or "cmyk".         |           |
+    +------------+---------------------------------+-----------+
+    | cmyk       | Inks in C, M, Y, K order.       | list of   |
+    |            |                                 | floats    |
+    +------------+---------------------------------+-----------+
+    | rgb        | Inks in R, G, B order.          | list of   |
+    |            |                                 | floats    |
+    +------------+---------------------------------+-----------+
     """
 
     defaults = {
-        "Black": {
-            "space": "cmyk",
-            "colors": [0, 0, 0, 100]
-        },
-        "Blue": {
-            "space": "rgb",
-            "colors": [0, 0, 255]
-        },
-        "Cool Black": {
-            "space": "cmyk",
-            "colors": [60, 0, 0, 100]
-        },
-        "Cyan": {
-            "space": "cmyk",
-            "colors": [100, 0, 0, 0]
-        },
-        "Green": {
-            "space": "rgb",
-            "colors": [0, 255, 0]
-        },
-        "Magenta": {
-            "space": "cmyk",
-            "colors": [0, 100, 0, 0]
-        },
-        "Red": {
-            "space": "rgb",
-            "colors": [255, 0, 0]
-        },
+        "Black": {"space": "cmyk", "colors": [0, 0, 0, 100]},
+        "Blue": {"space": "rgb", "colors": [0, 0, 255]},
+        "Cool Black": {"space": "cmyk", "colors": [60, 0, 0, 100]},
+        "Cyan": {"space": "cmyk", "colors": [100, 0, 0, 0]},
+        "Green": {"space": "rgb", "colors": [0, 255, 0]},
+        "Magenta": {"space": "cmyk", "colors": [0, 100, 0, 0]},
+        "Red": {"space": "rgb", "colors": [255, 0, 0]},
         "Registration": {
             "space": "cmyk",
             "colors": [100, 100, 100, 100],
-            "register": True
-        },
-        "Rich Black": {
-            "space": "cmyk",
-            "colors": [60, 40, 40, 100]
+            "register": True,
         },
+        "Rich Black": {"space": "cmyk", "colors": [60, 40, 40, 100]},
         "Warm Black": {
             "space": "cmyk",
-            "colors": [0, 60, 29.8039215686275, 100]
-        },
-        "White": {
-            "space": "cmyk",
-            "colors": [0, 0, 0, 0]
-        },
-        "Yellow": {
-            "space": "cmyk",
-            "colors": [0, 0, 100, 0]
+            "colors": [0, 60, 29.8039215686275, 100],
         },
+        "White": {"space": "cmyk", "colors": [0, 0, 0, 0]},
+        "Yellow": {"space": "cmyk", "colors": [0, 0, 100, 0]},
     }
 
+    rgb = lambda s: s.lower() == "rgb"
+    cmyk = lambda s: s.lower() == "cmyk"
+
     def __init__(
-            self, name="Black", space="CMYK", colors=[0,0,0,100],
-            register="0", **kwargs):
+        self,
+        name: str = "Black",
+        space: str = "CMYK",
+        colors: list = [0, 0, 0, 100],
+        register: str = "0",
+        **kwargs,
+    ):
         super().__init__()
 
         self.pyscribus_defaults = [k for k in Color.defaults.keys()]
 
         self.name = name
         self.register = register
+
+        self.colors = {}
+        self.is_cmyk = False
+        self.is_rgb = False
+
         self.set_space_colors(space, colors)
 
         self._quick_setup(kwargs)
 
-    #--- Color management --------------------------------------
+    # Color management -----------------------------------------
 
-    def set_space_colors(self, space, colors):
+    @property
+    def space(self):
+        try:
+            return {True: "cmyk", False: "rgb"}[self.is_cmyk]
+        except KeyError:
+            return None
+
+    def set_space_colors(
+        self, space: ColorSpace, colors: List[float]
+    ) -> NoReturn:
         """
         Set color space and color inks of the colors.
 
         :type space: string
         :param space: Color space. Either "cmyk" or "rgb".
         :type colors: list
         :param colors: List of inks values (float).
@@ -142,49 +154,56 @@
            color.set_space_colors("cmyk", [0, 0, 0, 0])
 
         """
 
         spaced = self.set_space(space)
 
         if spaced:
-            self.set_colors(colors)
+            self.set_colors(colors, self.space)
 
-    def set_colors(self, colors, space=False):
+    def set_colors(
+        self, colors: List[float], space: Union[ColorSpace, bool]
+    ) -> bool:
+        """
+        :type colors: list
+        :param colors: List of inks values (float).
+        :type space: string
+        :param space: Optionnal. Color space. Either "cmyk" or "rgb".
+        :rtype: bool
+        """
 
         if not space:
-            if self.is_cmyk:
-                space = "cmyk"
-            else:
-                space = "rgb"
+            space = {True: "cmyk", False: "rgb"}[self.is_cmyk]
 
         if space.lower() in ["cmyk", "rgb"]:
 
-            if space.lower() == "cmyk":
+            if Color.cmyk(space):
+
                 self.colors = {
                     "C": float(colors[0]),
                     "M": float(colors[1]),
                     "Y": float(colors[2]),
-                    "K": float(colors[3])
+                    "K": float(colors[3]),
                 }
 
                 # Avoid invalid values
 
                 for ink in ["C", "M", "Y", "K"]:
+
                     if self.colors[ink] > float(100.0):
                         self.colors[ink] = 100.0
 
-                for ink in ["C", "M", "Y", "K"]:
                     if self.colors[ink] < float(0.0):
                         self.colors[ink] = 0.0
 
-            if space.lower() == "rgb":
+            if Color.rgb(space):
                 self.colors = {
                     "R": float(colors[0]),
                     "G": float(colors[1]),
-                    "B": float(colors[2])
+                    "B": float(colors[2]),
                 }
 
                 # Avoid invalid values
 
                 for ink in ["R", "G", "B"]:
                     if self.colors[ink] > float(255.0):
                         self.colors[ink] = 255.0
@@ -193,52 +212,51 @@
                     if self.colors[ink] < float(0.0):
                         self.colors[ink] = 0.0
 
             return True
 
         return False
 
-    def set_space(self, space):
+    def set_space(self, space: ColorSpace) -> bool:
         """
         Set the color space (CMYK / RGB) of the color.
 
         :type space: string
         :param space: Color space. Either "cmyk" or "rgb".
+        :rtype: bool
         """
 
-        if space.lower() in ["cmyk", "rgb"]:
-            if space.lower() == "cmyk":
-                self.is_cmyk = True
-                self.is_rvb = False
-
-            if space.lower() == "rgb":
-                self.is_cmyk = False
-                self.is_rvb = True
+        space = space.lower()
+
+        if space in ["cmyk", "rgb"]:
+            self.is_cmyk = Color.cmyk(space)
+            self.is_rgb = Color.rgb(space)
 
             return True
 
         return False
 
-    #--- PyScribus standard methods ----------------------------
+    # PyScribus standard methods -------------------------------
 
-    def fromdefault(self, default="Black"):
+    def fromdefault(self, default: str = "Black") -> bool:
         """
         Set default attributes for this color.
 
         :Example:
 
         .. code:: python
 
            # with fromdefault method :
            black = Color()
            black.fromdefault("Black")
 
            # with quick setup :
            blue = Color(default="Blue")
 
+
         .. seealso::
             **For fromdefault explanation**:
             `pyscribus.common.xml.PyScribusElement.fromdefault`
 
             **For current class default sets**:
             `pyscribus.colors.Color.listdefaults`
 
@@ -246,86 +264,83 @@
 
         if default in self.pyscribus_defaults:
 
             self.name = default
 
             self.set_space_colors(
                 Color.defaults[default]["space"],
-                Color.defaults[default]["colors"]
+                Color.defaults[default]["colors"],
             )
 
             if "register" in Color.defaults[default]:
                 self.register = True
 
             return True
 
         return False
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
-        :type xml: lxml._Element
+        :type xml: lxml.etree._Element
         :param xml: XML source of color
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
         space = xml.get("SPACE")
 
-        if space is not None:
-            # Name -------------------------------------------------------
+        if space is None:
+            return False
+
+        # Name -------------------------------------------------------
 
-            name = xml.get("NAME")
+        name = xml.get("NAME")
+        if name is not None:
+            self.name = name
 
-            if name is not None:
-                self.name = name
+        # Space ------------------------------------------------------
 
-            # Space ------------------------------------------------------
+        if space.lower() in ["cmyk", "rgb"]:
+            self.set_space(space)
 
-            if space.lower() in ["cmyk", "rgb"]:
-                self.set_space(space)
+            # Colors -------------------------------------------------
 
-                # Colors -------------------------------------------------
+            if self.is_cmyk:
+                colors = [xml.get(c) for c in ["C", "M", "Y", "K"]]
+            else:
+                colors = [xml.get(c) for c in ["R", "G", "B"]]
 
-                if self.is_cmyk:
-                    colors = [xml.get(c) for c in ["C", "M", "Y", "K"]]
-                else:
-                    colors = [xml.get(c) for c in ["R", "G", "B"]]
+            if not colors:
+                raise exceptions.InvalidColor("No inks.")
 
-                if colors:
-                    if None in colors:
-                        raise exceptions.InvalidColor(
-                            "Invalid inks <{}>.".format(",".join(colors))
-                        )
-                    else:
-                        self.set_colors(colors)
-                else:
-                    raise exceptions.InvalidColor("No inks.")
+            if None in colors:
+                raise exceptions.InvalidColor(
+                    "Invalid inks <{}>.".format(",".join(colors))
+                )
 
-            # Register ---------------------------------------------------
+            self.set_colors(colors, self.space)
 
-            reg = xml.get("Register")
+        # Register ---------------------------------------------------
 
-            if reg is None:
-                self.register = False
+        reg = xml.get("Register")
+        if reg is None:
+            self.register = False
+        else:
+            if int(reg):
+                self.register = True
             else:
-                if int(reg):
-                    self.register = True
-                else:
-                    self.register = False
-
-            # ------------------------------------------------------------
+                self.register = False
 
-            return True
+        # ------------------------------------------------------------
 
-        else:
-            return False
+        return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         :returns: Color as XML element
         """
 
         xml = ET.Element("COLOR")
         xml.attrib["NAME"] = self.name
 
         if self.is_cmyk:
@@ -343,85 +358,124 @@
                 xml.attrib[color] = str(color_value)
 
         if self.register:
             xml.attrib["Register"] = "1"
 
         return xml
 
-    def _quick_setup(self, settings: dict):
+    def _quick_setup(self, settings: dict) -> NoReturn:
         """
         Method for defining gradient stop settings from class
         instanciation kwargs.
 
         :type settings: dict
         :param settings: Kwargs dictionnary
         """
 
         if settings:
             xmlc.PyScribusElement._quick_setup(self, settings)
 
+            # Color space is treated first. ------------------------------
+
+            if "space" in settings:
+                self.set_space(str(settings["space"]))
+                settings.pop("space")
+
             for setting_name, setting_value in settings.items():
-                pass
 
-    #--- Python __ methods -------------------------------------
+                # Color name ---------------------------------------------
+
+                if setting_name == "name":
+                    self.name = str(setting_value)
 
-    def __eq__(self, other):
+                # Setting colors -----------------------------------------
+
+                if setting_name == "rgb":
+                    if len(setting_value) < 3:
+                        while len(setting_value) < 3:
+                            setting_value.append(float(0))
+
+                    setting_value = setting_value[:3]
+                    self.set_colors(setting_value, self.space)
+
+                if setting_name == "cmyk":
+                    if len(setting_value) < 4:
+                        while len(setting_value) < 4:
+                            setting_value.append(float(0))
+
+                    setting_value = setting_value[:4]
+                    self.set_colors(setting_value, self.space)
+
+    def same_space(self, other: Color) -> bool:
         """
-        Equality operator.
+        Is that color and other color share the same color space ?
 
-        Doesn’t check if RVB color can be an equivalent in CMYK.
+        :param other: Color instance to compare.
+        :type other: pyscribus.colors.Color
+        :returns: True if both color share the same color space.
+        :rtype: bool
         """
 
         # NOTE Obviously we don't translate colors of different spaces
         # to compare their inks, as RVB and CMYK color spectrums are
         # not the same.
 
-        same_space = False
-
         if self.is_cmyk and other.is_cmyk:
-            same_space = True
+            return True
+        if self.is_rgb and other.is_rgb:
+            return True
 
-        if self.is_rvb and other.is_rvb:
-            same_space = True
+        return False
 
-        if same_space:
-            # NOTE Self colors and other colors are in the same space, so
-            # inks dicts have the same keys. So we get a list of
-            # [(R1,R2)…] or [(C1,C2)…]. Having one ink different is enough.
-            inks = zip(self.colors.values(), other.values())
-
-            for ink in inks:
-                if ink[0] != ink[1]:
-                    return False
-        else:
+    # Python __ methods ----------------------------------------
+
+    def __iadd__(self, other: Color) -> Color:
+        if not self.same_space(other):
+            raise exceptions.ColorMixing(
+                f"Colors {self} and {other} do not share the same color space."
+            )
+
+        # FIXME TODO Implement that !
+
+        return self
+
+    def __eq__(self, other: Color) -> bool:
+        """
+        Equality operator.
+
+        Doesn’t check if RVB color can be an equivalent in CMYK.
+        """
+
+        if not self.same_space(other):
             return False
 
+        # NOTE Self colors and other colors are in the same space, so
+        # inks dicts have the same keys. So we get a list of
+        # [(R1,R2)…] or [(C1,C2)…]. Having one ink different is enough.
+        inks = zip(self.colors.values(), other.values())
+
+        for ink in inks:
+            if ink[0] != ink[1]:
+                return False
+
         return True
 
     def __repr__(self):
-        if self.is_cmyk:
-            s = "CMYK"
-            inks = ["C", "M", "Y", "K"]
-        else:
-            s = "RGB"
-            inks = ["R", "G", "B"]
-
-        r = "{}:{}:{}:{}".format(
-            self.name, s,
-            ";".join(
-                [
-                    str(self.colors[ink])
-                    for ink in inks
-                ]
-            ),
-            self.register
+        space_name = {True: "CMYK", False: "RGB"}[self.is_cmyk]
+        inks = {True: ["C", "M", "Y", "K"], False: ["R", "G", "B"]}[
+            self.is_cmyk
+        ]
+
+        return "{}:{}:{}:{}".format(
+            self.name,
+            space_name,
+            ";".join([str(self.colors[ink]) for ink in inks]),
+            self.register,
         )
 
-        return r
-
 
 class GradientColorStop(xmlc.PyScribusElement):
     """
     Gradient color stop (Gradient/CSTOP)
 
     :type kwargs: dict
     :param kwargs: Quick setting (see kwargs table)
@@ -434,15 +488,15 @@
     |            |                                 |           |
     |            | Value being True or the name of |           |
     |            | the default set.                |           |
     +------------+---------------------------------+-----------+
     | opacity    | Percentage of opacity,          | float     |
     |            | from 0 to 1.                    |           |
     +------------+---------------------------------+-----------+
-    | color      | Color name                      | string    |
+    | name       | Color name                      | string    |
     +------------+---------------------------------+-----------+
     | position   |                                 |           |
     +------------+---------------------------------+-----------+
     | shade      |                                 |           |
     +------------+---------------------------------+-----------+
 
     :Example:
@@ -454,67 +508,65 @@
        )
 
     """
 
     def __init__(self, **kwargs):
         super().__init__()
 
-        self.color = None
+        self.name = None
         self.shade = None
         self.opacity = None
         self.position = None
 
         self._quick_setup(kwargs)
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """
         Equality operator.
         """
 
-        def dimcomp(a, b):
+        def compare_property(a, b):
             if a is None:
-                if b is not None:
-                    return True
-            else:
-                if other.position is not None:
-                    if a.value != b.value:
-                        return True
+                return b is not None
+
+            if other.position is not None:
+                return a.value != b.value
 
             return False
 
-        if self.color != other.color:
+        if self.name != other.name:
             return False
 
-        if dimcomp(self.position, other.position):
+        if compare_property(self.position, other.position):
             return False
 
-        if dimcomp(self.shade, other.shade):
+        if compare_property(self.shade, other.shade):
             return False
 
-        if dimcomp(self.opacity, other.opacity):
+        if compare_property(self.opacity, other.opacity):
             return False
 
         return True
 
-    def _quick_setup(self, settings):
+    def _quick_setup(self, settings: dict) -> NoReturn:
         """
         Method for defining gradient stop settings from class
         instanciation kwargs.
 
         :type settings: dict
         :param settings: Kwargs dictionnary
         """
 
         if settings:
             xmlc.PyScribusElement._quick_setup(self, settings)
 
             for setting_name, setting_value in settings.items():
 
-                if setting_name == "color":
-                    self.color = setting_value
+                if setting_name == "name":
+                    self.name = setting_value
 
                 if setting_name == "position":
                     self.position = dimensions.Dim(
                         float(setting_value), unit="pcdecim"
                     )
 
                 if setting_name == "opacity":
@@ -525,39 +577,37 @@
                 if setting_name == "shade":
                     self.shade = dimensions.Dim(float(setting_value), unit="pc")
 
     def fromdefault(self) -> NoReturn:
         self.opacity = dimensions.Dim(100, unit="pc")
         self.position = dimensions.Dim(0, unit="pcdecim")
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         if xml.tag == "CSTOP":
-
-            color = xml.get("NAME")
-            if color is not None:
-                self.color = color
+            name = xml.get("NAME")
+            if name is not None:
+                self.name = name
 
             shade = xml.get("SHADE")
             if shade is not None:
                 self.shade = dimensions.Dim(float(shade), unit="pc")
 
             ramp = xml.get("RAMP")
             if ramp is not None:
                 self.position = dimensions.Dim(float(ramp), unit="pcdecim")
 
             opacity = xml.get("TRANS")
             if opacity is not None:
-                self.opacity = dimensions.Dim(float(opacity), "pcdecim")
                 self.opacity = dimensions.Dim(float(opacity), unit="pcdecim")
 
             return True
 
         return False
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("CSTOP")
 
         if self.position is not None:
             xml.attrib["RAMP"] = self.position.toxmlstr()
 
         xml.attrib["NAME"] = self.name
 
@@ -584,18 +634,18 @@
 
     def __init__(self):
         super().__init__()
 
         self.name = None
         self.stops = []
 
-    def _sorted_stops(self):
+    def _sorted_stops(self) -> list:
         return sorted(self.stops, key=lambda s: s.position.value)
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         if xml.tag == "Gradient":
 
             name = xml.get("Name")
             if name is not None:
                 self.name = name
 
             # TODO FIXME Ext
@@ -608,15 +658,15 @@
                     if success:
                         self.stops.append(grs)
 
             return True
 
         return False
 
-    def append_stop(self, stop, sort=False):
+    def append_stop(self, stop: GradientColorStop, sort: bool = False) -> bool:
         """
         Append a gradient color stop.
 
         Avoids duplicates. Can sort stops by color stop position.
 
         :type stop: pyscribus.colors.GradientColorStop
         :param stop: Gradient color stop to append
@@ -635,26 +685,27 @@
                 if sort:
                     self.stops = self._sorted_stops()
 
                 return True
 
         return False
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("Gradient")
 
         xml.attrib["Name"] = self.name
 
         # TODO FIXME Ext
 
         if self.stops:
 
             # Sort the color stops of the gradient by their position in
             # the gradient spectrum, ranging from 0 to 100%
 
             for stop in self._sorted_stops():
-                sx = stop.toxml()
-                xml.append(sx)
+                stop_xml = stop.toxml()
+                xml.append(stop_xml)
 
         return xml
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/common/__init__.py` & `pyscribus-backported-0.3/pyscribus/model/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-backported-0.2.4/pyscribus/common/xml.py` & `pyscribus-backported-0.3/pyscribus/model/common/xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 """
 
 # Imports ===============================================================#
 
 import copy
 import pprint
 
+from typing import Union, NoReturn
+
 import lxml
 import lxml.etree as ET
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
@@ -41,28 +43,30 @@
     "lower-roman": "Type_i_ii_iii",
     "upper-roman": "Type_I_II_III",
     "lower-latin": "Type_a_b_c",
     "upper-latin": "Type_A_B_C",
     "alpha-ar": "Type_Alphabet_ar",
     "abjad-ar": "Type_Abjad_ar",
     "hebrew": "Type_Hebrew",
+    # ASTERIX EST LA !
     "asterix": "Type_asterix",
     "cjk": "Type_CJK",
 }
 
 alignment = {
     "left": "0",
     "center": "1",
     "right": "2",
     "justify-left": "3",
-    "justify": "4"
+    "justify": "4",
 }
 
 # Classes ===============================================================#
 
+
 class PyScribusElement:
     """
     Abstract class for any element that must implement PyScribus
     common methods.
 
     :ivar list pyscribus_defaults: Names of default settings for
         fromdefault
@@ -70,17 +74,17 @@
     .. warning:: except listdefaults, all methods must be redefined by
         inherited classes.
     """
 
     def __init__(self):
         self.pyscribus_defaults = []
 
-    #--- Quick setup ---------------------------------
+    # Quick setup ------------------------------------
 
-    def _quick_setup(self, settings):
+    def _quick_setup(self, settings: dict) -> NoReturn:
         """
         Method for defining style settings from class
         instanciation kwargs.
 
         In the inherited classes, the redefined method is called
         at class instanciation and PyScribusElement._quick_setup
         is called in the redefined method.
@@ -99,17 +103,17 @@
             if "default" in settings:
 
                 if isinstance(settings["default"], bool):
                     self.fromdefault()
                 else:
                     self.fromdefault(settings["default"])
 
-    #--- Default(s) ----------------------------------
+    # Default(s) -------------------------------------
 
-    def fromdefault(self):
+    def fromdefault(self) -> bool:
         """
         Modify PyScribus element attributes according to a set of
         defaults.
 
         If fromdefault() has not other argument than self, there is
         only one, unnamed, set of default.
 
@@ -124,17 +128,17 @@
            # The class has only one default
            inherited_class_instance.fromdefault()
 
            # The class hass more than one default
            inherited_class_instance.fromdefault("english_default")
 
         """
-        pass
+        return True
 
-    def listdefaults(self):
+    def listdefaults(self) -> list:
         """
         List available defaults for the current PyScribus object.
 
         .. note:: If this method returns an empty list, that
             doesn't mean there is no defaults : it could be mean
             there is **only one** default.
 
@@ -142,35 +146,35 @@
 
         :rtype: list
         :returns: List of available defaults for fromdefault() method
         """
 
         return self.pyscribus_defaults
 
-    #--- XML import / export -------------------------
+    # XML import / export ----------------------------
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         :returns: SLA element as LXML ElementTree element
         """
 
         return False
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
-        :type xml: lxml._Element
+        :type xml: lxml.etree._Element
         :param xml: Some XML element
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
         return False
 
-    #--- Copy ----------------------------------------
+    # Copy -------------------------------------------
 
     def copy(self, **kwargs):
         """
         Returns an independant copy of the instance.
 
         Use kwargs to quick set this copy as you made it.
 
@@ -193,172 +197,197 @@
 
     :type tag: str
     :param tag: XML tag
 
     :ivar string tag: XML tag
     """
 
-    def __init__(self, tag):
+    def __init__(self, tag: str):
         PyScribusElement.__init__(self)
         self.tag = tag
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         """
+
         xml = ET.Element(self.tag)
+
         return xml
 
-    def fromdefault(self):
+    def fromdefault(self) -> bool:
         # NOTE As this class implements XML elements without any attribute
         # or childs possible, an instanciation of OrphanElement is already
         # a default.
         return True
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element) -> bool:
         """
         Parse XML element with tag OrphanElement.tag
 
+        :type xml: lxml.etree._Element
         :param xml: XML element
-        :type xml: lxml._Element
         :rtype: bool
         :returns: bool
         """
+
         if xml.tag == self.tag:
             return True
 
         return False
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "<{}/>".format(self.tag)
 
+
 # Fonctions =============================================================#
 
+# NOTE
 # We need a better typology of functions here :
 #
-# +---------------------+------------------+---------+---------------------------------+-----------+
-# | Function name       | New name ?       | Returns | Manipulation                    | Side      |
-# +---------------------+------------------+---------+---------------------------------+-----------+
-# | float_or_int_string | out_cleanfloat   | string  | number without useless decimals | xml       |
-# | str_or_nonestr      | out_str_nonestr  | string  | string or "None"                | xml ?     |
-# | bool_to_num         | out_num_boolean  | string  | boolean as "0" or "1"           | xml       |
-# | num_to_bool         | in_num_boolean   | boolean | "0" or "1" as boolean           | pyscribus |
-# | bool_or_else_to_num | out_zero_string  | string  | "0" if not(v) or v              | xml       |
-# | none_or_str         | out_empty_string | string  | "" if v is None or v            | xml ?     |
-# +---------------------+------------------+---------+---------------------------------+-----------+
+# +---------------------+------------------+---------+------------------------+-----------+
+# | Function name       | New name ?       | Returns | Manipulation           | Side      |
+# +=====================+==================+=========+========================+===========+
+# | float_or_int_string | out_cleanfloat   | string  | number without useless | ps -> xml |
+# |                     |                  |         | decimals               |           |
+# +---------------------+------------------+---------+------------------------+-----------+
+# | str_or_nonestr      | out_str_nonestr  | string  | string or "None"       | ps -> xml |
+# +---------------------+------------------+---------+------------------------+-----------+
+# | bool_to_num         | out_num_boolean  | string  | boolean as "0" or "1"  | ps -> xml |
+# +---------------------+------------------+---------+------------------------+-----------+
+# | bool_or_else_to_num | out_zero_string  | string  | "0" if not(v) or v     | ps -> xml |
+# +---------------------+------------------+---------+------------------------+-----------+
+# | none_or_str         | out_empty_string | string  | "" if v is None or v   | ps -> xml |
+# +---------------------+------------------+---------+------------------------+-----------+
+# | num_to_bool         | in_num_boolean   | boolean | "0" or "1" as boolean  | xml -> ps |
+# +---------------------+------------------+---------+------------------------+-----------+
 
-def float_or_int_string(f):
+# From PyScribus to XML ========================================#
+
+
+def float_or_int_string(f: Union[float, int]) -> str:
 
     if float(f) == int(f):
         return str(int(f))
-    else:
-        return str(f)
 
-def str_or_nonestr(v):
+    return str(f)
+
+
+def str_or_nonestr(v: str) -> str:
     """
     Returns v if v is a non-empty string, else returns 'None'.
 
     :rtype: str
     """
 
     if v:
         return v
-    else:
-        return "None"
-
-def bool_to_num(b):
-    """
-    Returns '1' if b is true, returns '0' if b is false.
 
-    :rtype: str
-    """
+    return "None"
 
-    if b:
-        return "1"
-    else:
-        return "0"
 
-def num_to_bool(n):
+def bool_to_num(b) -> str:
     """
-    Return True if n == '1', else returns False.
+    Returns '1' if b is true, returns '0' if b is false.
 
-    :rtype: bool
+    :rtype: str
     """
+    return {True: "1", False: "0"}[bool(b)]
 
-    if n == "1":
-        return True
-    else:
-        return False
 
-def bool_or_else_to_num(b):
+def bool_or_else_to_num(b) -> str:
     """
     Returns '0' if b is False, else return b as string.
 
     :rtype: str
     """
 
     if b:
         return str(b)
-    else:
-        return "0"
 
-def none_or_str(v):
+    return "0"
+
+
+def none_or_str(v) -> str:
     """
     If v is None, return empty string, else return v as string.
 
     :rtype: str
     """
+
     if v is None:
         return ""
-    else:
-        return str(v)
 
-def undocumented_to_python(xml, attributes):
+    return str(v)
+
+
+# From XML to PyScribus ========================================#
+
+
+def num_to_bool(n: str) -> bool:
+    """
+    Return True if n == '1', else returns False.
+
+    :rtype: bool
+    """
+    return n == "1"
+
+
+# Undocumented attributes ======================================#
+
+
+def undocumented_to_python(xml: ET.Element, attributes: list) -> dict:
     """
     Function to manage the import of undocumented
     XML/SLA attributes.
 
     Used in PyScribus fromxml() methods until there is
     no attribute undocumented and handled.
 
+    :type xml: lxml.etree.Element
     :param xml: XML element
-    :type xml: lxml._Element
-    :param attributes: List of attributes' names
     :type attributes: list
-    :returns: Dictionnary with attributes names as
-        keys and attribute values as values.
+    :param attributes: List of attributes' names
+    :returns: Dictionnary with attributes names as keys and attribute values
+        as values.
     :rtype: dict
 
-    Use lxml._Element.get() to get attributes values,
+    Use lxml.etree.Element.get() to get attributes values,
     so missing attributes will have None as a value.
 
     .. seealso:: `undocumented_to_xml()`
     """
+
     undocumented = {}
 
     for att_name in attributes:
         undocumented[att_name] = xml.get(att_name)
 
     return undocumented
 
-def undocumented_to_xml(xml, undocumented, no_none=False):
+
+def undocumented_to_xml(
+    xml: ET.Element, undocumented: dict, no_none: bool = False
+) -> ET.Element:
     """
     Function to manage the export of undocumented
     XML/SLA attributes.
 
     Used in PyScribus toxml() methods until there is
     no attribute undocumented and handled.
 
+    :type xml: lxml.etree._Element
     :param xml: XML element
-    :type xml: lxml._Element
+    :type undocumented: dict
     :param undocumented: Dictionnary of XML attributes.
         Return of undocumented_to_python()
-    :type undocumented: dict
+    :type no_none: bool
+    :param no_none: Skips attribute if its value is None
     :returns: xml
-    :rtype: lxml._Element
+    :rtype: lxml.etree._Element
 
     Add attributes to a XML element using undocumented
     dictionnary keys as XML attributes' names and
     undocumented dictionnary values as XML attributes'
     values.
 
     None values are ignored, through none_or_str().
@@ -371,62 +400,68 @@
             if undvalue is None:
                 continue
 
         xml.attrib[undatt] = none_or_str(undvalue)
 
     return xml
 
-def all_undocumented_to_python(xml):
+
+def all_undocumented_to_python(xml: ET.Element) -> dict:
     """
     Function to manage the import of undocumented
     XML/SLA attributes.
 
     Used in PyScribus fromxml() methods until there is
     no attribute undocumented and handled.
 
     Used instead of undocumented_to_python() if there
     is no defined list of undocumented attributes.
 
+    :type xml: lxml.etree._Element
     :param xml: XML element
-    :type xml: lxml._Element
-    :param attributes: List of attributes' names
-    :type attributes: list
     :returns: Dictionnary with attributes names as
         keys and attribute values as values.
     :rtype: dict
 
     Get all xml attributes names and values so that
     all_undocumented_to_xml() will only have to filter
     those which aren't already in the LXML element to
     export.
 
     .. seealso:: all_undocumented_to_xml()
     """
+
     undocumented = {}
 
     for att_name, att_value in xml.attrib.items():
         undocumented[att_name] = att_value
 
     return undocumented
 
+
 def all_undocumented_to_xml(
-        xml, undocumented,
-        report=True, msg="", passattr=[], logger=False):
+    xml: ET.Element,
+    undocumented: dict,
+    report: bool = True,
+    msg: str = "",
+    passattr: list = [],
+    logger=False,
+) -> list:
     """
     Function to manage the export of undocumented
     XML/SLA attributes.
 
     Used in PyScribus toxml() methods until there is
     no attribute undocumented and handled.
 
+    :type xml: lxml.etree._Element
     :param xml: XML element
-    :type xml: lxml._Element
+    :type undocumented: dict
     :param undocumented: Dictionnary of XML attributes.
         Return of all_undocumented_to_python()
-    :type undocumented: dict
     :type report: bool
     :param report: Print all undocumented attributes found in xml element.
     :type msg: str
     :param msg: Human readable name for the xml element when report parameter
         is True.
     :type passattr: list
     :param passattr: List of SLA attributes names to not report. For debug.
@@ -463,11 +498,11 @@
             logger.debug(
                 undocstr + pprint.pformat(undoc_attribs, compact=True)
             )
         else:
             print(undocstr)
             pprint.pprint(undoc_attribs, width=80, compact=True)
 
-
     return [xml, undoc_attribs]
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/dimensions.py` & `pyscribus-backported-0.3/pyscribus/model/dimensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,55 +17,53 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
 PyScribus classes for measures and geometrical manipulations.
 """
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
 import copy
 import math
 
 from typing import Union, Literal
 
-from pyscribus.common.math import PICA_TO_MM
+from pyscribus.model.common.math import PICA_TO_MM
 
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
 
-import pyscribus.papers.ansi as ansipaper
-import pyscribus.papers.iso216 as iso216paper
+import pyscribus.model.papers.ansi as ansipaper
+import pyscribus.model.papers.iso216 as iso216paper
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 XY = Literal["x", "y"]
 DimValue = Union[float, int]
 BoxCorner = Literal["top-left", "top-right", "bottom-left", "bottom-right"]
 
 # Classes ===============================================================#
 
+
 class Dim:
     """
     Dimension object. Allows to convert and export in the correct unit.
 
     :type value: Union[float, int]
     :param value: Value of the dimension
-
-    :type unit: str
-    :param unit: Unit of the dimension.
-    :type is_int: boolean
-    :param is_int: Use integer instead of float type for value
-
     :type kwargs: dict
     :param kwargs: Dimension settings (see kwargs table)
 
-    :ivar float,int value: Value of the dimension in the original unit
+    :ivar Union[float, int] value: Value of the dimension in the original unit
     :ivar string unit: Unit of the dimension
 
     +---------------+------------------------------------+
     | Kwargs        | Setting                            |
     +===============+====================================+
     | unit          | Unit of the dimension. See unit    |
     |               | table.                             |
@@ -103,30 +101,43 @@
     +--------------------------+---------------+
     | Line per inch (LPI)      | lpi           |
     +--------------------------+---------------+
     | Second                   | s, sec        |
     +--------------------------+---------------+
     """
 
-    # 1 pica point = 25,4/72 milimeters
-    PICA_TO_MM = (25.4 / 72)
-
     UNIT_ARGS = {
         "mm": ["mm"],
         "pica": ["pica", "pct"],
         "pt": ["pt"],
         "perc": ["perc", "pc"],
         "pcdecim": ["pcdecim", "pcd"],
+        "pcscale": ["pcscale"],
         "cdeg": ["cdeg"],
+        "pdeg": ["pdeg"],
         "deg": ["deg"],
         "dpi": ["dpi", "ppp", "ppi"],
         "lpi": ["lpi"],
-        "sec": ["s", "sec"]
+        "sec": ["s", "sec"],
     }
 
+    # Units that can be converted into picas at export.
+    NOT_TO_PICAS = [
+        "perc",
+        "pcdecim",
+        "pcscale",
+        "cdeg",
+        "pdeg",
+        "deg",
+        "lpi",
+        "dpi",
+        "pt",
+        "sec",
+    ]
+
     def __init__(self, value: DimValue, **kwargs: dict):
         self.value = value
         self.integer = False
         self.allow_negative = False
 
         if "integer" in kwargs:
             self.integer = bool(kwargs["integer"])
@@ -142,24 +153,22 @@
         else:
             self.set_unit("pica")
 
         if "original_unit" in kwargs:
             if kwargs["original_unit"]:
                 self.from_original_unit(kwargs["original_unit"])
 
-        print(self.__repr__())
-
         self.check_value()
 
-    #--- Checking, setting the unit --------------------------------------
+    # Checking, setting the unit -----------------------------------------
 
     def from_original_unit(self, original_unit):
         pass
 
-    def check_value(self):
+    def check_value(self) -> bool:
         """
         Check value validity according to unit.
 
         :rtype: boolean
         :return: True if the value is valid
         :raises pyscribus.exceptions.InvalidDim: Raised if value is invalid.
         """
@@ -180,211 +189,220 @@
                 raise exceptions.InvalidDim(
                     "DPI/PPP must be a positive number"
                 )
 
         if self.unit == "lpi":
 
             if self.value < 0:
-                raise exceptions.InvalidDim(
-                    "LPI must be a positive number"
-                )
+                raise exceptions.InvalidDim("LPI must be a positive number")
 
         if self.unit == "sec":
             if int(float(self.value)) != float(self.value):
                 raise exceptions.InvalidDim(
                     "Second Dim must be an integer, is {}".format(self.value)
                 )
 
+        if self.unit == "pdeg":
+            if self.value >= -180:
+                if self.value <= 180:
+                    return True
+
+                raise exceptions.InvalidDim(
+                    "Polygon tool rotation angle must range from -180 to 180"
+                )
+
+            raise exceptions.InvalidDim(
+                "Polygon tool rotation angle must range from -180 to 180"
+            )
+
         if self.unit == "cdeg":
 
             if self.value >= 0:
                 if self.value <= 180:
                     return True
-                else:
-                    raise exceptions.InvalidDim(
-                        "Calligraph pen angle must range from 0 to 180"
-                    )
-            else:
+
                 raise exceptions.InvalidDim(
                     "Calligraph pen angle must range from 0 to 180"
                 )
 
+            raise exceptions.InvalidDim(
+                "Calligraph pen angle must range from 0 to 180"
+            )
+
         if self.unit == "deg":
 
             if self.value >= 0:
 
                 if self.value <= 360:
                     return True
-                else:
-                    raise exceptions.InvalidDim(
-                        "Angle must range from 0 to 360"
-                    )
 
-            else:
-                raise exceptions.InvalidDim(
-                    "Angle must range from 0 to 360"
-                )
+                raise exceptions.InvalidDim("Angle must range from 0 to 360")
+
+            raise exceptions.InvalidDim("Angle must range from 0 to 360")
 
         return True
 
-    def set_unit(self, unit="pica"):
+    def set_unit(self, unit: str = "pica"):
         """
         Set the unit used.
 
         :type value: float,int
         :param value: Value of the dimension
         :type unit: str
         :param unit: Unit of the dimension.
         :rtype: boolean
         :return: True if the unit is valid
 
-        +-------------------------+---------------+
-        | Unit / Notation         | unit argument |
-        +=========================+===============+
-        | Milimeter               | mm            |
-        +-------------------------+---------------+
-        | Pica point              | pica, pt      |
-        +-------------------------+---------------+
-        | Percentage (0 to 100)   | perc, pc      |
-        +-------------------------+---------------+
-        | Percentage (0.0 to 1,   | pcdecim, pcd  |
-        | also negative)          |               |
-        +-------------------------+---------------+
-        | Calligraphic pen degree | cdeg          |
-        +-------------------------+---------------+
-        | Regular degree          | deg           |
-        +-------------------------+---------------+
-        | Dot per inch (DPI/PPP)  | dpi, ppp, ppi |
-        +-------------------------+---------------+
-        | Line per inch (LPI)     | lpi           |
-        +-------------------------+---------------+
-        | Second                  | s, sec        |
-        +-------------------------+---------------+
+        +--------------------------+---------------+
+        | Unit / Notation          | unit argument |
+        +==========================+===============+
+        | Milimeter                | mm            |
+        +--------------------------+---------------+
+        | Pica point               | pica, pt      |
+        +--------------------------+---------------+
+        | Percentage (0 to 100)    | perc, pc      |
+        +--------------------------+---------------+
+        | Percentage (0.0 to 1,    | pcdecim, pcd  |
+        | also negative)           |               |
+        +--------------------------+---------------+
+        | Percentage (decimal, can | pcscale       |
+        | be more than 1.0)        |               |
+        +--------------------------+---------------+
+        | Calligraphic pen degree  | cdeg          |
+        +--------------------------+---------------+
+        | Polygon tool degree      | pdeg          |
+        +--------------------------+---------------+
+        | Regular degree           | deg           |
+        +--------------------------+---------------+
+        | Dot per inch (DPI/PPP)   | dpi, ppp, ppi |
+        +--------------------------+---------------+
+        | Line per inch (LPI)      | lpi           |
+        +--------------------------+---------------+
+        | Second                   | s, sec        |
+        +--------------------------+---------------+
         """
 
         tmp_unit = unit.lower()
         valid_unit = False
 
-        for code,args in Dim.UNIT_ARGS.items():
+        for code, args in Dim.UNIT_ARGS.items():
 
             if tmp_unit in args:
                 self.unit = code
                 valid_unit = True
                 break
 
         if self.unit == "sec":
             self.integer = True
             self.value = int(self.value)
 
         return valid_unit
 
-    #--- XML export ------------------------------------------------------
+    # XML export ---------------------------------------------------------
 
-    def toxmlstr(self, no_useless_decimals=False):
+    def toxmlstr(self, no_useless_decimals: bool = False) -> str:
         """
         Returns a XML string of the dimension according to its unit.
 
         :type no_useless_decimals: boolean
         :param no_useless_decimals: Returns integer instead of float if
             decimals are 0. So 1.0 -> 1 ; 1.1 -> 1.1.
         :rtype: str
         :return: str
         """
 
-        def decimals(n):
-            if float(n) == int(n):
-                return int(n)
-            else:
-                return n
+        # Function to remove useless decimals ----------------------------
+
+        def decimals(number):
+            if float(number) == int(number):
+                return int(number)
 
             return number
 
-        if self.unit not in [
-            "perc",
-            "pcdecim",
-            "pcscale",
-            "cdeg",
-            "deg",
-            "lpi",
-            "dpi",
-            "pt",
-        ]:
+        # The value must be converted into picas points ------------------
+
+        if self.unit not in Dim.NOT_TO_PICAS:
             if no_useless_decimals:
                 pica = self.topica()
+
                 return str(decimals(pica))
-            else:
-                return str(self.topica())
-        else:
-            if self.unit == "pcdecim":
-                if self.value == 1.0:
-                    return "1"
-                else:
-                    if no_useless_decimals:
-                        return str(decimals(self.value))
-                    else:
-                        return str(self.value)
-            else:
-                if no_useless_decimals:
-                    return str(decimals(self.value))
-                else:
-                    return str(self.value)
 
-    def toxml(self):
+            return str(self.topica())
+
+        # Percentage as a decimal export ---------------------------------
+
+        if self.unit == "pcdecim":
+            if self.value == 1.0:
+                return "1"
+
+            if no_useless_decimals:
+                return str(decimals(self.value))
+
+            return str(self.value)
+
+        # Other units ----------------------------------------------------
+
+        if no_useless_decimals:
+            return str(decimals(self.value))
+
+        return str(self.value)
+
+    def toxml(self) -> str:
         """
         Alias of Dimension.toxmlstr()
 
         Returns a XML string of the dimension according to its unit.
 
         :rtype: str
         :return: str
         """
 
         return self.toxmlstr()
 
-    #--- Conversion into other units -------------------------------------
+    # Conversion into other units ----------------------------------------
 
-    def _ceil(self, value, ceil=False):
+    def _ceil(self, value, ceil: bool = False) -> Union[float, int]:
         """
         Ceil value if ceil is True.
 
         :type value: float,int
         :param value: Value to ceil (or not)
         :type ceil: boolean
         :param ceil: If True, apply ceil to value
         :rtype: float,int
         :return: Ceiled (or not) number
         """
 
         if ceil:
             return math.ceil(value)
-        else:
-            return value
 
-    def _convertorval(self, obj, value, unit):
+        return value
+
+    def _convertorval(self, obj, value, unit: str) -> Union[float, int, Dim]:
         """
         Returns a Dim object with unit <unit> if <obj>, or <value>.
 
         :rtype: float,int,Dim
         :return: Dim object or Dim value
         """
 
         if obj:
             return Dim(value, unit=unit)
 
         return value
 
-    def is_convertable_length(self):
+    def is_convertable_length(self) -> bool:
         """
         :rtype: boolean
         :return: If the Dim instance is a convertable length
         """
 
         return not (
             self.unit
-            in ["perc", "pcdecim", "pcscale", "cdeg", "deg", "dpi", "lpi"]
+            in ["perc", "pcdecim", "pcscale", "cdeg", "pdeg", "deg", "dpi", "lpi"]
         )
 
     def topica(
         self, ceil: bool = False, obj: bool = False
     ) -> Union[float, int, Dim]:
         """
         Returns the value of Dim in pica point unit.
@@ -404,15 +422,15 @@
         if self.unit == "pica":
             return self._convertorval(
                 obj, self._ceil(self.value, ceil), "pica"
             )
 
         if self.unit == "mm":
             return self._convertorval(
-                obj, self._ceil(self.value / Dim.PICA_TO_MM, ceil), "pica"
+                obj, self._ceil(self.value / PICA_TO_MM, ceil), "pica"
             )
 
     def todpi(
         self, ceil: bool = False, obj: bool = False
     ) -> Union[float, int, Dim]:
         """
         Returns the value of Dim in DPI unit.
@@ -421,41 +439,33 @@
         :type ceil: boolean
         :param ceil: If True, apply ceil to returned value
         :type obj: boolean
         :param obj: If True, returns a Dim object instead of value.
         """
 
         if self.unit == "lpi":
-            return self._convertorval(
-                obj, self._ceil(self.value * 16), "dpi"
-            )
-        else:
-            raise exceptions.IncompatibleDim(
-                "Can't convert that into DPI"
-            )
+            return self._convertorval(obj, self._ceil(self.value * 16), "dpi")
+
+        raise exceptions.IncompatibleDim("Can't convert that into DPI")
 
-    def topc(self, ceil, obj=False):
+    def topc(self, ceil: bool, obj: bool = False) -> Union[float, int, Dim]:
         """
         Returns the value of Dim as integer percentage.
         Raise ValueError if Dim is not convertable
 
         :type ceil: boolean
         :param ceil: If True, apply ceil to returned value
         :type obj: boolean
         :param obj: If True, returns a Dim object instead of value.
         """
 
-        if self.unit == "pcdecim":
-            return self._convertorval(
-                obj, self._ceil(self.value * 100), "pc"
-            )
-        else:
-            raise exceptions.IncompatibleDim(
-                "Can't convert that into percentage"
-            )
+        if self.unit in ["pcdecim", "pcscale"]:
+            return self._convertorval(obj, self._ceil(self.value * 100), "pc")
+
+        raise exceptions.IncompatibleDim("Can't convert that into percentage")
 
     def tolpi(
         self, ceil: bool = False, obj: bool = False
     ) -> Union[float, int, Dim]:
         """
         Returns the value of Dim in LPI unit.
         Raise ValueError if Dim is not convertable
@@ -463,21 +473,17 @@
         :type ceil: boolean
         :param ceil: If True, apply ceil to returned value
         :type obj: boolean
         :param obj: If True, returns a Dim object instead of value.
         """
 
         if self.unit == "dpi":
-            return self._convertorval(
-                obj, self._ceil(self.value / 16), "lpi"
-            )
-        else:
-            raise exceptions.IncompatibleDim(
-                "Can't convert that into LPI"
-            )
+            return self._convertorval(obj, self._ceil(self.value / 16), "lpi")
+
+        raise exceptions.IncompatibleDim("Can't convert that into LPI")
 
     def tomm(
         self, ceil: bool = False, obj: bool = False
     ) -> Union[float, int, Dim]:
         """
         Returns the value of Dim in milimeter unit.
 
@@ -490,131 +496,129 @@
         if not self.is_convertable_length():
             raise exceptions.IncompatibleDim(
                 "Can't convert that into milimeters"
             )
 
         if self.unit == "pica":
             return self._convertorval(
-                obj, self._ceil(self.value * Dim.PICA_TO_MM, ceil), "mm"
+                obj, self._ceil(self.value * PICA_TO_MM, ceil), "mm"
             )
 
         if self.unit == "mm":
-            return self._convertorval(
-                obj, self._ceil(self.value, ceil), "mm"
-            )
+            return self._convertorval(obj, self._ceil(self.value, ceil), "mm")
 
-    #--- Defaults --------------------------------------------------------
+    # Defaults -----------------------------------------------------------
 
-    def fromdefault(self, default):
+    def fromdefault(self, default: str) -> bool:
         """
         Set Dim attributes according to a named default.
 
         :type default: str
         :param default: Name of the set of defaults.
         :rtype: boolean
         :return: boolean
         """
 
         if default.startswith("a4-"):
             self.set_unit("pica")
 
-            if default == "a4-width":
-                self.value = iso216paper.A4.WIDTH
-
-            if default == "a4-height":
-                self.value = iso216paper.A4.HEIGHT
+            self.value = {
+                "a4-width": iso216paper.A4.WIDTH,
+                "a4-height": iso216paper.A4.HEIGHT,
+            }[default]
 
         if default.startswith("letter-"):
             self.set_unit("pica")
 
-            if default == "letter-width":
-                self.value = ansipaper.Letter.WIDTH
-
-            if default == "letter-height":
-                self.value = ansipaper.Letter.HEIGHT
+            self.value = {
+                "letter-width": ansipaper.Letter.WIDTH,
+                "letter-height": ansipaper.Letter.HEIGHT,
+            }[default]
 
         return True
 
-    #--- Python __ methods -----------------------------------------------
+    # Python __ methods --------------------------------------------------
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self.value)
 
-    def __str__(self):
-        r,u = str(self.value),""
+    def __str__(self) -> str:
+        r, u = str(self.value), ""
 
         if self.unit in Dim.UNIT_ARGS.keys():
             short = {"mm": "mm", "perc": "%", "pica": "pct", "lpi": "lpi"}
 
             if self.unit in short:
                 u = short[self.unit]
 
-            if self.unit in ["cdeg", "deg"]:
+            if self.unit in ["cdeg", "deg", "pdeg"]:
                 u = "°"
 
         else:
             raise exceptions.UnknownDimUnit(self.unit)
 
-        return "{} {}".format(r, u)
+        return f"{r} {u}"
 
     def __repr__(self):
         return "Dim(value={}, unit={}, integer={}, negative={})".format(
             self.value, self.unit, self.integer, self.allow_negative
         )
 
-    def __float__(self):
+    def __float__(self) -> float:
         return float(self.value)
 
-    def __int__(self):
+    def __int__(self) -> int:
         return int(self.value)
 
-    def __iadd__(self, dim):
+    def __iadd__(self, dim) -> Dim:
 
         if isinstance(dim, float):
             self.value += dim
 
         if isinstance(dim, Dim):
             if dim.unit == self.unit:
                 self.value += dim.value
             else:
                 raise exceptions.IncompatibleDim()
 
         return self
 
-    def __isub__(self, dim):
+    def __isub__(self, dim) -> Dim:
 
         if isinstance(dim, float):
             self.value -= dim
 
         if isinstance(dim, Dim):
             if dim.unit == self.unit:
                 self.value -= dim.value
             else:
                 raise exceptions.IncompatibleDim()
 
         return self
 
-    def __imul__(self, dim):
+    def __imul__(self, dim) -> Dim:
 
         if isinstance(dim, float):
             self.value *= dim
 
         if isinstance(dim, Dim):
             if dim.unit == self.unit:
                 self.value *= dim.value
             else:
                 raise exceptions.IncompatibleDim()
 
-    def __sub__(self, dim):
+        return self
+
+    def __sub__(self, dim) -> Dim:
         return self.__isub__(dim)
 
-    def __add__(self, dim):
+    def __add__(self, dim) -> Dim:
         return self.__iadd__(dim)
 
-    def __mul__(self, dim):
+    def __mul__(self, dim) -> Dim:
         return self.__imul__(dim)
 
 
 class DimBox:
     """
     Box/rectangle object to manipulate Scribus frames coordinates.
 
@@ -646,15 +650,15 @@
     +-------------------------+------------+
     | Box width               | width      |
     +-------------------------+------------+
     | Box height              | height     |
     +-------------------------+------------+
     """
 
-    def __init__(self,**kwargs):
+    def __init__(self, **kwargs):
         # X,Y coordinates for each corner
         # Use setx, sety, getx, gety methods as shorthands
         self.coords = {
             "top-left": [Dim(0), Dim(0)],
             "top-right": [Dim(0), Dim(0)],
             "bottom-left": [Dim(0), Dim(0)],
             "bottom-right": [Dim(0), Dim(0)],
@@ -674,22 +678,25 @@
             "bottom-right": [Dim(0), Dim(0)],
         }
 
         # -----------------------------------------------------------
 
         self.set_box(kwargs=kwargs)
 
-    #--- Shorthands for corners coordinates ------------------------------
+    # Shorthands for corners coordinates ---------------------------------
 
     def _setxy(
         self, corner: BoxCorner, value, xy: XY, rotated: bool = False
     ) -> bool:
         if corner.lower() in [
-                "top-left", "top-right",
-                "bottom-left", "bottom-right"]:
+            "top-left",
+            "top-right",
+            "bottom-left",
+            "bottom-right",
+        ]:
 
             if xy == "x":
                 if rotated:
                     self.rotated_coords[corner][0].value = value
                 else:
                     self.coords[corner][0].value = value
             else:
@@ -702,46 +709,49 @@
         else:
             raise KeyError()
 
     def _getxy(
         self, corner: BoxCorner, xy: XY, rotated: bool = False
     ) -> Union[float, int]:
         if corner.lower() in [
-                "top-left", "top-right",
-                "bottom-left", "bottom-right"]:
+            "top-left",
+            "top-right",
+            "bottom-left",
+            "bottom-right",
+        ]:
             if xy == "x":
                 if rotated:
                     return self.rotated_coords[corner][0].value
-                else:
-                    return self.coords[corner][0].value
+
+                return self.coords[corner][0].value
             else:
                 if rotated:
                     return self.rotated_coords[corner][1].value
-                else:
-                    return self.coords[corner][1].value
+
+                return self.coords[corner][1].value
         else:
             raise KeyError()
 
-    def setx(self, corner, value, rotated=False):
+    def setx(self, corner: BoxCorner, value, rotated: bool = False) -> bool:
         return self._setxy(corner, value, "x", rotated)
 
-    def sety(self, corner, value, rotated=False):
+    def sety(self, corner: BoxCorner, value, rotated: bool = False) -> bool:
         return self._setxy(corner, value, "y", rotated)
 
     def getx(
         self, corner: BoxCorner, rotated: bool = False
     ) -> Union[float, int]:
         return self._getxy(corner, "x", rotated)
 
     def gety(
         self, corner: BoxCorner, rotated: bool = False
     ) -> Union[float, int]:
         return self._getxy(corner, "y", rotated)
 
-    #--- Box modification ------------------------------------------------
+    # Box modification ---------------------------------------------------
 
     def move(
         self,
         posx: float = 0,
         posy: float = 0,
         refpoint: BoxCorner = "top-left",
     ) -> bool:
@@ -753,79 +763,86 @@
         :type posy: float
         :param posy: New Y position
         :type refpoint: string
         :param refpoint: Coordinate point of reference (DimBox.coords key)
         :rtype: boolean
         """
 
-        origin_x,origin_y = None,None
+        origin_x, origin_y = None, None
 
         if refpoint in self.coords.keys():
             origin_x = self.coords[refpoint][0].value
             origin_y = self.coords[refpoint][1].value
 
         if origin_x is not None and origin_y is not None:
 
             if origin_x != posx or origin_y != posy:
                 # Noving the box according to the reference point
 
                 if refpoint == "top-left":
                     self.set_box(
-                        top_lx=posx, top_ly=posy,
+                        top_lx=posx,
+                        top_ly=posy,
                         width=self.dims["width"].value,
                         height=self.dims["height"].value,
                     )
 
                     return True
 
             else:
                 # Moving the box at the exact same position is not a mistake
                 # even if it's useless
                 return True
 
         return False
 
-    def translate(self, amountx=0, amounty=0, refpoint="top-left"):
+    def translate(
+        self,
+        amountx: float = 0,
+        amounty: float = 0,
+        refpoint: BoxCorner = "top-left",
+    ) -> bool:
         """
         Move the box by an amount of amountx, amounty
 
         :type amountx: float
         :param amountx: Amount of X translation
         :type amounty: float
         :param amounty: Amount of Y translation
         :type refpoint: string
         :param refpoint: Coordinate point of reference (DimBox.coords key)
         :rtype: boolean
         """
 
-        origin_x,origin_y = None,None
+        origin_x, origin_y = None, None
 
         if refpoint in self.coords.keys():
             origin_x = self.coords[refpoint][0].value
             origin_y = self.coords[refpoint][1].value
 
         if origin_x is not None and origin_y is not None:
 
             # Translating the box by amountx, amounty
 
             if refpoint == "topleft":
                 npx = self.coords["top-left"][0].value + amountx
                 npy = self.coords["top-left"][1].value + amounty
 
                 self.set_box(
-                    top_lx=npx, top_ly=npy,
+                    top_lx=npx,
+                    top_ly=npy,
                     width=self.dims["width"].value,
                     height=self.dims["height"].value,
                 )
 
                 return True
 
         return False
 
-    def set_box(self, **kwargs):
+    def set_box(self, **kwargs) -> bool:
         """
         Set all coordinates of the box from a set a coordinates
         and/or width & height.
 
         +-------------------------+------------+
         | Box point coordinate    | kwargs key |
         +=========================+============+
@@ -859,16 +876,16 @@
             X-------X
 
             Height and width are deduced
 
             rtype: pyscribus.dimensions.DimBox
             """
 
-            tlx,tly = kwargs["top_lx"],kwargs["top_ly"]
-            brx,bry = kwargs["bottom_rx"],kwargs["bottom_ry"]
+            tlx, tly = kwargs["top_lx"], kwargs["top_ly"]
+            brx, bry = kwargs["bottom_rx"], kwargs["bottom_ry"]
 
             obj.dims["width"].value = brx - tlx
             obj.dims["height"].value = bry - tly
 
             obj.setx("top-right", brx)
             obj.sety("top-right", tly)
             obj.setx("top-left", tlx)
@@ -889,15 +906,15 @@
                      |
                      v
 
             rtype: pyscribus.dimensions.DimBox
             """
 
             # Troy to avoid using try and "tory".
-            # I don’t care about UK parties.
+            # I don’t care about UK politics.
             trox = float(kwargs["top_rx"])
             troy = float(kwargs["top_ry"])
             width = float(kwargs["width"])
             height = float(kwargs["height"])
 
             obj.dims["width"].value = width
             obj.dims["height"].value = height
@@ -952,15 +969,15 @@
             :rtype: string,boolean
             :returns: casename or False
             """
 
             case = False
 
             if casename == "set_from_all":
-                case =  ["top_lx", "top_ly", "bottom_rx", "bottom_ry"]
+                case = ["top_lx", "top_ly", "bottom_rx", "bottom_ry"]
 
             if casename == "set_from_tl":
                 case = ["top_lx", "top_ly", "width", "height"]
 
             if casename == "set_from_tr":
                 case = ["top_rx", "top_ry", "width", "height"]
 
@@ -1005,20 +1022,20 @@
                     self = from_tr(self, kwargs)
 
                 if rotation_deg:
                     self.rotated_coords = copy.deepcopy(self.coords)
                     self.rotate(rotation_deg)
 
                 return True
-            else:
-                return False
-        else:
+
             return False
 
-    def resize_side(self, side, value):
+        return False
+
+    def resize_side(self, side: str, value: float) -> bool:
         """
         Resize the box from a side.
 
         :type side: str
         :param side: Side of the box to resize from.
             Must be "left", "right", "top", "bottom".
         :type value: float
@@ -1050,18 +1067,18 @@
 
             if side == "bottom":
                 nby = self.gety("bottom-left") + value
                 self.sety("bottom-left", nby)
                 self.sety("bottom-right", nby)
 
             return True
-        else:
-            return False
 
-    def rotate(self, degree):
+        return False
+
+    def rotate(self, degree: float) -> bool:
         """
         Rotate the box by degree.
 
         .. warning:: NOT IMPLEMENTED YET & DON'T KNOW HOW TO
 
         :type degree: float
         :param degree: Degree of rotation
@@ -1080,15 +1097,15 @@
         #
         # NOTE It is crucial you don't modify Dim.coords, as in SLA
         # XML, only original box coords and rotation angle value
         # are saved.
 
         # FIXME Remove that after implementation -------
 
-        logger=logs.getLogger()
+        logger = logs.getLogger()
 
         if logger:
             logger.debug("Box rotation not implemented.")
             # logger.debug("Rotation degree : {}".format(degree))
         else:
             print("PyScribus - Box rotation not implemented.")
             # print("Rotation degree :", degree)
@@ -1098,29 +1115,29 @@
         valid = True
 
         if valid:
             self.rotation.value = degree
 
         return True
 
-    #--- Python __ methods -----------------------------------------------
+    # Python __ methods --------------------------------------------------
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         for cname in self.coords.keys():
 
-            for idx in [0,1]:
+            for idx in [0, 1]:
                 a = self.coords[cname][idx].value
                 b = other.coords[cname][idx].value
 
                 if not a == b:
                     return False
 
         return True
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "X {} Y {} Width {} Height {}".format(
             self.coords["top-left"][0].value,
             self.coords["top-left"][1].value,
             self.dims["width"],
             self.dims["height"],
         )
 
@@ -1157,8 +1174,9 @@
     +-------------------------+------------+
     """
 
     def __init__(self, **kwargs):
         DimBox.__init__(self)
         self.visible = True
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/document.py` & `pyscribus-backported-0.3/pyscribus/model/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,198 +19,384 @@
 
 """
 Document classes
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+from typing import Union, NoReturn, Optional, Any, List
+from collections import OrderedDict
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
-import pyscribus.dimensions as dimensions
-import pyscribus.colors as pscolors
-import pyscribus.toc as toc
-import pyscribus.marks as marks
-import pyscribus.pages as pages
-import pyscribus.styles as styles
-import pyscribus.itemattribute as itemattribute
-import pyscribus.patterns as patterns
-import pyscribus.pageobjects as pageobjects
-import pyscribus.notes as notes
-import pyscribus.printing as printing
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.colors as pscolors
+import pyscribus.model.toc as toc
+import pyscribus.model.marks as marks
+import pyscribus.model.pages as pages
+import pyscribus.model.styles as styles
+import pyscribus.model.itemattribute as itemattribute
+import pyscribus.model.patterns as patterns
+import pyscribus.model.layers as layers
+import pyscribus.model.pageobjects as pageobjects
+import pyscribus.model.notes as notes
+import pyscribus.model.printing as printing
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
+BoolOrElement = Union[bool, ET.Element]
+
+AppendableToDocument = Union[
+    pageobjects.PageObject,
+    pages.PageAbstract,
+    layers.Layer,
+    pscolors.Color,
+    styles.StyleAbstract,
+]
+
 # Classes ===============================================================#
 
+
 class Document(PyScribusElement):
     """
     SLA Document (DOCUMENT) in SLA file.
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     """
 
-    metadata_xml = {
-        "AUTHOR": "author", "COMMENTS": "comments", "PUBLISHER": "publisher",
-        "DOCDATE": "date", "DOCTYPE": "type", "DOCFORMAT": "format",
-        "DOCIDENT": "identifier", "DOCSOURCE": "source", "DOCLANGINFO": "lang",
-        "DOCRELATION": "related", "DOCCOVER": "cover", "DOCRIGHTS": "rights",
-        "TITLE": "title", "SUBJECT": "subject", "DOCCONTRIB": "contributor"
-    }
-
-    ui_show_xml = {
-        "SHOWMARGIN": "margins", "SHOWBASE": "baseline", "SHOWPICT": "images",
-        "SHOWLINK": "links", "SHOWGRID": "grid", "SHOWGUIDES": "guides",
-        "showcolborders": "colborders", "showrulers": "rulers"
+    metadata_xml = OrderedDict(
+        AUTHOR="author",
+        COMMENTS="comments",
+        KEYWORDS="keywords",
+        PUBLISHER="publisher",
+        DOCDATE="date",
+        DOCTYPE="type",
+        DOCFORMAT="format",
+        DOCIDENT="identifier",
+        DOCSOURCE="source",
+        DOCLANGINFO="lang",
+        DOCRELATION="related",
+        DOCCOVER="cover",
+        DOCRIGHTS="rights",
+        DOCCONTRIB="contributor",
+        TITLE="title",
+        SUBJECT="subject",
+    )
+
+    ui_show_xml = OrderedDict(
+        SHOWGRID="grid",
+        SHOWGUIDES="guides",
+        showcolborders="colborders",
+        SHOWFRAME="frames",
+        SHOWControl="caracters",
+        SHOWLAYERM="layer_hints",
+        SHOWMARGIN="margins",
+        SHOWBASE="baseline",
+        SHOWPICT="images",
+        SHOWLINK="links",
+        # rulerMode
+        showrulers="rulers",
+        showBleed="bleeds",
+    )
+
+    icc_xml = OrderedDict(
+        DPPr="printer",
+        DPIn="rgb_images",
+        DPInCMYK="cmyk_images",
+        DPIn2="rgb_colors",
+        DPIn3="cmyk_colors",
+    )
+
+    autoframes_xml = OrderedDict(
+        AUTOSPALTEN="columns",
+        ABSTSPALTEN="colgap",
+    )
+
+    bleed_xml = OrderedDict(
+        BleedTop="top",
+        BleedLeft="left",
+        BleedRight="right",
+        BleedBottom="bottom",
+    )
+
+    scratchspace_xml = OrderedDict(
+        ScratchBottom="bottom",
+        ScratchLeft="left",
+        ScratchRight="right",
+        ScratchTop="top",
+        GapHorizontal="horizontal_gap",
+        GapVertical="vertical_gap",
+    )
+
+    units_xml = {
+        "0": "points",
+        "1": "millimeters",
+        "2": "inches",
+        "3": "picas",
+        "4": "centimeters",
+        "5": "ciceros",
     }
 
-    autoframes_xml = {
-        "AUTOSPALTEN": "columns",
-        "ABSTSPALTEN": "colgap",
-    }
-
-    bleed_xml = {
-        "BleedTop": "top", "BleedRight": "right", "BleedLeft": "left",
-        "BleedBottom": "bottom"
+    ui_stack = {
+        "0": "objects",
+        "1": "guides",
+        "2": "grids",
+        "3": "baseline",
+        "4": "margins",
     }
 
     def __init__(self, sla_parent=False):
         super().__init__()
 
         self.sla_parent = sla_parent
 
-        #-----------------------------------------------
+        self.units = "points"
+
+        # ----------------------------------------------
 
         self.profiles = []
         self.pdf_settings = []
         self.printer_settings = []
 
-        #-----------------------------------------------
+        # ----------------------------------------------
+
+        self.hyphenation = None
+
+        # ----------------------------------------------
 
         self.colors = []
         self.layers = []
         self.patterns = []
         self.gradients = []
 
-        #-----------------------------------------------
+        # ----------------------------------------------
 
         self.pages = []
         self.page_sets = []
+        self.page_number = 0
         self.master_pages = []
         self.page_objects = []
 
-        #-----------------------------------------------
+        # ----------------------------------------------
 
         self.tocs = []
         self.marks = []
         self.sections = []
 
-        #-----------------------------------------------
-
-        self.page_number = 0
+        # ----------------------------------------------
 
         # Page dimensions, borders, bleeds
 
         self.dims = {
             "width": dimensions.Dim(595.275590551181),
-            "height": dimensions.Dim(841.889763779528)
+            "height": dimensions.Dim(841.889763779528),
         }
 
         self.borders = {
-            "left": dimensions.Dim(40), "right": dimensions.Dim(40),
-            "top": dimensions.Dim(40), "bottom": dimensions.Dim(40)
+            "left": dimensions.Dim(40),
+            "right": dimensions.Dim(40),
+            "top": dimensions.Dim(40),
+            "bottom": dimensions.Dim(40),
         }
 
-
         self.bleed = {
-            "top": dimensions.Dim(0), "right": dimensions.Dim(0),
-            "left": dimensions.Dim(0), "bottom": dimensions.Dim(0)
+            "top": dimensions.Dim(0),
+            "right": dimensions.Dim(0),
+            "left": dimensions.Dim(0),
+            "bottom": dimensions.Dim(0),
+        }
+
+        self.scratchspace = {
+            # Space at the top of the scratch space, before the pages
+            "top": dimensions.Dim(20),
+            # Space at the right of the scratch space
+            "right": dimensions.Dim(100),
+            # Space at the left of the scratch space
+            "left": dimensions.Dim(100),
+            # Space at the bottom of the scratch space, after the last page
+            "bottom": dimensions.Dim(20),
+            # Horizontal gap between two pages
+            "horizontal_gap": dimensions.Dim(0),
+            # Vertical gap between two pages
+            "vertical_gap": dimensions.Dim(40),
+        }
+
+        self.grids = {
+            "minor": {
+                "spacing": dimensions.Dim(20),
+                "color": "#00ff00",
+            },
+            "major": {
+                "spacing": dimensions.Dim(100),
+                "color": "#00ff00",
+            },
+            "baseline": {
+                "spacing": dimensions.Dim(14.4, unit="pt"),
+                "offset": dimensions.Dim(0, unit="pt"),
+                "color": "#c0c0c0",
+            },
         }
 
-        #-----------------------------------------------
+        # ----------------------------------------------
 
         self.notes = []
         self.notes_frames = []
 
         self.styles = {
             "note": [],
             "paragraph": [],
             "character": [],
             "table": [],
             "cell": [],
         }
 
-        #-----------------------------------------------
+        # ----------------------------------------------
 
         self.attributes = []
 
         # ----------------------------------------------
 
         self.metadata = {
-            "title": "", "author": "", "subject": "", "keywords": [],
-            "comments": "", "publisher": "", "contributor": "",
-            "date": "", "type": "", "format": "", "identifier": "",
-            "source": "", "lang": "", "related": "", "cover": "",
+            "title": "",
+            "author": "",
+            "subject": "",
+            "keywords": None,
+            "comments": "",
+            "publisher": "",
+            "contributor": "",
+            "date": "",
+            "type": "",
+            "format": "",
+            "identifier": "",
+            "source": "",
+            "lang": "",
+            "related": "",
+            "cover": "",
             "rights": "",
         }
 
-        #--- ICC color profiles ------------------------
+        # ICC color profiles ---------------------------
 
         self.icc_profiles = {
-            "rgb_images": "", "cmyk_images": "",
-            "rgb_colors": "", "cmyk_colors": "",
+            "rgb_images": "",
+            "cmyk_images": "",
+            "rgb_colors": "",
+            "cmyk_colors": "",
             "printer": "",
         }
 
         # ----------------------------------------------
 
-        self.ui_snapping = {"guides": False, "grid": False, "element": False}
+        self.ui_snapping = OrderedDict(
+            guides=False,
+            grid=False,
+            element=False,
+        )
 
         # ----------------------------------------------
 
         self.ui_show = {
-            "margins": True,
             "baseline": False,
-            "images": True,
-            "links": False,
+            "bleeds": True,
+            "caracters": False,
+            "colborders": True,
             "grid": False,
             "guides": True,
-            "colborders": True,
-            "rulers": True
-        }
-
-        # ----------------------------------------------
-
-        self.calligraphicpen = {
-            "angle": dimensions.Dim(0, unit="cdeg", integer=True),
-            "line_width": dimensions.Dim(0, unit="pica"),
-            "line_shade": dimensions.Dim(100, unit="perc", integer=True),
-            "line_color": "",
-            "width": dimensions.Dim(0, unit="pica"),
-            "style": "1",
-            "fill_color": "",
-            "fill_shade": dimensions.Dim(100, unit="perc", is_int=True),
+            "images": True,
+            "layer_hints": False,
+            "links": False,
+            "margins": True,
+            "rulers": True,
+            "stack": [
+                # Default is 2 0 4 1 3
+                "grids",
+                "objects",
+                "margins",
+                "guides",
+                "baseline",
+            ]
         }
 
         # ----------------------------------------------
 
         self.autoframes = {
             # Number of Columns in automatic Textframes
             # AUTOSPALTEN = "1"
             "columns": 1,
             # Distance between Columns in automatic Textframes
             # ABSTSPALTEN = "11"
-            "colgap": dimensions.Dim(11, unit="pt")
+            "colgap": dimensions.Dim(11, unit="pt"),
+        }
+
+        # Default settings for tools -------------------
+
+        self.tools = {
+            "text": {
+                "font": None,
+                "size": dimensions.Dim(12, unit="pt"),
+                "columns": 1,
+                "columns_gap": dimensions.Dim(0),
+            },
+            "shape": {
+                "pen": {
+                    "color": "Black",
+                    "shade": dimensions.Dim(100, unit="perc", is_int=True)
+                },
+                "brush": {
+                    "color": "None",
+                    "shade": dimensions.Dim(100, unit="perc", is_int=True)
+                },
+                "style": 1,
+                "width": dimensions.Dim(1, unit="pica"),
+            },
+            "polygon": {
+                "sides": 4,
+                "rotation": dimensions.Dim(0, unit="pdeg", integer=True),
+                # Convex/Concave polygon
+                "convconc": {
+                    "active": False,
+                    # POLYF = intensity. Unknown numeric type:
+                    # Value             GUI
+                    # 0                 -100
+                    # 0.923879532511287 0
+                    # 1.08239220029239  100
+                    "intensity": float(0),
+                    "curb_in": dimensions.Dim(0, unit="pcdecim"),
+                    "curb_out": dimensions.Dim(0, unit="pcdecim"),
+                    "rot_in": dimensions.Dim(0, unit="pdeg", integer=True),
+                }
+            },
+            "line": {
+                "arrows": {"start": 0, "end": 0},
+                "color": "Black",
+                "style": 1,
+                "width": dimensions.Dim(1, unit="pica"),
+                "shade": dimensions.Dim(100, unit="perc", is_int=True)
+            },
+            "calligraphicpen": {
+                "angle": dimensions.Dim(0, unit="cdeg", integer=True),
+                "line_width": dimensions.Dim(0, unit="pica"),
+                "line_shade": dimensions.Dim(100, unit="perc", integer=True),
+                "line_color": "",
+                "width": dimensions.Dim(0, unit="pica"),
+                "style": 1,
+                "fill_color": "",
+                "fill_shade": dimensions.Dim(100, unit="perc", is_int=True),
+            }
         }
 
         # ----------------------------------------------
 
         # FIXME Not documented -------------------------
         # PRESET="0"
 
@@ -225,389 +411,344 @@
             "size": pages.xml_size["A4"],
             # (optional) Which PageSet to use
             # This value is the index of page set used. And it is NOT optional.
             # So by default,
             # 0 is Single page, 1 is Facing pages, 2 is 3-Fold, 3 is 4-Fold
             # BOOK = "0"
             # TODO : Link this value to pages sets in Document object
-            "set": 0
+            "set": 0,
         }
 
         # (optional) First page number in the Doc
         FIRSTNUM = "1"
 
-        # (optional) Measurement unit for the Doc
-        # 0 = Points 1 = Millimeters 2 = Inches 3 = Picas
-        UNITS="1"
-
-        # Default Font
-        DFONT="Arial Regular"
-        # Default Fontsize
-        DSIZE="12"
-
-        # (optional) Number of Columns in Textframes
-        DCOL="1"
-        # (optional) Default Gap between Columns in Textframes
-        DGAP="0"
-
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # TabFill=""
 
         # Default width for tabs in text frames
-        TabWidth="36"
+        TabWidth = "36"
 
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # TextDistLeft="0"
         # TextDistRight="0"
         # TextDistBottom="0"
         # TextDistTop="0"
 
         # FIXME ---- À faire ---------------------------
 
         # Percentage for Superscript
-        VHOCH="33"
+        VHOCH = "33"
         # Percentage for scaling of the Glyphs in Superscript
-        VHOCHSC="66"
+        VHOCHSC = "66"
         # Percentage for Subscript
-        VTIEF="33"
+        VTIEF = "33"
         # Percentage for scaling of the Glyphs in Subscript
-        VTIEFSC="66"
+        VTIEFSC = "66"
         # Percentage for scaling of the Glyphs in Small Caps
-        VKAPIT="75"
+        VKAPIT = "75"
 
-        # (optional) Width of the Baseline Grid
-        BASEGRID="14.4"
-        # (optional) Startoffset for the Baseline Grid
-        BASEO="0"
-
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # AUTOL="100"
         # UnderlinePos="-1"
         # UnderlineWidth="-1"
         # StrikeThruPos="-1"
         # StrikeThruWidth="-1"
 
         # (optional) Counter for Groups in the Doc
-        GROUPC="1"
+        GROUPC = "1"
         # (optional) Colormanagement available 0 = off, 1 = on
-        HCMS="0"
+        HCMS = "0"
         # (optional) Simulate the Printer on Screen 0 = off, 1 = on
-        DPSo="0"
+        DPSo = "0"
 
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # DPSFo="0"
 
         # (optional) Use Colormanagement 0 = off, 1 = on
-        DPuse="0"
+        DPuse = "0"
         # (optional) Mark Colors out of Gamut 0 = off, 1 = on
-        DPgam="0"
+        DPgam = "0"
         # (optional) Use Blackpoint Compensation 0 = off, 1 = on
-        DPbla="1"
+        DPbla = "1"
 
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # DISc="1"
         # DIIm="0"
 
         # (optional) Active Layer
-        ALAYER="0"
+        ALAYER = "0"
 
         # (optional) Language of the Doc
-        LANGUAGE="fr"
+        LANGUAGE = "fr"
         # (optional) Automatic Hyphenation 0 = off, 1 = on
-        AUTOMATIC="1"
+        AUTOMATIC = "1"
         # (optional) Automatic Hyphenation during typing 0 = off, 1 = on
-        AUTOCHECK="0"
+        AUTOCHECK = "0"
         # (optional) Guides locked 0 = off, 1 = on
-        GUIDELOCK="0"
+        GUIDELOCK = "0"
 
         # FIXME ---- À faire ---------------------------
 
-        # (optional) Distance of the minor Gridlines
-        MINGRID="20"
-        # (optional) Distance of the major Gridlines
-        MAJGRID="100"
-
-        #--- FIXME Not documented ----------------------
-        # SHOWFRAME="1"
-        # SHOWControl="0"
-        # SHOWLAYERM="0"
-
-        # FIXME ---- À faire ---------------------------
-
-        #--- FIXME Not documented ----------------------
+        # FIXME Not documented -------------------------
         # rulerMode="1"
 
-        #--- FIXME Not documented ----------------------
-        # showBleed="1"
+        # FIXME Not documented -------------------------
         # rulerXoffset="0"
         # rulerYoffset="0"
         # GuideRad="10"
         # GRAB="4"
-        # POLYC="4"
-        # POLYF="0.5"
-        # POLYR="0"
-        # POLYIR="0"
-        # POLYCUR="0"
-        # POLYOCUR="0"
-        # POLYS="0"
         # arcStartAngle="30"
         # arcSweepAngle="300"
         # spiralStartAngle="0"
         # spiralEndAngle="1080"
         # spiralFactor="1.2"
         # AutoSave="1"
         # AutoSaveTime="600000" # milisec ?
         # AutoSaveCount="1"
         # AutoSaveKeep="0"
         # AUtoSaveInDocDir="1"
         # AutoSaveDir=""
 
-        # Space at the bottom of the scratch space, after the last page
-        ScratchBottom="20"
-        # Space at the left of the scratch space
-        ScratchLeft="100"
-        # Space at the right of the scratch space
-        ScratchRight="100"
-        # Space at the top of the scratch space, before the pages
-        ScratchTop="20"
-
-        #--- FIXME Not documented ----------------------
-        # GapHorizontal="0"
-        # GapVertical="40"
-        # StartArrow="0"
-        # EndArrow="0"
-        # PEN="Black"
-        # BRUSH="None"
-        # PENLINE="Black"
+        # FIXME Not documented -------------------------
         # PENTEXT="Black"
         # StrokeText="Black"
         # TextBackGround="None"
         # TextLineColor="None"
         # TextBackGroundShade="100"
         # TextLineShade="100"
         # TextPenShade="100"
         # TextStrokeShade="100"
-        # STIL="1"
-        # STILLINE="1"
-        # WIDTH="1"
-        # WIDTHLINE="1"
-        # PENSHADE="100"
-        # LINESHADE="100"
-        # BRUSHSHADE="100"
         # CPICT="None"
         # PICTSHADE="100"
         # CSPICT="None"
         # PICTSSHADE="100"
         # PICTSCX="1"
         # PICTSCY="1"
         # PSCALE="1"
         # PASPECT="1"
         # EmbeddedPath="0"
         # HalfRes="1"
         # dispX="10"
         # dispY="10"
         # constrain="15"
 
-        # MINORC="#00ff00"
-        # MAJORC="#00ff00"
         # GuideC="#000080"
-        # BaseC="#c0c0c0"
 
         # Scribus GUI Page background
-        PAGEC="#ffffff"
+        PAGEC = "#ffffff"
 
         # MARGC="#0000ff"
 
-        # renderStack="2 0 4 1 3"
         # GridType="0"
         # RANDF="0"
 
         # currentProfile="PDF 1.4"
 
-
         # ----------------------------------------------
 
-    #=== Setting defaults methods ===========================================
+    # Setting defaults methods ==============================================
 
-    def _default_profiles(self):
+    def _default_profiles(self) -> NoReturn:
         """
         Add default checking profiles.
         """
 
         for def_name in Profile.defaults:
             self.profiles.append(Profile(default=def_name))
 
-    def _default_layer(self):
+    def _default_layer(self) -> NoReturn:
         """
         Add default layer.
         """
-        self.layers.append(Layer(default=True))
+        self.layers.append(layers.Layer(default=True))
 
-    def _default_layers(self):
+    def _default_layers(self) -> NoReturn:
         """
         Add default checking profiles.
 
         Alias for add_default_layer()
         """
 
         self._default_layer()
 
-    def _default_snapping(self):
+    def _default_snapping(self) -> NoReturn:
         """
         Set default UI snapping options.
         """
 
         self.ui_snapping = {"guides": True, "grid": False, "element": True}
 
-    def _default_note_style(self):
+    def _default_note_style(self) -> NoReturn:
         ns = styles.NoteStyle()
         ns.fromdefault()
 
         self.styles["note"].append(ns)
 
-    def _default_note_styles(self):
+    def _default_note_styles(self) -> NoReturn:
         self._default_note_style()
 
-    def _default_pages(self):
+    def _default_pages(self) -> bool:
         """
         Add default page.
         """
 
         page = pages.Page()
         page.fromdefault()
         self.pages.append(page)
 
         return True
 
-    def _default_page(self):
+    def _default_page(self) -> NoReturn:
         """
         Alias of default_pages()
 
         .. sealso: default_pages()
         """
 
         self._default_pages()
 
-    def _default_icc(self):
+    def _default_icc(self) -> NoReturn:
         """
         Set default ICC colors profiles.
         """
         self.icc_profiles = {
             "rgb_images": "sRGB display profile (ICC v2.2)",
             "cmyk_images": "ISO Coated v2 300% (basICColor)",
             "rgb_colors": "sRGB display profile (ICC v2.2)",
             "cmyk_colors": "ISO Coated v2 300% (basICColor)",
             "printer": "ISO Coated v2 300% (basICColor)",
         }
 
-    def _default_ui_show(self):
+    def _default_ui_show(self) -> NoReturn:
         """
         Set default UI view options.
         """
 
         self.ui_show = {
-            "margins": True,
             "baseline": False,
-            "images": True,
-            "links": False,
+            "bleeds": True,
+            "caracters": False,
+            "colborders": True,
             "grid": False,
             "guides": True,
-            "colborders": True,
-            "rulers": True
+            "images": True,
+            "layer_hints": False,
+            "links": False,
+            "margins": True,
+            "rulers": True,
+            "stack": [
+                "grids",
+                "objects",
+                "margins",
+                "guides",
+                "baseline",
+            ]
         }
 
-    def _default_calligraphic_pen(self):
+    def _default_calligraphic_pen(self) -> NoReturn:
         """
         Set default calligraphic pen options.
         """
 
-        self.calligraphicpen = {
+        self.tools["calligraphicpen"] = {
             "angle": dimensions.Dim(0, unit="cdeg", integer=True),
             "line_width": dimensions.Dim(0, unit="pica"),
             "line_shade": dimensions.Dim(100, unit="perc", integer=True),
             "line_color": "",
             "width": dimensions.Dim(0, unit="pica"),
             "style": 1,
             "fill_color": "",
             "fill_shade": dimensions.Dim(100, unit="perc", integer=True),
         }
 
-    def _default_pagesets(self):
+    def _default_pagesets(self) -> NoReturn:
         """
         Set default page sets.
         """
 
         self.page_sets = []
 
         for default in ["Single Page", "Facing Pages", "3-Fold", "4-Fold"]:
             ps = pages.PageSet()
 
             success = ps.fromdefault(default)
             if success:
                 self.page_sets.append(ps)
 
-    def _default_colors(self):
+    def _default_colors(self) -> NoReturn:
         """
         Set default colors.
         """
 
         for default in [
-            "Black", "Blue", "Cool Black", "Cyan", "Green", "Magenta", "Red",
-            "Registration", "Rich Black", "Warm Black", "White", "Yellow"]:
+            "Black",
+            "Blue",
+            "Cool Black",
+            "Cyan",
+            "Green",
+            "Magenta",
+            "Red",
+            "Registration",
+            "Rich Black",
+            "Warm Black",
+            "White",
+            "Yellow",
+        ]:
 
             co = pscolors.Color()
             success = co.fromdefault(default)
 
             if success:
                 self.colors.append(co)
 
-    def _default_pdfsettings(self):
+    def _default_pdfsettings(self) -> NoReturn:
         """
         Add default PDF settings.
         """
 
         pdf = printing.PDFSettings()
         pdf.fromdefault()
         self.pdf_settings = [pdf]
 
-    def _default_section(self):
+    def _default_section(self) -> NoReturn:
         """
         Alias of default_sections()
 
         .. sealso: default_section()
         """
 
         self.default_sections()
 
-    def _default_sections(self):
+    def _default_sections(self) -> NoReturn:
         """
         Add default section.
         """
 
         sec = toc.Section()
         sec.fromdefault()
         self.sections = [sec]
 
-    def _default_paragraph_styles(self):
+    def _default_paragraph_styles(self) -> NoReturn:
         self.styles["paragraph"].append(
             styles.ParagraphStyle(self, default=True)
         )
         self.styles["paragraph"][-1].is_default = True
 
-    def _default_character_styles(self):
+    def _default_character_styles(self) -> NoReturn:
         self.styles["character"].append(
             styles.CharacterStyle(self, default=True)
         )
         self.styles["character"][-1].is_default = True
 
-    def fromdefault(self, default="all"):
+    def fromdefault(self, default: str = "all") -> NoReturn:
         """
         Set default settings from a default list
 
-        :param default: Set of default settings or list of default features to set.
+        :param default: Set of default settings or list of default features
+            to set.
         :type default: str,list
 
         Unlike other fromdefault() methods, Document.fromdefault() default
         parameter can only be "all" or a list of default features to set.
 
         +-------------------------+-------------------+
         | Default feature         | String            |
@@ -660,18 +801,15 @@
             "pdf": self._default_pdfsettings,
             "profiles": self._default_profiles,
             "section": self._default_sections,
             "uisnapping": self._default_snapping,
             "uishow": self._default_ui_show,
         }
 
-        plurals = {
-            "pages": "page",
-            "sections": "section"
-        }
+        plurals = {"pages": "page", "sections": "section"}
 
         seq = []
 
         if default == "all":
             seq = features.keys()
         else:
             for f in default:
@@ -685,701 +823,1197 @@
 
                     if f in plurals:
                         seq.append(plurals[f])
 
         for f in seq:
             features[f]()
 
-    #========================================================================
+    # =======================================================================
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         # --- DOCUMENT attributes ----------------------------------------
-        # TODO DOCUMENT many attribs…
 
-        # Pages settings
+        # Default settings for Scribus' tools -----------------------
+
+        # Text tool __________________________________
+
+        text_tool_font = xml.get("DFONT")
+        if text_tool_font is not None:
+            self.tools["text"]["font"] = text_tool_font
+
+        text_tool_size = xml.get("DSIZE")
+        if text_tool_size is not None:
+            self.tools["text"]["size"].value = float(text_tool_size)
+
+        text_tool_columns = xml.get("DCOL")
+        if text_tool_columns is not None:
+            self.tools["text"]["columns"] = int(text_tool_columns)
+
+        text_tool_colsgap = xml.get("DGAP")
+        if text_tool_colsgap is not None:
+            self.tools["text"]["columns_gap"].value = float(text_tool_colsgap)
+
+        # Shape tool _________________________________
+
+        shape_tool_style = xml.get("STIL")
+        if shape_tool_style is not None:
+            shape_tool_style = int(shape_tool_style)
+
+            # Shape tool line style range from 0 to 37
+            if shape_tool_style > 37 or shape_tool_style < 0:
+                shape_tool_style = 0
+
+            self.tools["shape"]["style"] = shape_tool_style
+
+        shape_tool_width = xml.get("WIDTH")
+        if shape_tool_width is not None:
+            self.tools["shape"]["width"].value = float(shape_tool_width)
+
+        shape_tool_pen_shade = xml.get("PENSHADE")
+        if shape_tool_pen_shade is not None:
+            self.tools["shape"]["pen"]["shade"].value = int(shape_tool_pen_shade)
+
+        shape_tool_brush_shade = xml.get("BRUSHSHADE")
+        if shape_tool_brush_shade is not None:
+            self.tools["shape"]["brush"]["shade"].value = int(shape_tool_brush_shade)
+
+        shape_tool_pen_color = xml.get("PEN")
+        if shape_tool_pen_color is not None:
+            self.tools["shape"]["pen"]["color"] = shape_tool_pen_color
+
+        shape_tool_brush_color = xml.get("BRUSH")
+        if shape_tool_brush_color is not None:
+            self.tools["shape"]["brush"]["color"] = shape_tool_brush_color
+
+        # Line tool __________________________________
+
+        for att_name, human in [["StartArrow", "start"], ["EndArrow", "end"]]:
+
+            att = xml.get(att_name)
+            if att is not None:
+                att = int(att)
+
+                # Arrows type for line tool range from 0 to 36
+                if att > 36 or att < 0:
+                    att = 0
+
+                self.tools["line"]["arrows"][human] = att
+
+        line_tool_width = xml.get("WIDTHLINE")
+        if line_tool_width is not None:
+            self.tools["line"]["width"].value = float(line_tool_width)
+
+        line_tool_shade = xml.get("LINESHADE")
+        if line_tool_shade is not None:
+            self.tools["line"]["shade"].value = int(line_tool_shade)
+
+        line_tool_color = xml.get("PENLINE")
+        if line_tool_color is not None:
+            self.tools["line"]["color"] = line_tool_color
+
+        line_tool_style = xml.get("STILLINE")
+        if line_tool_style is not None:
+            line_tool_style = int(line_tool_style)
+
+            # Line tool line style range from 0 to 37
+            if line_tool_style > 37 or line_tool_style < 0:
+                line_tool_style = 0
+
+            self.tools["line"]["style"] = line_tool_style
+
+        # Poylgon tool _______________________________
+
+        poly_tool_convconc = xml.get("POLYS")
+        if poly_tool_convconc is not None:
+            self.tools["polygon"]["convconc"]["active"] = num_to_bool(
+                poly_tool_convconc
+            )
 
-        orientation = xml.get("orientation")
-        if orientation is not None:
-            if int(orientation):
+        poly_tool_sides = xml.get("POLYC")
+        if poly_tool_sides is not None:
+            self.tools["polygon"]["sides"] = int(poly_tool_sides)
+
+        poly_tool_rot = xml.get("POLYR")
+        if poly_tool_rot is not None:
+            self.tools["polygon"]["rotation"].value = int(poly_tool_rot)
+
+        poly_tool_cc_intensity = xml.get("POLYF")
+        if poly_tool_cc_intensity is not None:
+            self.tools["polygon"]["convconc"]["intensity"] = float(
+                poly_tool_cc_intensity
+            )
+
+        for att_name, human in [
+                ["POLYR", "rot_in"], ["POLYCUR", "curb_in"],
+                ["POLYOCUR", "curb_out"]]:
+            att = xml.get(att_name)
+            if att is not None:
+                if human == "rot_in":
+                    att = int(att)
+                else:
+                    att = float(att)
+
+                self.tools["polygon"]["convconc"][human].value = att
+
+        # Calligraphic pen tool ______________________
+
+        for att_base, key in [
+            ["Angle", "angle"],
+            ["LineColorShade", "line_shade"],
+            ["FillColorShade", "fill_shade"],
+        ]:
+            att_name = f"calligraphicPen{att_base}"
+
+            att = xml.get(att_name)
+            if att is not None:
+                self.tools["calligraphicpen"][key].value = int(att)
+
+        for att_base, key in [["LineWidth", "line_width"], ["Width", "width"]]:
+            att_name = f"calligraphicPen{att_base}"
+
+            att = xml.get(att_name)
+            if att is not None:
+                self.tools["calligraphicpen"][key].value = float(att)
+
+        for att_base, key in [
+            ["LineColor", "line_color"],
+            ["FillColor", "fill_color"],
+            ["PenStyle", "style"],
+        ]:
+
+            att_name = f"calligraphicPen{att_base}"
+
+            att = xml.get(att_name)
+            if att is not None:
+                if att_base == "PenStyle":
+                    self.tools["calligraphicpen"][key] = int(att)
+                else:
+                    self.tools["calligraphicpen"][key] = att
+
+        # Document units --------------------------------------------
+
+        doc_units = xml.get("UNITS")
+        if doc_units is not None:
+            self.units = Document.units_xml[doc_units]
+
+        # Scratch space ---------------------------------------------
+
+        for att_name, human in Document.scratchspace_xml.items():
+            att = xml.get(att_name)
+            if att is not None:
+                self.scratchspace[human].value = float(att)
+
+        # Borders ---------------------------------------------------
+
+        for border in ["LEFT", "RIGHT", "TOP", "BOTTM"]:
+            border_side = xml.get(f"BORDER{border}")
+            if border_side is not None:
+                self.borders[border.lower()].value = float(border_side)
+
+        # Pages settings --------------------------------------------
+
+        pagenumber = xml.get("ANZPAGES")
+        if pagenumber is not None:
+            self.page_number = int(pagenumber)
+
+        att_value = xml.get("orientation")
+        if (att_value = xml.get("orientation")) is not None:
+            if int(att_value):
                 self.doc_pages["orientation"] = pages.Orientation.LANDSCAPE
             else:
                 self.doc_pages["orientation"] = pages.Orientation.PORTRAIT
 
-        pagesize = xml.get("PAGESIZE")
-        if pagesize is not None:
+        att_value = xml.get("PAGESIZE")
+        if att_value is not None:
             for att, human in pages.xml_size.items():
-                if pagesize == att:
-                    self.doc_pages["size"] = pages.xml_size[pagesize]
+                if att_value == att:
+                    self.doc_pages["size"] = pages.xml_size[att_value]
                     break
 
-        book = xml.get("BOOK")
-        if book is not None:
-            self.doc_pages["set"] = int(book)
+        for page_dim in ["WIDTH", "HEIGHT"]:
+            pgdim = xml.get(f"PAGE{page_dim}")
+            if pgdim is not None:
+                self.dims[page_dim.lower()].value = float(pgdim)
+
+        att_value = xml.get("BOOK")
+        if att_value is not None:
+            self.doc_pages["set"] = int(att_value)
 
-        # Metadatas
+        # Metadatas -------------------------------------------------
 
         for att, key in Document.metadata_xml.items():
-            v = xml.get(att)
-            if v is not None:
-                self.metadata[key] = v
+            meta_value = xml.get(att)
+            if meta_value is not None:
 
-        # Auto text frames
+                # Make keywords a list
+                if att == "KEYWORDS":
+                    self.metadata[key] = meta_value.split("; ")
+                    continue
+
+                self.metadata[key] = meta_value
+
+        # Auto text frames ------------------------------------------
 
         for att, human in Document.autoframes_xml.items():
             att_value = xml.get(att)
-
             if att_value is not None:
                 if human == "colums":
                     self.autoframes[human] = int(att_value)
                 if human == "colgap":
                     self.autoframes[human].value = float(att_value)
 
-        # UI snapping
+        # UI snapping -----------------------------------------------
 
         for snap_thing in ["grid", "guides", "element"]:
             att_name = "SnapTo{}".format(snap_thing.capitalize())
 
             att = xml.get(att_name)
             if att is not None:
                 self.ui_snapping[snap_thing] = num_to_bool(att)
 
-        # Bleed settings
+        # Bleed settings --------------------------------------------
 
-        for att,human in Document.bleed_xml.items():
+        for att, human in Document.bleed_xml.items():
             att_value = xml.get(att)
             if att_value is not None:
-                self.bleed[human] = float(att_value)
+                self.bleed[human].value = float(att_value)
 
-        # UI show
+        # Grid settings ---------------------------------------------
 
-        for att_name, ui_name in Document.ui_show_xml.items():
+        for grid_name, grid_setting, att_name in [
+                ["minor", "spacing", "MINGRID"],
+                ["major", "spacing", "MAJGRID"],
+                ["baseline", "offset", "BASEO"],
+                ["baseline", "spacing", "BASEGRID"],
+            ]:
             att = xml.get(att_name)
             if att is not None:
-                self.ui_show[ui_name] = num_to_bool(att)
-
-        # ICC color profiles
+                self.grids[grid_name][grid_setting].value = float(att)
 
-        for case in [
-            ["DPIn", "rgb_images"], ["DPInCMYK", "cmyk_images"],
-            ["DPIn2", "rgb_colors"], ["DPIn3", "cmyk_colors"],
-            ["DPPr", "printer"]]:
-            att_name,icc_key = case
+        # UI show ---------------------------------------------------
 
+        for att_name, ui_name in Document.ui_show_xml.items():
             att = xml.get(att_name)
             if att is not None:
-                self.icc_profiles[icc_key] = att
+                self.ui_show[ui_name] = num_to_bool(att)
 
-        # Calligraphic pen
+        ui_show_stack = xml.get("renderStack")
+        if ui_show_stack is not None:
+            stack = ui_show_stack.split()
 
-        for case in [
-                ["Angle", "angle"], ["LineColorShade", "line_shade"],
-                ["FillColorShade", "fill_shade"]]:
-            att_name = "calligraphicPen{}".format(case[0])
+            if len(stack) == 5:
+                self.ui_show["stack"] = []
 
-            att = xml.get(att_name)
-            if att is not None:
-                self.calligraphicpen[case[1]].value = int(att)
+                for stack_element in stack:
+                    try:
+                        self.ui_show["stack"].append(
+                            Document.ui_stack[stack_element]
+                        )
+                    except KeyError:
+                        continue
 
-        for case in [["LineWidth", "line_width"], ["Width", "width"]]:
-            att_name = "calligraphicPen{}".format(case[0])
+        # UI grid colors --------------------------------------------
 
+        for grid_name, grid_setting, att_name in [
+                ["minor", "color", "MINORC"],
+                ["major", "color", "MAJORC"],
+                ["baseline", "color", "BaseC"],
+            ]:
             att = xml.get(att_name)
             if att is not None:
-                self.calligraphicpen[case[1]].value = float(att)
+                self.grids[grid_name][grid_setting] = att
 
-        for case in [
-                ["LineColor", "line_color"], ["FillColor", "fill_color"],
-                ["PenStyle", "style"]]:
-
-            att_name = "calligraphicPen{}".format(case[0])
+        # ICC color profiles ----------------------------------------
 
+        for att_name, icc_key in Document.icc_xml.items():
             att = xml.get(att_name)
             if att is not None:
-                self.calligraphicpen[case[1]] = att
+                self.icc_profiles[icc_key] = att
 
         # --- DOCUMENT childs --------------------------------------------
 
         for child in xml:
 
-            if child.tag == "CheckProfile":
-                p = Profile()
+            self.__fromxml_item(child, "CheckProfile", Profile, self.profiles)
 
-                success = p.fromxml(child)
-                if success:
-                    self.profiles.append(p)
+            self.__fromxml_item(
+                child, "Gradient", pscolors.Gradient, self.gradients
+            )
+
+            self.__fromxml_item(child, "COLOR", pscolors.Color, self.colors)
+
+            self.__fromxml_item(
+                child, "Pattern", patterns.Pattern, self.patterns
+            )
+
+            self.__fromxml_item(
+                child, "HYPHEN", Hyphenation, self.hyphenation
+            )
+
+            self.__fromxml_item(
+                child, "STYLE", styles.ParagraphStyle, self.styles["paragraph"],
+                True
+            )
+
+            self.__fromxml_item(
+                child, "CHARSTYLE", styles.CharacterStyle,
+                self.styles["character"], True
+            )
+
+            self.__fromxml_item(
+                child, "TableStyle", styles.TableStyle, self.styles["table"],
+                True
+            )
+
+            self.__fromxml_item(
+                child, "CellStyle", styles.CellStyle, self.styles["cell"], True
+            )
+
+            self.__fromxml_item(
+                child, "LAYERS", layers.Layer, self.layers, True
+            )
+
+            self.__fromxml_item(
+                child, "Printer", printing.PrinterSettings,
+                self.printer_settings
+            )
+
+            self.__fromxml_item(
+                child, "PDF", printing.PDFSettings, self.pdf_settings
+            )
 
-            if child.tag == "Gradient":
-                gr = pscolors.Gradient()
+            if child.tag == "DocItemAttributes":
 
-                success = gr.fromxml(child)
-                if success:
-                    self.gradients.append(gr)
+                for attribute in child:
+                    doc_att_item = itemattribute.DocumentAttribute()
 
-            if child.tag == "COLOR":
-                c = pscolors.Color()
+                    success = doc_att_item.fromxml(attribute)
+                    if success:
+                        self.attributes.append(doc_att_item)
 
-                success = c.fromxml(child)
-                if success:
-                    self.colors.append(c)
+            self.__fromxml_section(
+                child,
+                "TablesOfContents",
+                "TableOfContents",
+                toc.TOC,
+                self.tocs,
+            )
+
+            self.__fromxml_section(
+                child,
+                "Marks",
+                "Mark",
+                marks.DocumentMark,
+                self.marks,
+            )
+
+            self.__fromxml_section(
+                child,
+                "NotesStyles",
+                "notesStyle",
+                styles.NoteStyle,
+                self.styles["note"],
+            )
 
-            if child.tag == "Pattern":
-                patt = patterns.Pattern()
+            if child.tag == "NotesFrames":
 
-                success = patt.fromxml(child)
-                if success:
-                    self.patterns.append(patt)
+                for sub in child:
 
-            # TODO FIXME hyphen
+                    if sub.tag == "FOOTNOTEFRAME":
+                        note_frame = notes.NoteFrame()
 
-            if child.tag in ["STYLE", "CHARSTYLE"]:
+                        success = note_frame.fromxml(sub)
+                        if success:
+                            self.notes_frames.append(note_frame)
 
-                if child.tag == "STYLE":
-                    key,xstyle = "paragraph",styles.ParagraphStyle(self)
+            self.__fromxml_section(
+                child,
+                "Notes",
+                "Note",
+                notes.Note,
+                self.notes,
+                True
+            )
 
-                if child.tag == "CHARSTYLE":
-                    key,xstyle = "character",styles.CharacterStyle(self)
+            if child.tag == "PageSets":
 
-                success = xstyle.fromxml(child)
-                if success:
-                    self.styles[key].append(xstyle)
+                for page_set in child:
+                    page_set_item = pages.PageSet()
 
-            if child.tag == "TableStyle":
-                tstyle = styles.TableStyle(self)
+                    success = page_set_item.fromxml(page_set)
+                    if success:
+                        self.page_sets.append(page_set_item)
 
-                success = tstyle.fromxml(child)
-                if success:
-                    self.styles["table"].append(tstyle)
+            self.__fromxml_section(
+                child,
+                "Sections",
+                "Section",
+                toc.Section,
+                self.sections,
+            )
+
+            self.__fromxml_item(
+                child, "MASTERPAGE", pages.MasterPage, self.master_pages, False
+            )
+
+            if child.tag == "PAGE":
+                page_item = pages.Page()
 
-            if child.tag == "CellStyle":
-                cstyle = styles.CellStyle(self)
+                page_item.sla_parent = self.sla_parent
+                page_item.doc_parent = self
 
-                success = cstyle.fromxml(child)
+                success = page_item.fromxml(child)
                 if success:
-                    self.styles["cell"].append(cstyle)
+                    self.pages.append(page_item)
 
-            if child.tag == "LAYERS":
-                l = Layer()
+            if child.tag == "PAGEOBJECT":
+                ptype = child.get("PTYPE")
 
-                success = l.fromxml(child)
-                if success:
-                    self.layers.append(l)
+                if ptype is None:
+                    continue
 
-            if child.tag == "Printer":
+                try:
+                    p_object = pageobjects.new_from_type(
+                        ptype, self.sla_parent, self
+                    )
 
-                ps = printing.PrinterSettings()
+                    success = p_object.fromxml(child)
+                    if success:
+                        self.page_objects.append(p_object)
 
-                success = ps.fromxml(child)
-                if success:
-                    self.printer_settings.append(ps)
+                except ValueError:
+                    pass
 
-            if child.tag == "PDF":
+        # ----------------------------------------------------------------
 
-                pds = printing.PDFSettings()
+        return True
 
-                success = pds.fromxml(child)
-                if success:
-                    self.pdf_settings.append(pds)
+    def toxml(self, optional: bool = True) -> ET.Element:
+        xml = ET.Element("DOCUMENT")
 
-            if child.tag == "DocItemAttributes":
+        # === DOCUMENT attributes : new order (WIP) ======================
 
-                for attribute in child:
-                    da = itemattribute.DocumentAttribute()
+        # DONE: 001 — ANZPAGES
+        # DONE: 002 — PAGEWIDTH
+        # DONE: 003 — PAGEHEIGHT
+        xml.attrib["ANZPAGES"] = str(self.page_number)
+        xml.attrib["PAGEWIDTH"] = self.dims["width"].toxmlstr()
+        xml.attrib["PAGEHEIGHT"] = self.dims["height"].toxmlstr()
 
-                    success = da.fromxml(attribute)
-                    if success:
-                        self.attributes.append(da)
+        # Borders --------------------------------------------------------
+        # DONE: 004 — BORDERLEFT
+        # DONE: 005 — BORDERRIGHT
+        # DONE: 006 — BORDERTOP
+        # DONE: 007 — BORDERBOTTOM
+
+        for border_side, border_value in self.borders.items():
+            att = "BORDER{}".format(border_side.upper())
+            xml.attrib[att] = border_value.toxmlstr()
+
+        # 008 — PRESET
+
+        # Bleed settings -------------------------------------------------
+
+        # DONE: 009 — BleedTop
+        # DONE: 010 — BleedLeft
+        # DONE: 011 — BleedRight
+        # DONE: 012 — BleedBottom
 
-            if child.tag == "TablesOfContents":
+        for att, human in Document.bleed_xml.items():
+            xml.attrib[att] = self.bleed[human].toxmlstr(True)
 
-                for sub in child:
+        # ----------------------------------------------------------------
 
-                    if sub.tag == "TableOfContents":
-                        toc_settings = toc.TOC()
+        # DONE: 013 — ORIENTATION
 
-                        success = toc_settings.fromxml(sub)
-                        if success:
-                            self.tocs.append(toc_settings)
+        xml.attrib["ORIENTATION"] = str(int(self.doc_pages["orientation"]))
 
-            if child.tag == "Marks":
+        # DONE: 014 — PAGESIZE
 
-                for sub in child:
+        for att, human in pages.xml_size.items():
+            if human == self.doc_pages["size"]:
+                xml.attrib["PAGESIZE"] = att
+                break
 
-                    if sub.tag == "Mark":
-                        mx = marks.DocumentMark()
+        # 015 — FIRSTNUM
 
-                        success = mx.fromxml(sub)
-                        if success:
-                            self.marks.append(mx)
+        # DONE: 016 — BOOK
+        xml.attrib["BOOK"] = str(self.doc_pages["set"])
 
-            if child.tag == "NotesStyles":
+        # Auto text frames -----------------------------------------------
 
-                for sub in child:
+        # DONE: 017 — AUTOSPALTEN
+        # DONE: 018 — ABSTSPALTEN
 
-                    if sub.tag == "notesStyle":
-                        s = styles.NoteStyle()
+        for att, human in Document.autoframes_xml.items():
 
-                        success = s.fromxml(sub)
-                        if success:
-                            self.styles["note"].append(s)
+            if human == "columns":
+                xml.attrib[att] = str(self.autoframes[human])
 
-            if child.tag == "NotesFrames":
+            if human == "colgap":
+                xml.attrib[att] = self.autoframes[human].toxmlstr(True)
 
-                for sub in child:
+        # Document units -------------------------------------------------
+        # DONE: 019 — UNITS
 
-                    if sub.tag == "FOOTNOTEFRAME":
-                        nf = notes.NoteFrame()
+        # Optional if the units are points
+        if self.units != "points":
+            for code, human in Document.units_xml.items():
+                if self.units == human:
+                    xml.attrib["UNITS"] = code
+                    break
 
-                        success = nf.fromxml(sub)
-                        if success:
-                            self.notes_frames.append(nf)
+        # Default settings -----------------------------------------------
+        # DONE: 020 — DFONT
+        # DONE: 021 — DSIZE
+        # DONE: 022 — DCOL
+        # DONE: 023 — DGAP
 
-            if child.tag == "Notes":
+        if self.tools["text"]["font"] is not None:
+            xml.attrib["DFONT"] = self.tools["text"]["font"]
 
-                for sub in child:
+        xml.attrib["DSIZE"] = self.tools["text"]["size"].toxmlstr(True)
 
-                    if child.tag == "Note":
-                        nc = notes.Note()
+        # NOTE Marked as optional but is not
+        xml.attrib["DCOL"] = str(self.tools["text"]["columns"])
 
-                        success = nc.fromxml(sub)
-                        if success:
-                            self.notes.append(nc)
+        xml.attrib["DGAP"] = self.tools["text"]["columns_gap"].toxmlstr()
 
-            if child.tag == "PageSets":
+        # ----------------------------------------------------------------
 
-                for page_set in child:
-                    ps = pages.PageSet()
+        # 024 — TabFill
 
-                    success = ps.fromxml(page_set)
-                    if success:
-                        self.page_sets.append(ps)
+        # 025 — TabWidth
 
-            if child.tag == "Sections":
+        # 026 — TextDistLeft
 
-                for sub in child:
+        # 027 — TextDistRight
 
-                    if sub.tag == "Section":
-                        sec = toc.Section()
+        # 028 — TextDistBottom
+
+        # 029 — TextDistTop
+
+        # 030 — FirstLineOffset
+
+        # Metadatas ------------------------------------------------------
+        # DONE: 031 — AUTHOR
+        # DONE: 032 — COMMENTS
+        # DONE: 033 — KEYWORDS
+        # DONE: 034 — PUBLISHER
+        # DONE: 035 — DOCDATE
+        # DONE: 036 — DOCTYPE
+        # DONE: 037 — DOCFORMAT
+        # DONE: 038 — DOCIDENT
+        # DONE: 039 — DOCSOURCE
+        # DONE: 040 — DOCLANGINFO
+        # DONE: 041 — DOCRELATION
+        # DONE: 042 — DOCCOVER
+        # DONE: 043 — DOCRIGHTS
+        # DONE: 044 — DOCCONTRIB
+        # DONE: 045 — TITLE
+        # DONE: 046 — SUBJECT
+
+        for att, human in Document.metadata_xml.items():
+            if human == "keywords":
+                xml.attrib[att] = "; ".join(self.metadata[human])
+                continue
 
-                        success = sec.fromxml(sub)
-                        if success:
-                            self.sections.append(sec)
+            xml.attrib[att] = self.metadata[human]
 
-            if child.tag == "MASTERPAGE":
-                m = pages.MasterPage()
+        # ----------------------------------------------------------------
 
-                success = m.fromxml(child)
-                if success:
-                    self.master_pages.append(m)
+        # 047 — VHOCH
 
-            if child.tag == "PAGE":
-                p = pages.Page()
+        # 048 — VHOCHSC
 
-                p.sla_parent = self.sla_parent
-                p.doc_parent = self
+        # 049 — VTIEF
 
-                success = p.fromxml(child)
-                if success:
-                    self.pages.append(p)
+        # 050 — VTIEFSC
 
-            if child.tag == "PAGEOBJECT":
-                ptype = child.get("PTYPE")
+        # 051 — VKAPIT
 
-                if ptype is not None:
+        # UI grids (baseline grid) ---------------------------------------
+        # DONE: 052 — BASEGRID
+        # DONE: 053 — BASEO
+        xml.attrib["BASEGRID"] = self.grids["baseline"]["spacing"].toxmlstr(True)
+        xml.attrib["BASEO"] = self.grids["baseline"]["offset"].toxmlstr(True)
 
-                    try:
-                        po = pageobjects.new_from_type(
-                            ptype, self.sla_parent, self
-                        )
+        # ----------------------------------------------------------------
 
-                        success = po.fromxml(child)
-                        if success:
-                            self.page_objects.append(po)
+        # 054 — AUTOL
+
+        # 055 — UnderlinePos
+
+        # 056 — UnderlineWidth
+
+        # 057 — StrikeThruPos
+
+        # 058 — StrikeThruWidth
+
+        # 059 — GROUPC
 
-                    except ValueError:
-                        pass
+        # 060 — HCMS
+
+        # 061 — DPSo
+
+        # 062 — DPSFo
+
+        # 063 — DPuse
+
+        # 064 — DPgam
+
+        # 065 — DPbla
+
+        # ICC profiles ---------------------------------------------------
+        # DONE: 066 — DPPr
+        # DONE: 067 — DPIn
+        # DONE: 068 — DPInCMYK
+        # DONE: 069 — DPIn2
+        # DONE: 070 — DPIn3
+
+        for att, human in Document.icc_xml.items():
+            xml.attrib[att] = self.icc_profiles[human]
 
         # ----------------------------------------------------------------
 
-        return True
+        # 071 — DISc
 
-    def toxml(self, optional=True):
-        xml = ET.Element("DOCUMENT")
+        # 072 — DIIm
 
-        # --- DOCUMENT attributes ----------------------------------------
+        # 073 — ALAYER
 
-        # TODO DOCUMENT many attribs…
+        # 074 — LANGUAGE
 
-        # Pages settings
+        # 075 — AUTOMATIC
 
-        xml.attrib["ORIENTATION"] = str(int(self.doc_pages["orientation"]))
+        # 076 — AUTOCHECK
 
-        for att, human in pages.xml_size.items():
-            if human == self.doc_pages["size"]:
-                xml.attrib["PAGESIZE"] = att
+        # 077 — GUIDELOCK
+
+        # UI snapping ----------------------------------------------------
+        # DONE: 078 — SnapToGuides
+        # DONE: 079 — SnapToGrid
+        # DONE: 080 — SnapToElement
+
+        for att_base, snap_value in self.ui_snapping.items():
+            att = "SnapTo{}".format(att_base.capitalize())
+            xml.attrib[att] = bool_to_num(snap_value)
+
+        # UI grids -------------------------------------------------------
+        # DONE: 081 — MINGRID (minor grid)
+        # DONE: 082 — MAJGRID (major grid)
+        xml.attrib["MINGRID"] = self.grids["minor"]["spacing"].toxmlstr()
+        xml.attrib["MAJGRID"] = self.grids["major"]["spacing"].toxmlstr()
+
+        # UI show --------------------------------------------------------
+        # DONE: 083 — SHOWGRID
+        # DONE: 084 — SHOWGUIDES
+        # DONE: 085 — showcolborders
+        # DONE: 086 — SHOWFRAME
+        # DONE: 087 — SHOWControl
+        # DONE: 088 — SHOWLAYERM
+        # DONE: 089 — SHOWMARGIN
+        # DONE: 090 — SHOWBASE
+        # DONE: 091 — SHOWPICT
+        # DONE: 092 — SHOWLINK
+
+        for att, human in Document.ui_show_xml.items():
+            if att == "showrulers":
                 break
 
-        xml.attrib["BOOK"] = str(self.doc_pages["set"])
+            xml.attrib[att] = bool_to_num(self.ui_show[human])
 
-        # Auto text frames
+        # ----------------------------------------------------------------
 
-        for att, human in Document.autoframes_xml.items():
+        # 093 — rulerMode
 
-            if human == "columns":
-                xml.attrib[att] = str(self.autoframes[human])
+        # DONE: 094 — showrulers
+        # DONE: 095 — showBleed
 
-            if human == "colgap":
-                xml.attrib[att] = self.autoframes[human].toxmlstr(True)
+        for att in ["showrulers", "showBleed"]:
+            for att_name, ui_name in Document.ui_show_xml.items():
+                if att_name != att:
+                    continue
 
-        # Bleed settings
+                xml.attrib[att_name] = bool_to_num(self.ui_show[ui_name])
 
-        for att,human in Document.bleed_xml.items():
-            xml.attrib[att] = str(self.bleed[human])
+        # 096 — rulerXoffset
 
-        xml.attrib["ANZPAGES"] = str(self.page_number)
+        # 097 — rulerYoffset
 
-        # Dimensions
+        # 098 — GuideRad
 
-        xml.attrib["PAGEWIDTH"] = self.dims["width"].toxmlstr()
-        xml.attrib["PAGEHEIGHT"] = self.dims["height"].toxmlstr()
+        # 099 — GRAB
 
-        # Borders
+        # Polygon tool -------------------------------------------
 
-        for b in self.borders.keys():
-            att = "BORDER{}".format(b.upper())
-            xml.attrib[att] = self.borders[b].toxmlstr()
+        # DONE: DONE: 100 — POLYC
+        # DONE: 101 — POLYF — FIXME : Unknown float numeric type with Dim unit
+        # DONE: 102 — POLYR
+        # DONE: 103 — POLYIR
+        # DONE: 104 — POLYCUR
+        # DONE: 105 — POLYOCUR
+        # DONE: 106 — POLYS
 
-        # Metadatas
+        xml.attrib["POLYC"] = str(self.tools["polygon"]["sides"])
 
-        for att, key in Document.metadata_xml.items():
-            xml.attrib[att] = self.metadata[key]
+        convconc_intensity = self.tools["polygon"]["convconc"]["intensity"]
 
-        xml.attrib["KEYWORDS"] = "; ".join(self.metadata["keywords"])
+        if float(convconc_intensity) == float(int(convconc_intensity)):
+            xml.attrib["POLYF"] = str(int(convconc_intensity))
 
-        # UI snapping
+        xml.attrib["POLYF"] = str(convconc_intensity)
 
-        for k,v in self.ui_snapping.items():
-            att = "SnapTo{}".format(k.capitalize())
+        xml.attrib["POLYR"] = self.tools["polygon"]["rotation"].toxmlstr()
 
-            xml.attrib[att] = bool_to_num(v)
+        for att, hmn in [
+                ["POLYR", "rot_in"], ["POLYCUR", "curb_in"],
+                ["POLYOCUR", "curb_out"]]:
+            xml.attrib[att] = self.tools["polygon"]["convconc"][hmn].toxmlstr()
 
-        # UI show
+        xml.attrib["POLYS"] = bool_to_num(
+            self.tools["polygon"]["convconc"]["active"]
+        )
 
-        for att_name, ui_name in Document.ui_show_xml.items():
-            xml.attrib[att_name] = bool_to_num(self.ui_show[ui_name])
+        # --------------------------------------------------------
 
-        # ICC profiles
+        # 107 — arcStartAngle
 
-        xml.attrib["DPIn"] = self.icc_profiles["rgb_images"]
-        xml.attrib["DPInCMYK"] = self.icc_profiles["cmyk_images"]
-        xml.attrib["DPIn2"] = self.icc_profiles["rgb_colors"]
-        xml.attrib["DPIn3"] = self.icc_profiles["cmyk_colors"]
-        xml.attrib["DPPr"] = self.icc_profiles["printer"]
-
-        # Calligraphic pen
-        # -------------------------------------------------
-
-        for case in [
-                ["Angle", "angle", True],
-                ["LineWidth", "line_width", True],
-                ["LineColorShade", "line_shade", True],
-                ["LineColor", "line_color", False],
-                ["Width", "width", True],
-                ["Style", "style", False],
-                ["FillColor", "fill_color", False],
-                ["FillColorShade", "fill_shade", True]]:
+        # 108 — arcSweepAngle
 
-            att_name = "calligraphicPen{}".format(case[0])
-            att_value = self.calligraphicpen[case[1]]
+        # 109 — spiralStartAngle
 
-            if case[2]:
-                att_value = att_value.toxmlstr()
+        # 110 — spiralEndAngle
 
-            if case[0] == "Style":
-                att_value = str(att_value)
+        # 111 — spiralFactor
 
-            xml.attrib[att_name] = att_value
+        # 112 — AutoSave
 
-        # --- DOCUMENT childs --------------------------------------------
+        # 113 — AutoSaveTime
 
-        # Checking profiles -------------------------------
+        # 114 — AutoSaveCount
 
-        for profile in self.profiles:
-            px = profile.toxml()
+        # 115 — AutoSaveKeep
 
-            if not isinstance(px, bool):
-                xml.append(px)
+        # 116 — AUtoSaveInDocDir
 
-        # Colors ------------------------------------------
+        # 117 — AutoSaveDir
 
-        for color in self.colors:
-            cx = color.toxml()
-            xml.append(cx)
+        # Scratch space ------------------------------------------
+        # DONE: 118 — ScratchBottom
+        # DONE: 119 — ScratchLeft
+        # DONE: 120 — ScratchRight
+        # DONE: 121 — ScratchTop
+        # DONE: 122 — GapHorizontal
+        # DONE: 123 — GapVertical
 
-        # TODO hyphen
+        for att, human in Document.scratchspace_xml.items():
+            xml.attrib[att] = self.scratchspace[human].toxmlstr(True)
 
-        # Styles ------------------------------------------
+        # --------------------------------------------------------
 
-        for pstyle in self.styles["paragraph"]:
-            pstylex = pstyle.toxml()
-            xml.append(pstylex)
+        # Line tool ----------------------------------------------
+        # 0 is no arrow, arrow styles goes from 1 to 36 (incl)
+        #
+        # DONE: 124 — StartArrow
+        # DONE: 125 — EndArrow
 
-        for cstyle in self.styles["character"]:
-            cstylex = cstyle.toxml()
-            xml.append(cstylex)
+        for att, human in [["StartArrow", "start"], ["EndArrow", "end"]]:
+            xml.attrib[att] = str(self.tools["line"]["arrows"][human])
 
-        for tstyle in self.styles["table"]:
-            tstylex = tstyle.toxml()
-            xml.append(tstylex)
+        # ------------------------------------------------------
 
-        for cstyle in self.styles["cell"]:
-            cstylex = cstyle.toxml()
-            xml.append(cstylex)
+        # DONE: 126 — PEN (Shape tool, pen)
+        xml.attrib["PEN"] = str(self.tools["shape"]["pen"]["color"])
 
-        # Layers ------------------------------------------
+        # DONE: 127 — BRUSH (Shape tool, brush)
+        xml.attrib["BRUSH"] = str(self.tools["shape"]["brush"]["color"])
 
-        for layer in self.layers:
-            layerx = layer.toxml()
-            xml.append(layerx)
+        # 128 — PENLINE (Line tool)
+        xml.attrib["PENLINE"] = str(self.tools["line"]["color"])
 
-        # Printer settings --------------------------------
+        # 129 — PENTEXT
 
-        for ps in self.printer_settings:
-            px = ps.toxml()
-            xml.append(px)
+        # 130 — StrokeText
 
-        # PDF settings ------------------------------------
+        # 131 — TextBackGround
+        # 132 — TextLineColor
+        # 133 — TextBackGroundShade
+        # 134 — TextLineShade
+        # 135 — TextPenShade
+        # 136 — TextStrokeShade
 
-        for pds in self.pdf_settings:
-            px = pds.toxml()
-            xml.append(px)
+        # DONE: 137 — STIL (Shape tool)
+        xml.attrib["STIL"] = str(self.tools["shape"]["style"])
 
-        # Document attributes -----------------------------
+        # DONE: 138 — STILLINE (Line tool)
+        xml.attrib["STILLINE"] = str(self.tools["line"]["style"])
 
-        doca = ET.Element("DocItemAttributes")
+        # DONE: 139 — WIDTH (Shape tool)
+        xml.attrib["WIDTH"] = self.tools["shape"]["width"].toxmlstr(True)
 
-        for attribute in self.attributes:
-            ax = attribute.toxml()
-            doca.append(ax)
+        # DONE: 140 — WIDTHLINE (Line tool)
+        xml.attrib["WIDTHLINE"] = self.tools["line"]["width"].toxmlstr(True)
 
-        xml.append(doca)
+        # DONE: 141 — PENSHADE (Shape tool, pen)
+        xml.attrib["PENSHADE"] = self.tools["shape"]["pen"]["shade"].toxmlstr()
 
-        # Tables of contents ------------------------------
+        # DONE: 142 — LINESHADE (Line tool)
+        xml.attrib["LINESHADE"] = self.tools["line"]["shade"].toxmlstr()
 
-        tocx = ET.Element("TablesOfContents")
+        # DONE: 143 — BRUSHSHADE (Shape tool, brush)
+        xml.attrib["BRUSHSHADE"] = self.tools["shape"]["brush"]["shade"].toxmlstr()
 
-        for toc in self.tocs:
-            tx = toc.toxml()
-            tocx.append(tx)
+        # ------------------------------------------------------
 
-        xml.append(tocx)
+        # TODO: From 144 to 156, most probably Image tool settings
 
-        # Marks -------------------------------------------
+        # 144 — CPICT
+        # 145 — PICTSHADE
 
-        if self.marks:
+        # 146 — CSPICT
+        # 147 — PICTSSHADE
 
-            marksx = ET.Element("Marks")
+        # 148 — PICTSCX
+        # 149 — PICTSCY
 
-            for m in self.marks:
-                mx = m.toxml()
-                marksx.append(mx)
+        # 150 — PSCALE
 
-            xml.append(marksx)
+        # 151 — PASPECT
 
-        # Notes : styles, frames, notes content -----------
+        # 152 — EmbeddedPath
 
-        # Notes styles -------------------------------
+        # 153 — HalfRes
 
-        nsx = ET.Element("NotesStyles")
+        # 154 — dispX
+        # 155 — dispY
 
-        for note_style in self.styles["note"]:
-            nx = note_style.toxml()
-            nsx.append(nx)
+        # 156 — constrain
 
-        xml.append(nsx)
+        # ------------------------------------------------------
 
-        # Notes frames -------------------------------
+        # DONE: 157 — MINORC
+        # DONE: 158 — MAJORC
+        xml.attrib["MINORC"] = self.grids["minor"]["color"]
+        xml.attrib["MAJORC"] = self.grids["major"]["color"]
 
-        if self.notes_frames:
+        # 159 — GuideC
 
-            nfx = ET.Element("NotesFrames")
+        # DONE: 160 — BaseC
+        xml.attrib["BaseC"] = self.grids["baseline"]["color"]
 
-            for note_frame in self.notes_frames:
-                n = note_frame.toxml()
-                nfx.append(n)
+        # DONE: 161 — renderStack
 
-            xml.append(nfx)
+        if self.ui_show["stack"]:
+            stack = []
 
-        # Notes content ------------------------------
+            for stack_element in self.ui_show["stack"]:
+                for code, human in Document.ui_stack.items():
+                    if human != stack_element:
+                        continue
+                    stack.append(code)
+                    break
 
-        if self.notes:
+            if stack:
+                stack = " ".join(stack)
+            else:
+                stack = "2 0 4 1 3"
+        else:
+            stack = "2 0 4 1 3"
 
-            nx = ET.Element("Notes")
+        xml.attrib["renderStack"] = stack
 
-            for note in self.notes:
-                # n = note.toxml()
-                # nx.append(n)
-                pass
+        # 162 — GridType
 
-            xml.append(nx)
+        # 163 — PAGEC
 
-        # Page sets ---------------------------------------
+        # 164 — MARGC
+
+        # 165 — RANDF
+
+        # 166 — currentProfile
+
+        # Calligraphic pen -----------------------------------------------
+        # DONE: 167 — calligraphicPenFillColor
+        # DONE: 168 — calligraphicPenLineColor
+        # DONE: 169 — calligraphicPenFillColorShade
+        # DONE: 170 — calligraphicPenLineColorShade
+        # DONE: 171 — calligraphicPenLineWidth
+        # DONE: 172 — calligraphicPenAngle
+        # DONE: 173 — calligraphicPenWidth
+        # DONE: 174 — calligraphicPenStyle
+
+        for key_out_suffix, key_in, as_string in [
+            ["FillColor", "fill_color", False],
+            ["LineColor", "line_color", False],
+            ["FillColorShade", "fill_shade", True],
+            ["LineColorShade", "line_shade", True],
+            ["LineWidth", "line_width", True],
+            ["Angle", "angle", True],
+            ["Width", "width", True],
+            ["Style", "style", False],
+        ]:
+            att_name = f"calligraphicPen{key_out_suffix}"
+            att_value = self.tools["calligraphicpen"][key_in]
 
-        pssx = ET.Element("PageSets")
+            if as_string:
+                att_value = att_value.toxmlstr()
 
-        for page_set in self.page_sets:
-            px = page_set.toxml()
-            pssx.append(px)
+            if key_out_suffix == "Style":
+                att_value = str(att_value)
 
-        xml.append(pssx)
+            xml.attrib[att_name] = att_value
 
-        # Sections ----------------------------------------
+        # === DOCUMENT childs ============================================
 
-        secx = ET.Element("Sections")
+        # Checking profiles ----------------------------------------------
 
-        for section in self.sections:
-            sx = section.toxml()
-            secx.append(sx)
+        for profile in self.profiles:
+            profile_xml = profile.toxml()
+
+            if not isinstance(profile_xml, bool):
+                xml.append(profile_xml)
 
-        xml.append(secx)
+        # Colors ---------------------------------------------------------
 
-        # Master pages ------------------------------------
+        xml = self.__toxml_items(xml, self.colors)
 
-        for master in self.master_pages:
-            mx = master.toxml()
-            xml.append(mx)
+        # Hyphenation settings -------------------------------------------
+
+        if self.hyphenation is None:
+            hyphen = Hyphenation(default=True)
+            hyphen_xml = hyphen.toxml()
+        else:
+            hyphen_xml = self.hyphenation.toxml()
 
-        # Pages -------------------------------------------
+        xml.append(hyphen_xml)
 
-        for page in self.pages:
-            p = page.toxml()
-            xml.append(p)
+        # Styles ---------------------------------------------------------
 
-        # Pages objects -----------------------------------
+        for style_type in ["character", "paragraph", "table", "cell"]:
 
-        for po in self.page_objects:
-            px = po.toxml()
-            xml.append(px)
+            for style_item in self.styles[style_type]:
+                item_xml = style_item.toxml()
+                xml.append(item_xml)
 
         # ----------------------------------------------------------------
 
-        return xml
+        # Layers
+        xml = self.__toxml_items(xml, self.layers)
 
-    #========================================================================
+        # Printer settings
+        xml = self.__toxml_items(xml, self.printer_settings)
 
-    def pageobjects(self, object_type=False, templatable=False):
-        pos_ret = []
+        # PDF settings
+        xml = self.__toxml_items(xml, self.pdf_settings)
 
-        # If there is a object type filter, we filter before checking
-        # if we must return only templatable objects
+        # Document attributes
+        xml = self.__toxml_section(xml, "DocItemAttributes", self.attributes)
 
-        if object_type:
+        # Tables of contents
+        xml = self.__toxml_section(xml, "TablesOfContents", self.tocs)
 
-            if object_type in pageobjects.po_type_classes:
-                pos = []
+        # Marks
+        if self.marks:
+            xml = self.__toxml_section(xml, "Marks", self.marks)
 
-                for po in self.page_objects:
-                    if isinstance(po, pageobjects.po_type_classes[object_type]):
-                        pos.append(po)
+        # Notes : styles, frames, content --------------------------------
 
-        if templatable:
+        # Notes styles
+        xml = self.__toxml_section(xml, "NotesStyles", self.styles["note"])
 
-            if self.sla_parent.templating["active"]:
-                lookup_set = []
-                templatable_set = []
+        # Notes frames
+        if self.notes_frames:
+            xml = self.__toxml_section(xml, "NotesFrames", self.notes_frames)
 
-                if object_type:
-                    lookup_set = pos
-                else:
-                    lookup_set = self.page_objects
+        # Notes content
 
-                for po in lookup_set:
-                    # If the page object is a text frame with templatable
-                    # stories, we add these templatable stories
+        if self.notes:
+            nx = ET.Element("Notes")
 
-                    if isinstance(po, pageobjects.TextObject):
-                        po_templatable_stories = po.templatable()
+            for note in self.notes:
+                # n = note.toxml()
+                # nx.append(n)
+                pass
+
+            xml.append(nx)
+
+        # ----------------------------------------------------------------
+
+        # Page sets
+        xml = self.__toxml_section(xml, "PageSets", self.page_sets)
+        # Sections
+        xml = self.__toxml_section(xml, "Sections", self.sections)
 
-                        if po_templatable_stories:
-                            templatable_set.extend(po_templatable_stories)
+        # Pages (master, regular) ----------------------------------------
 
-                    else:
-                        # TODO If this page object is another type of page
-                        # object, we look its properties and find if it
-                        # is templatable through sla.SLA.templating settings
+        # Master pages
+        xml = self.__toxml_items(xml, self.master_pages)
+        # Pages
+        xml = self.__toxml_items(xml, self.pages)
 
-                        if po.templatable():
-                            templatable_set.append(po)
+        # Pages objects --------------------------------------------------
 
-                pos_ret = templatable_set
+        xml = self.__toxml_items(xml, self.page_objects)
 
+        # ----------------------------------------------------------------
+
+        return xml
+
+    def __fromxml_item(
+        self,
+        xml: ET.Element,
+        item_tag: str,
+        object_class,
+        attribute,
+        parent: bool = False
+    ):
+        if xml.tag != item_tag:
+            return
+
+        if parent:
+            item_object = object_class(self)
         else:
-            if object_type:
-                pos_ret = pos
+            item_object = object_class()
+
+        success = item_object.fromxml(xml)
+        if success:
+            if isinstance(attribute, list):
+                attribute.append(item_object)
             else:
-                pos_ret = self.page_objects
+                attribute = item_object
 
-        return pos_ret
+    def __fromxml_section(
+        self,
+        xml,
+        section_tag: str,
+        item_tag: str,
+        object_class,
+        attribute,
+        parent: bool = False
+    ):
+        if xml.tag != section_tag:
+            return
 
-    def stories(self):
+        for element in xml:
+
+            if element.tag != item_tag:
+                continue
+
+            if parent:
+                item_object = object_class(self)
+            else:
+                item_object = object_class()
+
+            success = item_object.fromxml(element)
+            if success:
+                attribute.append(item_object)
+
+    def __toxml_items(self, xml: ET.Element, items: list) -> ET.Element:
         """
-        Returns all stories in the document.
+        Add children nodes from `toxml()` methods of items to node `xml`.
 
-        :rtype: list
-        :returns: List of stories
+        :type xml: ET.Element
+        :type items: list
+        :rtype: ET.Element
         """
 
-        stories = []
+        for item in items:
+            item_xml = item.toxml()
+            xml.append(item_xml)
+
+        return xml
+
+    def __toxml_section(
+        self,
+        xml: ET.Element,
+        section_tag: str,
+        section_items: list
+    ) -> ET.Element:
+        """
+        Add a node with tag `section_tag` containing the XML representation
+        of `sections_items` (accessed through `toxml()` methods) as children,
+        to node `xml`.
+
+        :type xml: ET.Element
+        :type section_tag: str
+        :type section_items: list
+        :rtype: ET.Element
+        """
+
+        section = ET.Element(section_tag)
+
+        for item in section_items:
+            item_xml = item.toxml()
+            section.append(item_xml)
+
+        xml.append(section)
+
+        return xml
+
+    # =======================================================================
 
-        #--- Text frames stories -----------------------------------------
+    def style(
+        self,
+        name: Optional[str] = None,
+        style_type: Optional[str] = None,
+        default: bool = False,
+    ) -> Union[List[styles.StyleAbstract], styles.StyleAbstract]:
 
-        filtered = [
-            po for po in self.page_objects if po.have_stories and po.stories
-        ]
+        result = []
+        style_types = list(self.styles.keys())
 
-        if filtered:
+        if style_type is not None:
+            if style_type in style_types:
+                style_types = [style_type]
 
-            for po in filtered:
-                stories.extend(po.stories)
+        for type_key in style_types:
 
-        #--- Table cells stories -----------------------------------------
+            for style in self.styles[type_key]:
 
-        tables = [
-            po for po in self.page_objects if po.ptype == "table"
-        ]
+                if name is None and style_type is not None:
 
-        if tables:
-            cells = []
+                    # Returns only default style of type X
+                    if default and style.is_default:
+                        return style
 
-            for po in tables:
-                cells.extend(po.cells)
+                    # Returns all types of type X
+                    result.append(style)
+                    continue
 
-            for cell in cells:
-                if cell.story is not None:
-                    stories.append(cell.story)
+                # Request for default style not satisfactory
+                if default and not style.is_default:
+                    continue
 
-        #-----------------------------------------------------------------
+                # Request for style name not satisfactory
+                if name != style.name:
+                    continue
 
-        return stories
+                result.append(style)
 
-    #========================================================================
+        return result
 
-    def page_number(self):
+    # =======================================================================
+
+    # TODO Maybe delete page_number ?
+
+    def page_number(self) -> int:
         """
         Get document pages number.
         """
 
         pn = 0
 
-        for p in self.pages:
+        for po in self.pages:
             if po.number > pn:
                 pn = po.number
 
         return pn
 
-    def append(self, sla_object, **kwargs):
+    def append(self, sla_object: AppendableToDocument, **kwargs) -> bool:
         """
         Append a page, a page object, layer, style…
 
         +----------------+---------+-----------------------------------------+
         | Argument name  | Type    | Usage                                   |
         +================+=========+=========================================+
         | check_color    | boolean | If True, check if a document's color    |
@@ -1427,15 +2061,16 @@
                 if "overlap_layer" in kwargs:
                     same_layer = kwargs["overlap_layer"]
                 else:
                     same_layer = True
 
                 if same_layer:
                     page_objets = [
-                        po for po in self.page_objets
+                        po
+                        for po in self.page_objects
                         if po.layer == sla_object.layer
                     ]
                 else:
                     page_objets = self.page_objects
 
                 for po in page_objets:
                     # TODO FIXME Test coordinates
@@ -1449,16 +2084,16 @@
             if add:
                 sla_object.doc_parent = self
                 sla_object.sla_parent = self.sla_parent
 
                 self.page_objects.append(sla_object)
 
                 return True
-            else:
-                return False
+
+            return False
 
         if isinstance(sla_object, pages.PageAbstract):
             # NOTE If sla_object is a page or a master page, its number
             # attribute is only relevant if there is a page number gap.
 
             # TODO Obtenir les numéros de page actuellement utilisés,
             # puis vérifier s’il y a des pages manquantes.
@@ -1502,15 +2137,15 @@
                 self.pages.append(sla_object)
                 return True
 
             if isinstance(sla_object, pages.MasterPage):
                 self.master_pages.append(sla_object)
                 return True
 
-        if isinstance(sla_object, Layer):
+        if isinstance(sla_object, layers.Layer):
 
             for layer in self.layers:
 
                 # If a layer have the same level
 
                 if layer.level == sla_object.level:
                     raise exceptions.ConflictingLayer(
@@ -1580,31 +2215,37 @@
                 if isinstance(sla_object, styles.CharacterStyle):
                     self.styles["character"].append(sla_object)
                     return True
 
                 # TODO NOTE Then we should call a "hook" to all styles that
                 # may have parents styles to update them as well.
                 # Something like :
+                #
                 # for paragraph_style in self.styles["paragraph"]:
-                    # if isinstance(sla_object, styles.CharacterStyle):
-                        # paragraph_style.event("charstyle-added-document")
-                    # if isinstance(sla_object, styles.ParagraphStyle):
-                        # paragraph_style.event("parastyle-added-document")
+                #     if isinstance(sla_object, styles.CharacterStyle):
+                #         paragraph_style.event("charstyle-added-document")
+                #     if isinstance(sla_object, styles.ParagraphStyle):
+                #         paragraph_style.event("parastyle-added-document")
 
         return False
 
-    #========================================================================
+    # =======================================================================
 
 
 class Profile(PyScribusElement):
-    """
-    """
+    """"""
 
     defaults = [
-        "PDF 1.3", "PDF 1.4", "PDF 1.5", "PDF/X-3", "PDF/X-4", "PostScript", "PDF/X-1a"
+        "PDF 1.3",
+        "PDF 1.4",
+        "PDF 1.5",
+        "PDF/X-3",
+        "PDF/X-4",
+        "PostScript",
+        "PDF/X-1a",
     ]
 
     def __init__(self, default=False):
         super().__init__()
 
         self.pyscribus_defaults = [k for k in Profile.defaults]
 
@@ -1623,71 +2264,93 @@
             "RasterPDF": False,
             "ForGIF": False,
             "NotCMYKOrSpot": False,
             "DeviceColorsAndOutputIntent": False,
             "FontNotEmbedded": False,
             "FontIsOpenType": False,
             "AppliedMasterDifferentSide": False,
-            "EmptyTextFrames": False
+            "EmptyTextFrames": False,
         }
 
         self.ignores = {"Errors": False, "OffLayers": False}
 
         self.resolution = {
             "min": dimensions.Dim(0, unit="dpi", integer=True),
             "max": dimensions.Dim(0, unit="dpi", integer=True),
         }
 
         if default:
             self.fromdefault(default)
 
-    def set_checks(self, checks, value=True):
+    def set_checks(self, checks: list, value=True) -> NoReturn:
         """
         :param checks: List of checks names
         :type checks: list
         :param value: –
         :type value: –
         """
         for check in checks:
             self.checks[check] = value
 
-    def unset_checks(self, checks, value=False):
+    def unset_checks(self, checks: list, value=False) -> NoReturn:
         """
         :param checks: List of checks names
         :type checks: list
         :param value: –
         :type value: –
 
         .. sealso: set_checks()
         """
         self.set_checks(checks, value)
 
-    #--- PyScribus standard methods ----------------------------
+    # PyScribus standard methods -------------------------------
 
-    def toxml(self):
-        if self.checks:
-            xml = ET.Element("CheckProfile")
-            xml.attrib["Name"] = self.name
-            xml.attrib["autoCheck"] = bool_to_num(self.checks["auto"])
+    def toxml(self) -> BoolOrElement:
+        if not self.checks:
+            return False
 
-            for check in self.checks.keys():
-                if check != "auto":
-                    xml.attrib["check{}".format(check)] = bool_to_num(self.checks[check])
+        xml = ET.Element("CheckProfile")
+        xml.attrib["Name"] = self.name
 
-            for ignore in self.ignores.keys():
-                xml.attrib["ignore{}".format(ignore)] = bool_to_num(self.ignores[ignore])
+        xml.attrib["ignoreErrors"] = bool_to_num(self.ignores["Errors"])
 
-            for res in self.resolution.keys():
-                xml.attrib["{}Resolution".format(res)] = self.resolution[res].toxmlstr()
+        xml.attrib["autoCheck"] = bool_to_num(self.checks["auto"])
 
-            return xml
-        else:
-            return False
+        for check in [
+            "Glyphs",
+            "Orphans",
+            "Overflow",
+            "Pictures",
+            "PartFilledImageFrames",
+            "Resolution",
+            "Transparency",
+        ]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
+
+        for res in self.resolution.keys():
+            xml.attrib[f"{res}Resolution"] = self.resolution[res].toxmlstr()
+
+        for check in ["Annotations", "RasterPDF", "ForGIF"]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
 
-    def fromxml(self, xml):
+        xml.attrib["ignoreOffLayers"] = bool_to_num(self.ignores["OffLayers"])
+
+        for check in [
+            "NotCMYKOrSpot",
+            "DeviceColorsAndOutputIntent",
+            "FontNotEmbedded",
+            "FontIsOpenType",
+            "AppliedMasterDifferentSide",
+            "EmptyTextFrames",
+        ]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
+
+        return xml
+
+    def fromxml(self, xml: ET.Element) -> bool:
         name = xml.get("Name")
 
         if name is not None:
             self.name = name
 
         autocheck = xml.get("autoCheck")
 
@@ -1710,146 +2373,341 @@
             value = xml.get("{}Resolution".format(res))
 
             if value is not None:
                 self.resolution[res].value = int(value)
 
         return True
 
-    def fromdefault(self, name):
-        """
-        """
+    def fromdefault(self, name: str) -> bool:
+        """ """
 
-        if name in self.pyscribus_defaults:
-            self.name = name
+        if name not in self.pyscribus_defaults:
+            return False
 
-            if name in [
-                    "PDF 1.3", "PDF 1.4", "PDF 1.5", "PDF/X-1a", "PDF/X-3",
-                    "PDF/X-4", "PostScript"]:
-
-                self.ignores = {"Errors": False, "OffLayers": False}
-                self.resolution = {
-                    "min": dimensions.Dim(144, "dpi", True),
-                    "max": dimensions.Dim(2400, "dpi", True)
-                }
+        self.name = name
 
-            if name == "PDF 1.3":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "Transparency", "RasterPDF", "ForGIF",
-                        "FontNotEmbedded", "FontIsOpenType",
-                        "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+        if name in [
+            "PDF 1.3",
+            "PDF 1.4",
+            "PDF 1.5",
+            "PDF/X-1a",
+            "PDF/X-3",
+            "PDF/X-4",
+            "PostScript",
+        ]:
+
+            self.ignores = {"Errors": False, "OffLayers": False}
+            self.resolution = {
+                "min": dimensions.Dim(144, unit="dpi", integer=True),
+                "max": dimensions.Dim(2400, unit="dpi", integer=True),
+            }
+
+        if name == "PDF 1.3":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "Transparency",
+                    "RasterPDF",
+                    "ForGIF",
+                    "FontNotEmbedded",
+                    "FontIsOpenType",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "Annotations",
+                    "PartFilledImageFrames",
+                    "NotCMYKOrSpot",
+                    "DeviceColorsAndOutputIntent",
+                ]
+            )
+
+        if name == "PDF 1.4":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "RasterPDF",
+                    "ForGIF",
+                    "FontNotEmbedded",
+                    "FontIsOpenType",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                    "Resolution",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "checkPartFilledImageFrames",
+                    "checkTransparency",
+                    "checkAnnotations",
+                    "checkNotCMYKOrSpot",
+                    "checkDeviceColorsAndOutputIntent",
+                ]
+            )
+
+        if name == "PDF 1.5":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "RasterPDF",
+                    "ForGIF",
+                    "FontNotEmbedded",
+                    "FontIsOpenType",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "checkNotCMYKOrSpot",
+                    "checkDeviceColorsAndOutputIntent",
+                    "checkTransparency",
+                    "checkAnnotations",
+                    "PartFilledImageFrames",
+                ]
+            )
+
+        if name == "PDF/X-1a":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "Transparency",
+                    "Annotations",
+                    "RasterPDF",
+                    "ForGIF",
+                    "NotCMYKOrSpot",
+                    "FontNotEmbedded",
+                    "FontIsOpenType",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "checkPartFilledImageFrames",
+                    "checkDeviceColorsAndOutputIntent",
+                ]
+            )
+
+        if name == "PDF/X-3":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "Transparency",
+                    "Annotations",
+                    "RasterPDF",
+                    "ForGIF",
+                    "DeviceColorsAndOutputIntent",
+                    "FontNotEmbedded",
+                    "FontIsOpenType",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                ["checkPartFilledImageFrames", "checkNotCMYKOrSpot"]
+            )
+
+        if name == "PDF/X-4":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "Annotations",
+                    "RasterPDF",
+                    "ForGIF",
+                    "DeviceColorsAndOutputIntent",
+                    "FontNotEmbedded",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "checkPartFilledImageFrames",
+                    "checkTransparency",
+                    "checkNotCMYKOrSpot",
+                    "checkFontIsOpenType",
+                ]
+            )
+
+        if name == "PostScript":
+            self.set_checks(
+                [
+                    "auto",
+                    "Glyphs",
+                    "Orphans",
+                    "Overflow",
+                    "Pictures",
+                    "Resolution",
+                    "Transparency",
+                    "RasterPDF",
+                    "ForGIF",
+                    "AppliedMasterDifferentSide",
+                    "EmptyTextFrames",
+                ]
+            )
+
+            self.unset_checks(
+                [
+                    "checkPartFilledImageFrames",
+                    "checkAnnotations",
+                    "checkNotCMYKOrSpot",
+                    "checkDeviceColorsAndOutputIntent",
+                    "checkFontNotEmbedded",
+                    "checkFontIsOpenType",
+                ]
+            )
 
-                self.unset_checks(
-                    [
-                        "Annotations", "PartFilledImageFrames", "NotCMYKOrSpot",
-                        "DeviceColorsAndOutputIntent"
-                    ]
-                )
+        return True
 
-            if name == "PDF 1.4":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "RasterPDF", "ForGIF", "FontNotEmbedded", "FontIsOpenType",
-                        "AppliedMasterDifferentSide", "EmptyTextFrames",
-                        "Resolution"
-                    ]
-                )
 
-                self.unset_checks(
-                    [
-                        "checkPartFilledImageFrames", "checkTransparency",
-                        "checkAnnotations", "checkNotCMYKOrSpot",
-                        "checkDeviceColorsAndOutputIntent"
-                    ]
-                )
+class HyphenationRule(PyScribusElement):
+    """
+    Abstract class for hyphenation rules listed in <HYPHEN>.
+    """
 
-            if name == "PDF 1.5":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "RasterPDF", "ForGIF", "FontNotEmbedded",
-                        "FontIsOpenType", "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+    def __init__(self, rule_type: str):
+        super().__init__()
 
-                self.unset_checks(
-                    [
-                        "checkNotCMYKOrSpot", "checkDeviceColorsAndOutputIntent",
-                        "checkTransparency", "checkAnnotations", "PartFilledImageFrames"
-                    ]
-                )
+        if rule_type == "exception":
+            self.tag = "EXCEPTION"
+        if rule_type == "exclusion":
+            self.tag = "IGNORE"
 
-            if name == "PDF/X-1a":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "Transparency", "Annotations", "RasterPDF",
-                        "ForGIF", "NotCMYKOrSpot", "FontNotEmbedded", "FontIsOpenType",
-                        "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+        self.word = None
 
-                self.unset_checks(
-                    [
-                        "checkPartFilledImageFrames",
-                        "checkDeviceColorsAndOutputIntent"
-                    ]
-                )
+    # PyScribus standard methods -------------------------------
 
-            if name == "PDF/X-3":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "Transparency", "Annotations", "RasterPDF",
-                        "ForGIF", "DeviceColorsAndOutputIntent", "FontNotEmbedded",
-                        "FontIsOpenType", "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+    def toxml(self) -> BoolOrElement:
+        xml = ET.Element(self.tag)
 
-                self.unset_checks(
-                    [
-                        "checkPartFilledImageFrames", "checkNotCMYKOrSpot"
-                    ]
-                )
+        xml.attrib["WORD"] = self.word
 
-            if name == "PDF/X-4":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "Annotations", "RasterPDF", "ForGIF",
-                        "DeviceColorsAndOutputIntent", "FontNotEmbedded",
-                        "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+        return xml
 
-                self.unset_checks(
-                    [
-                        "checkPartFilledImageFrames", "checkTransparency",
-                        "checkNotCMYKOrSpot", "checkFontIsOpenType"
-                    ]
-                )
+    def fromxml(self, xml: ET.Element) -> bool:
+        word = xml.get("WORD")
 
-            if name == "PostScript":
-                self.set_checks(
-                    [
-                        "auto", "Glyphs", "Orphans", "Overflow", "Pictures",
-                        "Resolution", "Transparency", "RasterPDF", "ForGIF",
-                        "AppliedMasterDifferentSide", "EmptyTextFrames"
-                    ]
-                )
+        if word is None:
+            return False
 
-                self.unset_checks(
-                    [
-                        "checkPartFilledImageFrames", "checkAnnotations",
-                        "checkNotCMYKOrSpot", "checkDeviceColorsAndOutputIntent",
-                        "checkFontNotEmbedded", "checkFontIsOpenType"
-                    ]
-                )
+        self.word = word
 
-        else:
-            return False
+        return True
+
+
+class HyphenationException(HyphenationRule):
+    """
+    Hyphenation exception rule (DOCUMENT/HYPHEN/EXCEPTION).
+    """
+
+    def __init__(self):
+        HyphenationRule.__init__(self, "exception")
+
+    def toxml(self) -> BoolOrElement:
+        xml = HyphenationRule.toxml(self)
+        xml.attrib["HYPHENATED"] = self.word
+
+        return xml
+
+
+class HyphenationExclusion(HyphenationRule):
+    """
+    Hyphenation exclusion rule (DOCUMENT/HYPHEN/IGNORE).
+    """
+
+    def __init__(self):
+        HyphenationRule.__init__(self, "exclusion")
+
+
+class Hyphenation(PyScribusElement):
+    """
+    Hyphenation settings of the document (DOCUMENT/HYPHEN).
+    """
+
+    def __init__(self, default=False):
+        super().__init__()
+
+        self.rules = []
+
+        if default:
+            self.fromdefault(default)
+
+    # PyScribus standard methods -------------------------------
+
+    def toxml(self) -> BoolOrElement:
+        xml = ET.Element("HYPHEN")
+
+        for rule in self.rules:
+            rule_xml = rule.toxml()
+            xml.append(rule_xml)
+
+        return xml
+
+    def fromxml(self, xml: ET.Element) -> bool:
+        for element in xml:
+
+            if element.tag not in ["EXCEPTION", "IGNORE"]:
+                continue
+
+            if element.tag == "EXCEPTION":
+                new_rule = HyphenationException()
+
+            if element.tag == "IGNORE":
+                new_rule = HyphenationExclusion()
+
+            if new_rule.fromxml(element):
+                self.rules.append(new_rule)
+
+        return True
+
+    def fromdefault(self, name: str) -> bool:
+        """
+        Set default settings for hyphenation.
+
+        By default, there is no rules (this does not mean anomy).
+
+        :rtype: bool
+        """
+
+        self.rules = []
+
+        return True
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/exceptions.py` & `pyscribus-backported-0.3/pyscribus/model/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,110 +21,123 @@
 Exceptions raised by PyScribus.
 """
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class InsaneSLAValue(Exception):
     """
     Exception raised if a XML value or a set of XML values is/are
     not possible, are both in contradiction.
 
     This usually happens if someone edited a SLA file and wroted some
     wrong values in it.
 
     For example, a list can't be a numeroted and bullet one, Scribus UI
     doesn't allow that but manual SLA editing does.
     """
-    pass
 
 
 class MissingSLAAttribute(Exception):
     """
     Exception raised when a mandatory XML attribute in SLA file is missing.
 
     An exception more precise than InsaneSLAValue.
     """
-    pass
 
 
 class ConflictingLayer(Exception):
     """
-    Exception raised if a document Layer have same attributes that an other one.
+    Exception raised if a document Layer have same attributes that an other
+    one.
     """
-    pass
+
 
 # --- Items attributes -----------------------------------------
 
+
 class UnknownOrEmptyItemAttributeType(Exception):
     """
-    Exception raised when a itemattribute.ItemAttribute (and inherited
+    Exception raised when a ``itemattribute.ItemAttribute`` (and inherited
     classes) has a unknown or empty type, as it is not in
-    itemattribute.ItemAttribute.attrib_types
+    ``itemattribute.ItemAttribute.attrib_types``
     """
-    pass
+
 
 # --- Quick setup ----------------------------------------------
 
+
 class QuickSetupInvalidValue(Exception):
     """
     Exception raised when a quick setup value is invalid.
     """
-    pass
+
 
 # --- Unknown SLA references -----------------------------------
 
+
 class UnknownLayer(Exception):
     """
-    Exception raised if a SLA element points to a layer unknown to the document.
+    Exception raised if a SLA element points to a layer unknown to the
+    document.
     """
-    pass
 
 
 class UnknownStyleInStory(Exception):
     """
-    Exception raised if a SLA element points to a style unknown to the document.
+    Exception raised if a SLA element points to a style unknown to the
+    document.
     """
-    pass
 
 
 class InvalidColor(Exception):
     """
     Exception raised when color inks (CMYK or RGB) are invalid, incomplete
     or doesn't even exists.
 
-    RGB inks must range from 0 to 255.
-    CMYK inks must range from 0 to 100.
+    - RGB inks must range from 0 to 255.
+    - CMYK inks must range from 0 to 100.
+    """
+
+
+class ColorMixing(Exception):
+    """
+    Exception raised when two colors do not share the same color space (CMYK
+    or RVB).
     """
-    pass
 
 
 class UnknownRenderBufferProperty(Exception):
     """
     Exception raised when a render buffer property is missing.
     """
-    pass
+
 
 # --- dimensions -----------------------------------------------
 
+
 class UnknownDimUnit(Exception):
-    pass
+    """
+    That ``dimensions.Dim`` unit is not handled.
+    """
 
 
 class InvalidDim(Exception):
     """
-    Exception raised if a dimensions.Dim value is impossible according to its
-    unit.
+    Exception raised if a ``dimensions.Dim`` value is impossible according
+    to its unit.
 
-    Pica points must no be inferior to 0.
-    (Ordinary) angle (deg unit) must range from 0 to 180.
-    Calligraphic pen angle (cdeg unit) must range from 0 to 180.
+    - Pica points must no be inferior to 0.
+    - (Ordinary) angle (deg unit) must range from 0 to 180.
+    - Calligraphic pen angle (cdeg unit) must range from 0 to 180.
     """
-    pass
 
 
 class IncompatibleDim(Exception):
-    """Exception raised on incompatible dimensions.Dim units conversions."""
-    pass
+    """
+    Exception raised on incompatible ``dimensions.Dim`` units conversions.
+    """
+
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/extra/__init__.py` & `pyscribus-backported-0.3/pyscribus/model/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-backported-0.2.4/pyscribus/extra/wireframe.py` & `pyscribus-backported-0.3/pyscribus/model/extra/wireframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,27 @@
 """
 Reads SLA file and use Pillow to draw a schematic picture of all page
 and page objects.
 """
 
 # Imports ===============================================================#
 
-import math
-
 from PIL import Image, ImageDraw
 
-import pyscribus.dimensions as dimensions
-import pyscribus.pageobjects as pageobjects
-import pyscribus.pages as pages
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.pageobjects as pageobjects
+import pyscribus.model.pages as pages
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class WireframeObject:
     """
     Wireframe object : something to draw on the wireframe, like pages,
     page objects.
 
     :type sla_object: pyscribus.pages.Page, pyscribus.pageobjects.PageObject
     :param sla_object: PyScribus instance of drawnable object
@@ -54,35 +53,32 @@
         self.is_page = False
         self.type = "undefined"
         self.group_objects = []
 
         # Pages have layer -1, as 0 is the lower layer available
         self.layer = -1
 
-        self.draw_settings = {
-            "fill": "",
-            "outline": "",
-            "bleed": "red"
-        }
+        self.draw_settings = {"fill": "", "outline": "", "bleed": "red"}
 
         if sla_object:
             self.from_object(sla_object)
 
     def from_object(self, sla_object):
 
         if isinstance(sla_object, pages.Page):
             self.is_page = True
             self.type = "page"
         else:
             self.is_page = False
             type_ok = False
 
             for class_test in [
-                    pageobjects.LatexObject,
-                    pageobjects.RenderObject]:
+                pageobjects.LatexObject,
+                pageobjects.RenderObject,
+            ]:
 
                 if isinstance(sla_object, class_test):
                     self.type = "render"
                     type_ok = True
                     break
 
             if not type_ok:
@@ -111,36 +107,35 @@
 
     def draw_on_canvas(self, canvas, bleed=False):
 
         if bleed and self.bleed:
             tx = self.box.coords["top-left"][0].value - self.bleed["left"]
             ty = self.box.coords["top-left"][1].value - self.bleed["top"]
             bx = self.box.coords["bottom-right"][0].value + self.bleed["right"]
-            by = self.box.coords["bottom-right"][1].value + self.bleed["bottom"]
+            by = (
+                self.box.coords["bottom-right"][1].value + self.bleed["bottom"]
+            )
 
             bleed_rect = ((tx, ty), (bx, by))
             canvas.rectangle(bleed_rect, outline="red")
 
         rect = (
-            (
-                self.box.coords["top-left"][0],
-                self.box.coords["top-left"][1]
-            ),
+            (self.box.coords["top-left"][0], self.box.coords["top-left"][1]),
             (
                 self.box.coords["bottom-right"][0],
-                self.box.coords["bottom-right"][1]
+                self.box.coords["bottom-right"][1],
             ),
         )
 
         if self.draw_settings["fill"] and self.draw_settings["outline"]:
 
             canvas.rectangle(
                 rect,
                 fill=self.draw_settings["fill"],
-                outline=self.draw_settings["outline"]
+                outline=self.draw_settings["outline"],
             )
 
         else:
 
             if self.draw_settings["fill"]:
                 canvas.rectangle(rect, fill=self.draw_settings["fill"])
 
@@ -178,16 +173,18 @@
     }
 
     def __init__(self):
         self.pages = []
         self.page_objects = []
 
         self.bleed = {
-            "top": dimensions.Dim(0), "right": dimensions.Dim(0),
-            "left": dimensions.Dim(0), "bottom": dimensions.Dim(0)
+            "top": dimensions.Dim(0),
+            "right": dimensions.Dim(0),
+            "left": dimensions.Dim(0),
+            "bottom": dimensions.Dim(0),
         }
 
     def from_sla(self, sla):
         """
         Load all drawnable objects of sla file.
 
         :type sla: string
@@ -201,29 +198,28 @@
             self.pages.append(wo)
 
         for pago in sla.document.page_objects:
             wo = WireframeObject(pago)
             self.page_objects.append(wo)
 
     def append(self, sla_object):
-
         def add(obj, sla_obj):
             if sla_obj.is_page:
                 obj.pages.append(sla_obj)
             else:
                 obj.page_objects.append(sla_obj)
 
             return obj
 
         if isinstance(sla_object, WireframeObject):
             self = add(self, sla_object)
         else:
             self = add(self, WireframeObject(sla_object))
 
-    def _image_size(self, margins=[0,0]):
+    def _image_size(self, margins=[0, 0]):
         max_x = float()
         max_y = float()
 
         for po in self.page_objects:
             trx = po.box.coords["top-right"][0].value
             bry = po.box.coords["bottom-right"][1].value
 
@@ -280,25 +276,25 @@
         draw_pages = "all"
         draw_layers = "all"
         draw_landmark = True
         draw_bleed = True
 
         out_file = False
 
-        canvas_margins = [0,0]
+        canvas_margins = [0, 0]
         background_color = "grey"
 
         default_outline = "black"
 
         use_stylesheet = False
         stylesheet = Wireframe.stylesheet
 
         # --- Options processing ------------------------------------
 
-        for opt_name,opt_value in kwargs.items():
+        for opt_name, opt_value in kwargs.items():
 
             if opt_name == "layers":
                 draw_layers = opt_value
 
             if opt_name == "pages":
 
                 if isinstance(opt_value, bool):
@@ -315,24 +311,18 @@
             if opt_name == "background":
                 background_color = opt_value
 
             if opt_name == "default_outline":
                 default_outline = opt_value
 
             if opt_name == "landmark":
-                if opt_value:
-                    draw_landmark = True
-                else:
-                    draw_landmark = False
+                draw_landmark = bool(opt_value)
 
             if opt_name == "bleed":
-                if opt_value:
-                    draw_bleed = True
-                else:
-                    draw_bleed = False
+                draw_bleed = bool(opt_value)
 
             if opt_name == "stylesheet":
 
                 if isinstance(opt_value, bool):
                     if opt_value:
                         use_stylesheet = True
                 else:
@@ -348,16 +338,16 @@
 
         image = Image.new("RGB", image_size, color=background_color)
         canvas = ImageDraw.Draw(image)
 
         # --- Drawing landmark --------------------------------------
 
         if draw_landmark:
-            canvas.line(((-5,0),(5,0)), fill="red")
-            canvas.line(((0,-5),(0,-5)), fill="red")
+            canvas.line(((-5, 0), (5, 0)), fill="red")
+            canvas.line(((0, -5), (0, -5)), fill="red")
 
         # --- Using default_outline or stylesheet -------------------
 
         if use_stylesheet:
             # --- Using stylesheet ----------------------------------
 
             for object_set in [self.pages, self.page_objects]:
@@ -366,27 +356,32 @@
                     key = False
 
                     if obj.type in stylesheet:
                         key = obj.type
 
                     if key:
                         obj.draw_settings["fill"] = stylesheet[key]["fill"]
-                        obj.draw_settings["outline"] = stylesheet[key]["outline"]
+                        obj.draw_settings["outline"] = stylesheet[key][
+                            "outline"
+                        ]
 
         else:
             # --- Using default_outline if no defined outline -------
 
             if default_outline:
 
                 for object_set in [self.pages, self.page_objects]:
 
                     for obj in object_set:
                         drawed = False
 
-                        if obj.draw_settings["fill"] or obj.draw_settings["outline"]:
+                        if (
+                            obj.draw_settings["fill"]
+                            or obj.draw_settings["outline"]
+                        ):
                             drawed = True
 
                         if not drawed:
                             obj.draw_settings["outline"] = default_outline
 
             # -------------------------------------------------------
 
@@ -422,11 +417,12 @@
 
         # -----------------------------------------------------------
 
         if out_file:
             image.save(out_file)
 
             return True
-        else:
-            return image
+
+        return image
+
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/headless/__init__.py` & `pyscribus-backported-0.3/pyscribus/model/headless/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Imports ===============================================================#
 
 import copy
 import subprocess
 
 from pathlib import Path
 
-import pyscribus.headless.scripts.topdf as script_to_pdf
+import pyscribus.model.headless.scripts.topdf as script_to_pdf
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 SCRIPTS = {
     "topdf": script_to_pdf,
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/headless/scripts/topdf.py` & `pyscribus-backported-0.3/pyscribus/model/headless/scripts/topdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Usage in Pyscribus:
 
 :Example:
 
 .. code:: python
 
-   from pyscribus.headless import run_pyh_script
+   from pyscribus.model.headless import run_pyh_script
    run_pyh_script("topdf", sla_input="/home/user/example.sla")
 
 Usage in command-line:
 
 .. code:: bash
 
    scribus -g -py to-pdf.py -- file.sla
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/itemattribute.py` & `pyscribus-backported-0.3/pyscribus/model/itemattribute.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,52 +19,60 @@
 
 """
 Item attributes for document, page objects.
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+from typing import Union, NoReturn
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class ItemAttribute(PyScribusElement):
     attrib_types = ["boolean", "integer", "double", "string", "none"]
 
-    #--- FIXME Not documented -----------------------------
+    # FIXME Not documented --------------------------------
     # Parameter=""
     # Relationship="none"
     # RelationshipTo=""
     # AutoAddTo="none"
 
-    #--- NOTE Examples in SLA -----------------------------
+    # NOTE Examples in SLA --------------------------------
     # Name="entier" Type="integer" Value="1"
     # Name="reel" Type="double" Value="-5"
     # Name="chaine" Type="string" Value="&quot;Test&quot;"
     # Name="" Type="none" Value=""
 
     def __init__(self):
         super().__init__()
 
         self.name = ""
         self.attribute_type = "none"
         self.value = ""
 
     def as_python(
-            self, bool_keywords={"true": "True", "false": "False"},
-            lower_bool=False):
+        self,
+        bool_keywords: dict={"true": "True", "false": "False"},
+        lower_bool: bool=False,
+    ) -> Union[int, str, bool]:
         """
         Returns the value of ItemAttribute.value as a valid python
         object (int for integer, bool for boolean, etc).
 
         :type bool_keywords: dict
         :param bool_keywords: Dictionnary of true and false values to test
             against. If bool_keywords["true"] is equal to
@@ -82,42 +90,43 @@
         - str object if attribute type is "string"
         - bool object if attribute type is "boolean"
         - str if attribute_type is "none", as attribute_type "none" allows
             other values than None.
 
         Raise a ValueError if attribute_type is empty/unknown.
 
-        :rtype: int,long,string,boolean
+        :rtype: int,float,string,boolean
         """
 
         if self.attribute_type == "integer":
             return int(self.value)
-        elif self.attribute_type == "double":
+
+        if self.attribute_type == "double":
             return float(self.value)
-        elif self.attribute_type == "string":
+
+        if self.attribute_type == "string":
             # FIXME TODO Escape &quot; and other entities in unicode caracters
             return str(self.value)
-        elif self.attribute_type == "none":
+
+        if self.attribute_type == "none":
             return self.value
-        elif self.attribute_type == "boolean":
+
+        if self.attribute_type == "boolean":
+            tested = str(self.value)
+
             if lower_bool:
-                v = str(self.value).lower()
-            else:
-                v = str(self.value)
-
-            if v == bool_keywords["true"]:
-                return True
-            else:
-                return False
-        else:
-            raise exceptions.UnknownOrEmptyItemAttributeType()
+                tested = tested.lower()
 
-    #--- PyScribus standard methods ----------------------------
+            return tested == bool_keywords["true"]
 
-    def fromxml(self, xml):
+        raise exceptions.UnknownOrEmptyItemAttributeType()
+
+    # PyScribus standard methods -------------------------------
+
+    def fromxml(self, xml: ET.Element) -> bool:
         name = xml.get("Name")
 
         if name is not None:
             self.name = name
 
         atype = xml.get("Type")
 
@@ -130,42 +139,43 @@
         if v is not None:
             self.value = v
 
         # TODO
 
         return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("ItemAttribute")
 
         xml.attrib["Name"] = self.name
         xml.attrib["Type"] = self.attribute_type
         xml.attrib["Value"] = self.value
 
         # TODO
 
         return xml
 
-    def fromdefault(self):
+    def fromdefault(self) -> NoReturn:
         # TODO
 
         self.attribute_type = "none"
 
 
 class DocumentAttribute(ItemAttribute):
     """
     Item attribute at document level
     """
 
-    def __init__(self):
-        super().__init__()
+    # def __init__(self):
+        # super().__init__()
 
 
 class PageObjectAttribute(ItemAttribute):
     """
     Item attribute at page object level
     """
 
-    def __init__(self):
-        super().__init__()
+    # def __init__(self):
+        # super().__init__()
+
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/layers.py` & `pyscribus-backported-0.3/pyscribus/model/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 from __future__ import annotations
 
 from typing import Union, NoReturn
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/logs.py` & `pyscribus-backported-0.3/pyscribus/model/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,44 +19,48 @@
 
 """
 Logging for PyScribus
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
 import os
 import logging
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 USE_LOG = False
 
 # Fonctions =============================================================#
 
+
 def init_logging(
-        filepath="test.log",
-        formatstr="%(asctime)s:%(levelname)s:%(message)s"):
+    filepath="test.log", formatstr="%(asctime)s:%(levelname)s:%(message)s"
+):
     global USE_LOG
 
     logger = getLogger()
 
     filepath = os.path.realpath(filepath)
 
     logging.basicConfig(
-        filename=filepath,
-        level=logging.DEBUG,
-        format=formatstr
+        filename=filepath, level=logging.DEBUG, format=formatstr
     )
 
     USE_LOG = True
 
+
 def getLogger():
     global USE_LOG
 
     if USE_LOG:
-        return logging.getLogger('pyscribus')
-    else:
-        return False
+        return logging.getLogger("pyscribus")
+
+    return False
+
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/marks.py` & `pyscribus-backported-0.3/pyscribus/model/marks.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,91 +19,92 @@
 
 """
 Classes related to marks management
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+from typing import NoReturn, Literal, Optional, Union
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.exceptions as exceptions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.exceptions as exceptions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
-mark_type_xml = {
-    "anchor": "0",
-    "objectref": "1",
-    "markref": "2",
-    "variable": "3",
-    "note": "4",
-}
+MarkType = Literal["anchor", "objectref", "markref", "variable", "note"]
 
 # Classes ===============================================================#
 
+
 class DocumentMark(xmlc.PyScribusElement):
     """
     Mark element (DOCUMENT/Marks/Mark)
     """
 
-    def __init__(self):
-        global mark_type_xml
+    type_xml = {
+        "anchor": "0",
+        "objectref": "1",
+        "markref": "2",
+        "variable": "3",
+        "note": "4",
+    }
 
+    def __init__(self):
         super().__init__()
 
         self.type = ""
         self.name = ""
         self.label = ""
 
         self.target_object = None
         self.target_mark = {"label": None, "type": "-1"}
 
-        self.pyscribus_defaults = [k for k in mark_type_xml.keys()]
+        self.pyscribus_defaults = [k for k in DocumentMark.type_xml.keys()]
 
-    def fromdefault(self, default):
+    def fromdefault(self, default: str) -> bool:
         """
         :type default: string
         :param default: Set of default settings to apply
         :rtype: boolean
         """
 
         if default in self.pyscribus_defaults:
             self.type = default
 
             return True
-        else:
-            return False
 
-    def set_type(self, mtype):
+        return False
+
+    def set_type(self, mtype: MarkType) -> bool:
         """
         :type mtype: string
-        :param mtype: Mark type in pyscribus.marks.mark_type_xml keys()
+        :param mtype: Mark type in pyscribus.marks.DocumentMark.type_xml keys()
         :rtype: boolean
         :returns: True if setting type succeed
         """
-        global mark_type_xml
 
-        if mtype in mark_type_xml.keys():
-            self.type = mark_type_xml[mtype]
+        if mtype in DocumentMark.type_xml.keys():
+            self.type = DocumentMark.type_xml[mtype]
             return True
 
-        else:
-            return False
+        return False
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         :rtype: lxml.etree._Element
         :returns: XML representation of document mark
         """
-
-        global mark_type_xml
-
         xml = ET.Element("Mark")
 
         if self.type:
 
             # --- Label -----------------------------------------------------
 
             # When @type is "3" (variable text), @str acts as @label
@@ -116,95 +117,94 @@
             if self.type == "variable":
                 xml.attrib["label"] = self.name
             else:
                 xml.attrib["label"] = self.label
 
             # ---------------------------------------------------------------
 
-            xml.attrib["type"] = mark_type_xml[self.type]
+            xml.attrib["type"] = DocumentMark.type_xml[self.type]
 
             if self.type == "variable":
                 xml.attrib["str"] = self.label
 
             if self.type == "objectref":
                 xml.attrib["ItemID"] = self.target_object
 
             if self.type == "markref":
                 xml.attrib["MARKlabel"] = self.target_mark["label"]
-                xml.attrib["MARKtype"] = mark_type_xml[self.target_mark["type"]]
+                xml.attrib["MARKtype"] = DocumentMark.type_xml[
+                    self.target_mark["type"]
+                ]
 
         else:
             raise exceptions.InsaneSLAValue("Invalid Marks/Mark @type")
 
         return xml
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
-        global mark_type_xml
-
-        if xml.tag == "Mark":
-            mtype = xml.get("type")
+        if xml.tag != "Mark":
+            return False
 
-            if mtype is not None:
-                for h,x in mark_type_xml.items():
-                    if mtype == x:
-                        self.type = h
-                        break
+        mtype = xml.get("type")
 
-            # --- Name and/or label -----------------------------------------
-
-            # When @type is "3" (variable text), @str acts as @label
-            # in other @types, and @label acts as a mark identifier.
-            #
-            # So :
-            #   DocumentMark.name  = @label if @type == "3"
-            #   DocumentMark.label = @label if @type != "3"
-
-            mlabel = xml.get("label")
-            if mlabel is not None:
-                if self.type == "variable":
-                    self.name = mlabel
-                else:
-                    self.label = mlabel
+        if mtype is not None:
+            for human, code in DocumentMark.type_xml.items():
+                if mtype == code:
+                    self.type = human
+                    break
+
+        # --- Name and/or label -----------------------------------------
+
+        # When @type is "3" (variable text), @str acts as @label
+        # in other @types, and @label acts as a mark identifier.
+        #
+        # So :
+        #   DocumentMark.name  = @label if @type == "3"
+        #   DocumentMark.label = @label if @type != "3"
 
+        mlabel = xml.get("label")
+        if mlabel is not None:
             if self.type == "variable":
-                mstr = xml.get("str")
-                if mstr is not None:
-                    self.label = mstr
-
-            # ---------------------------------------------------------------
-
-            if self.type == "objectref":
-                mitem = xml.get("ItemID")
-                if mitem is not None:
-                    self.target_object = mitem
-
-            if self.type == "markref":
-                mtarget_label = xml.get("MARKlabel")
-                if mtarget_label is not None:
-                    self.target_mark["label"] = mtarget_label
-
-                mtarget_type = xml.get("MARKtype")
-                if mtarget_type is not None:
-
-                    if mtarget_type in mark_type_xml.values():
-                        self.target_mark["type"] = mark_type_xml[mtarget_type]
-                    else:
-                        raise exceptions.InsaneSLAValue(
-                            "Invalid Marks/Mark @type"
-                        )
+                self.name = mlabel
+            else:
+                self.label = mlabel
 
-            return True
+        if self.type == "variable":
+            mstr = xml.get("str")
+            if mstr is not None:
+                self.label = mstr
+
+        # ---------------------------------------------------------------
+
+        if self.type == "objectref":
+            mitem = xml.get("ItemID")
+            if mitem is not None:
+                self.target_object = mitem
+
+        if self.type == "markref":
+            mtarget_label = xml.get("MARKlabel")
+            if mtarget_label is not None:
+                self.target_mark["label"] = mtarget_label
+
+            mtarget_type = xml.get("MARKtype")
+            if mtarget_type is not None:
+
+                if mtarget_type in DocumentMark.type_xml.values():
+                    self.target_mark["type"] = DocumentMark.type_xml[
+                        mtarget_type
+                    ]
+                else:
+                    raise exceptions.InsaneSLAValue("Invalid Marks/Mark @type")
 
-        else:
-            return False
+        return True
 
 
 class StoryMarkAbstract(xmlc.PyScribusElement):
     """
     Abstract class for MARK elements in Scribus stories.
 
     :type mark_type: str
@@ -213,152 +213,206 @@
     :param label: Mark label
     :type features: dict
     :param features: Text formatting features as dict
 
     .. seealso:: :class:`pyscribus.stories.StoryNoteMark`
     """
 
-    def __init__(self, mark_type, label="", features=False):
-        global mark_type_xml
-
+    def __init__(
+        self,
+        mark_type: MarkType,
+        label: str = "",
+        features: Optional[dict] = False,
+    ):
         super().__init__()
 
         self.features = {
             "inherit": False,
             "superscript": False,
         }
 
         self.label = label
 
-        if mark_type in mark_type_xml:
+        if mark_type in DocumentMark.type_xml:
             self.type = mark_type
         else:
             raise ValueError("Unknown mark type")
 
         if features:
             self.set_features(features)
 
-    def fromxml(self, xml):
-        global mark_type_xml
-
-        if xml.tag == "MARK":
-
-            mtype = xml.get("type")
-            if mtype is not None:
-                for h,x in mark_type_xml.items():
-                    if mtype == x:
-                        self.type = h
-                        break
-
-            mlabel = xml.get("label")
-            if mlabel is not None:
-                self.label = mlabel
-
-            mfeatures = xml.get("features")
-            if mfeatures is not None:
-                self.set_features(mfeatures)
-
-            return True
+    def fromxml(self, xml: ET.Element) -> bool:
+        if xml.tag != "MARK":
+            return False
 
-        return False
+        mtype = xml.get("type")
+        if mtype is not None:
+            for human, code in DocumentMark.type_xml.items():
+                if mtype == code:
+                    self.type = human
+                    break
+
+        mlabel = xml.get("label")
+        if mlabel is not None:
+            self.label = mlabel
+
+        mfeatures = xml.get("features")
+        if mfeatures is not None:
+            self.set_features(mfeatures)
 
-    def toxml(self):
-        global mark_type_xml
+        return True
 
+    def toxml(self) -> ET.Element:
         xml = ET.Element("MARK")
 
-        xml.attrib["type"] = mark_type_xml[self.type]
+        xml.attrib["type"] = DocumentMark.type_xml[self.type]
         xml.attrib["label"] = self.label
 
         have_features = len([f for f in self.features.values() if f])
 
         if have_features:
             features = []
 
-            for f,v in self.features.items():
-                if v:
-                    features.append(f)
+            for feature_name, feature_value in self.features.items():
+                if feature_value:
+                    features.append(feature_name)
 
             features = " ".join(features)
 
             xml.attrib["FEATURES"] = features
 
         return xml
 
-    def set_features(self, features):
+    def set_features(self, features: str):
         """
         :type features: str
         :param features: Formatting features as string separated by spaces.
             Ex: ``"inherit superscript"``
         :rtype: bool
         :returns: False if one features was not set.
         """
 
         features = features.split()
 
         fset = 0
 
         for feature in features:
-            if feature in self.features.keys():
+            if feature in self.features:
                 self.features[feature] = True
                 fset += 1
 
-        if fset == len(features):
-            return True
-        else:
-            return False
+        return fset == len(features)
 
 
 class StoryNoteMark(StoryMarkAbstract):
     """
     Mark (MARK) for a (foot|end)note in Scribus stories.
     """
 
-    def __init__(self, label="", features=False):
+    def __init__(
+        self,
+        label: str = "",
+        features: Optional[dict] = False,
+        default: bool = False
+    ):
         StoryMarkAbstract.__init__(self, "note", label, features)
 
-    def fromdefault(self):
+        if default:
+            self.fromdefault()
+
+    def fromdefault(self) -> NoReturn:
         self.set_features("inherit superscript")
 
     def __repr__(self):
         return "NOTEMARK|{}|{}".format(
             self.label,
-            [k for k,v in self.features.items() if self.features[k]]
+            [k for k in self.features if bool(k)],
         )
 
 
 class StoryVariableMark(StoryMarkAbstract):
     """
     Variable text mark
     """
 
-    def __init__(self, label=""):
+    def __init__(self, label: str = ""):
         StoryMarkAbstract.__init__(self, "variable", label, False)
 
 
 class StoryAnchorMark(StoryMarkAbstract):
     """
     Anchor mark
     """
 
-    def __init__(self, label=""):
+    def __init__(self, label: str = ""):
         StoryMarkAbstract.__init__(self, "anchor", label, False)
 
 
 class StoryPageObjectRefMark(StoryMarkAbstract):
     """
     Reference to a page object mark
     """
 
-    def __init__(self, label=""):
+    def __init__(self, label: str = ""):
         StoryMarkAbstract.__init__(self, "objectref", label, False)
 
 
 class StoryMarkRefMark(StoryMarkAbstract):
     """
     Reference to a mark... mark
     """
 
-    def __init__(self, label=""):
+    def __init__(self, label: str = ""):
         StoryMarkAbstract.__init__(self, "markref", label, False)
 
+
+def story_mark_from_xml(
+    xml: ET.Element,
+) -> Union[
+    StoryAnchorMark,
+    StoryPageObjectRefMark,
+    StoryMarkRefMark,
+    StoryVariableMark,
+    StoryNoteMark,
+]:
+    """
+    Return the relevant subclass of StoryMarkAbstract from a story mark
+    XML element.
+    """
+
+    mark_type = xml.get("type")
+
+    if mark_type is None:
+        return False
+
+    # Match StoryMarkAbstract subclass to a mark type encoded in MARK/@type
+
+    mark_class = None
+
+    for human, code in DocumentMark.type_xml.items():
+        if mark_type == code:
+            mark_class = {
+                "anchor": StoryAnchorMark,
+                "objectref": StoryPageObjectRefMark,
+                "markref": StoryMarkRefMark,
+                "variable": StoryVariableMark,
+                "note": StoryNoteMark,
+            }[human]
+            break
+
+    if mark_class is None:
+        return False
+
+    # Initialize new mark ---------------------------------
+
+    new_mark = mark_class()
+    success = new_mark.fromxml(xml)
+
+    # Or fail to do so
+
+    if not success:
+        return False
+
+    return new_mark
+
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/notes.py` & `pyscribus-backported-0.3/pyscribus/model/notes.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,146 +19,191 @@
 
 """
 PyScribus classes for notes
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+import copy
+
+from typing import Union, NoReturn
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
+import pyscribus.model.exceptions as exceptions
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class Note(PyScribusElement):
     """
     Note element (Note)
     """
 
-    def __init__(self):
+    def __init__(self, doc_parent=False):
         PyScribusElement.__init__(self)
 
         self.style = ""
         self.parent_mark = ""
         self.parent_frame = ""
-        self.text = NoteText()
 
-    def fromdefault(self):
+        self.doc_parent = doc_parent
+
+        self.text = NoteText(parent_note=self)
+
+    def fromdefault(self) -> NoReturn:
         self.style = "Default"
         self.text = NoteText()
         self.text.fromdefault()
 
-    def get_parent_mark(self):
-        return "NoteMark_{} in frame {}".format(
-            self.style, self.parent_frame
-        )
+    def get_parent_mark(self) -> str:
+        return "NoteMark_{} in frame {}".format(self.style, self.parent_frame)
+
+    def fromxml(self, xml: ET.Element) -> bool:
 
-    def fromxml(self, xml):
+        if xml.tag != "Note":
+            return False
 
-        if xml.tag == "Note":
-            style = xml.get("NStyle")
-            parent_mark = xml.get("Master")
+        style = xml.get("NStyle")
+        parent_mark = xml.get("Master")
 
-            if style is not None:
-                self.style = style
+        if style is not None:
+            self.style = style
 
-            if parent_mark is not None:
-                self.parent_mark = parent_mark
-                self.parent_frame = self.parent_mark.split("in frame ")[-1]
+        if parent_mark is not None:
+            self.parent_mark = parent_mark
+            self.parent_frame = self.parent_mark.split("in frame ")[-1]
 
-            if "Text" in xml.attrib:
-                text = NoteText()
-                success = text.fromxml(xml)
+        if "Text" in xml.attrib:
+            text = NoteText()
+            success = text.fromxml(xml)
 
-                if success:
-                    self.text = text
+            if success:
+                self.text = text
 
-            return True
-        else:
-            return False
+        return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("Note")
 
         xml.attrib["Master"] = self.get_parent_mark()
         xml.attrib["NStyle"] = self.style
         xml.attrib["Text"] = self.text.toxmlstr()
 
         return xml
 
 
 class NoteText(PyScribusElement):
     """
     Note element text (Note/@Text).
 
-    Note element text consists in a full XML file dumped into
-    @Text attribute of Note, hence the need for a specific
-    class.
+    Note element text consists in a full XML file dumped into @Text attribute
+    of Note, hence the need for a specific class.
     """
 
-    #Text="&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt;&lt;SCRIBUSTEXT &gt;&lt;defaultstyle /&gt;&lt;p &gt;&lt;style /&gt;&lt;span &gt;&lt;charstyle Features=&quot;inherit &quot; /&gt; Pri tiuj ĉi ideoj « estas modo » paroli ne alie, ol kun ironia kaj malestima rideto, tial tiel agas ankaŭ A kaj B kaj C, kaj ĉiu el ili timas enpensiĝi serioze eĉ unu minuton pri la mokata ideo, ĉar li « scias antaŭe », ke « ĝi krom malsaĝaĵo enhavas ja nenion », kaj li timas, ke oni iel alkalkulos lin mem al la nombro de « tiuj malsaĝuloj », se li eĉ en la daŭro de unu minuto provos rilati serioze al tiu ĉi malsaĝaĵo. La homoj miras, « kiamaniere en nia praktika tempo povas aperi tiaj malsaĝaj fantaziuloj kaj kial oni ne metas ilin en la domojn por frenezuloj ».&lt;/span&gt;&lt;/p&gt;&lt;/SCRIBUSTEXT&gt;&#10;"/>
+    # Text="&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt;&lt;SCRIBUSTEXT &gt;&lt;defaultstyle /&gt;&lt;p &gt;&lt;style /&gt;&lt;span &gt;&lt;charstyle Features=&quot;inherit &quot; /&gt; Pri tiuj ĉi ideoj « estas modo » paroli ne alie, ol kun ironia kaj malestima rideto, tial tiel agas ankaŭ A kaj B kaj C, kaj ĉiu el ili timas enpensiĝi serioze eĉ unu minuton pri la mokata ideo, ĉar li « scias antaŭe », ke « ĝi krom malsaĝaĵo enhavas ja nenion », kaj li timas, ke oni iel alkalkulos lin mem al la nombro de « tiuj malsaĝuloj », se li eĉ en la daŭro de unu minuto provos rilati serioze al tiu ĉi malsaĝaĵo. La homoj miras, « kiamaniere en nia praktika tempo povas aperi tiaj malsaĝaj fantaziuloj kaj kial oni ne metas ilin en la domojn por frenezuloj ».&lt;/span&gt;&lt;/p&gt;&lt;/SCRIBUSTEXT&gt;&#10;"/>
 
-    #Text="
+    # Text="
     # <?xml version="1.0" encoding="UTF-8"?>
     # <SCRIBUSTEXT >
-        # <defaultstyle />
-        # <p >
-            # <style />
-            # <span >
-                # <charstyle Features="inherit " />
-                # Pri tiuj ĉi ideoj « estas modo » paroli ne alie, ol kun ironia kaj malestima rideto, tial tiel agas ankaŭ A kaj B kaj C, kaj ĉiu el ili timas enpensiĝi serioze eĉ unu minuton pri la mokata ideo, ĉar li « scias antaŭe », ke « ĝi krom malsaĝaĵo enhavas ja nenion », kaj li timas, ke oni iel alkalkulos lin mem al la nombro de « tiuj malsaĝuloj », se li eĉ en la daŭro de unu minuto provos rilati serioze al tiu ĉi malsaĝaĵo. La homoj miras, « kiamaniere en nia praktika tempo povas aperi tiaj malsaĝaj fantaziuloj kaj kial oni ne metas ilin en la domojn por frenezuloj ».
-            # </span>
-        # </p>
+    # <defaultstyle />
+    # <p >
+    # <style />
+    # <span >
+    # <charstyle Features="inherit " />
+    # Pri tiuj ĉi ideoj « estas modo » paroli ne alie, ol kun ironia kaj malestima rideto, tial tiel agas ankaŭ A kaj B kaj C, kaj ĉiu el ili timas enpensiĝi serioze eĉ unu minuton pri la mokata ideo, ĉar li « scias antaŭe », ke « ĝi krom malsaĝaĵo enhavas ja nenion », kaj li timas, ke oni iel alkalkulos lin mem al la nombro de « tiuj malsaĝuloj », se li eĉ en la daŭro de unu minuto provos rilati serioze al tiu ĉi malsaĝaĵo. La homoj miras, « kiamaniere en nia praktika tempo povas aperi tiaj malsaĝaj fantaziuloj kaj kial oni ne metas ilin en la domojn por frenezuloj ».
+    # </span>
+    # </p>
     # </SCRIBUSTEXT>
     # &#10;"/>
 
-    def __init__(self):
-        PyScribusElement.__init__(self)
+    empty_text = '&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt;' \
+    '&lt;SCRIBUSTEXT &gt;&lt;defaultstyle /&gt;' \
+    '&lt;p &gt;&lt;style /&gt;&lt;span &gt;' \
+    '&lt;charstyle Features=&quot;inherit &quot; /&gt;' \
+    '&lt;/span&gt;&lt;/p&gt;&lt;/SCRIBUSTEXT&gt;&#10;'
+
+    empty_pattern = '&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt;' \
+    '&lt;SCRIBUSTEXT &gt;&lt;defaultstyle /&gt;' \
+    '&lt;p &gt;&lt;style /&gt;&lt;span &gt;' \
+    '&lt;charstyle Features=&quot;inherit &quot; /&gt;' \
+    '&lt;/span&gt;&lt;/p&gt;{0}&lt;/SCRIBUSTEXT&gt;&#10;'
 
-    def fromxml(self, xml):
+    def __init__(self, parent_note=False):
+        PyScribusElement.__init__(self)
 
-        if xml == "Note":
-            content = xml.get("Text")
+        self.xml = None
 
-            if content is not None:
-                text = content
+        # We need to link NoteText to its note element (Note), because Note
+        # is linked with pyscribus.document.Document.
+        self.parent_note = parent_note
 
-                # &#10; = Line feed character
+    def fromxml(self, xml: ET.Element) -> bool:
 
-                for normalise in [
-                            [" &gt;&lt;","><"], ["&lt;", "<"], ["&gt;", ">"],
-                            ["&quot;", '"'], ["&#10;",""]
-                        ]:
-                    text = text.replace(normalise[0], normalise[1])
+        if xml.tag != "Note":
+            return False
 
-                xml_text = ET.fromstring(text)
+        content = xml.get("Text")
 
-                return True
-            else:
-                return False
-        else:
+        if content is None:
             return False
 
-    def toxml(self):
+        text = content
+
+        # &#10; = Line feed character
+
+        for normalise in [
+            ["&gt;&lt;", "><"],
+            [" &gt;", ">"],
+            ["&lt;", "<"],
+            ["&quot;", '"'],
+            ["&#10;", ""],
+        ]:
+            text = text.replace(normalise[0], normalise[1])
+
+        # Remove encoding declaration because lxml.etree.fromstring does not
+        # support it in unicode strings.
+        text = text.replace('<?xml version="1.0" encoding="UTF-8"?>', "")
+
+        print(text)
+
+        self.xml = ET.fromstring(text)
+
+        return True
+
+    def toxml(self) -> str:
         """
         Alias of toxmlstr()
         """
         return self.toxmlstr()
 
-    def toxmlstr(self):
-        xml_string = ""
+    def toxmlstr(self) -> str:
+        if self.xml is None:
+            return NoteText.empty_text
+
+        xml_string = copy.deepcopy(self.xml)
+        xml_string = ET.tostring(xml_string, encoding="utf8")
+
+        xml_string = xml_string.replace("><", "&gt;&lt;")
+        xml_string = xml_string.replace(">", "&gt;")
+        xml_string = xml_string.replace("<", "&lt;")
+        xml_string = xml_string.replace('"', "&quot;")
+        xml_string += "&#10;"
 
-        # TODO
+        print(xml_string)
 
         return xml_string
 
 
 class NoteFrame(PyScribusElement):
     """
     Note frame (NotesFrames/FOOTNOTEFRAME).
@@ -174,52 +219,53 @@
         # NOTE @MasterID
         # The page object with the story where note references are located
         self.story_frame_id = None
 
         # NOTE @NSname
         self.note_style = None
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
 
-        if xml == "FOOTNOTEFRAME":
-            note_style = xml.get("NSname")
-            own_frame = xml.get("myID")
-            story_frame = xml.get("MasterID")
+        if xml.tag != "FOOTNOTEFRAME":
+            return False
 
-            if note_style is not None:
-                self.note_style = note_style
+        note_style = xml.get("NSname")
+        own_frame = xml.get("myID")
+        story_frame = xml.get("MasterID")
 
-            if own_frame is not None:
-                self.own_frame_id = own_frame
+        if note_style is not None:
+            self.note_style = note_style
 
-            if story_frame is not None:
-                self.story_frame_id = story_frame
+        if own_frame is not None:
+            self.own_frame_id = own_frame
 
-            if story_frame is None or own_frame is None:
+        if story_frame is not None:
+            self.story_frame_id = story_frame
 
-                raise exceptions.InsaneSLAValue(
-                    "Note frame has no page object ID or\
-                     no parent page object ID."
-                )
+        if story_frame is None or own_frame is None:
 
-            return True
+            raise exceptions.InsaneSLAValue(
+                "Note frame has no page object ID or\
+                 no parent page object ID."
+            )
 
-        return False
+        return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("FOOTNOTEFRAME")
 
         if self.note_style is not None:
             xml.attrib["NSname"] = self.note_style
 
         if self.own_frame_id is not None:
             xml.attrib["myID"] = self.own_frame_id
 
         if self.story_frame_id is not None:
             xml.attrib["MasterID"] = self.story_frame_id
 
         return xml
 
-    def fromdefault(self):
+    def fromdefault(self) -> NoReturn:
         self.note_style = "Default"
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/pageobjects.py` & `pyscribus-backported-0.3/pyscribus/model/pageobjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,32 @@
 
 """
 PyScribus objects for… page objects manipulations.
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
 import copy
 import math
 
 import lxml
 import lxml.etree as ET
 
 import svg.path as svg
 
-import pyscribus.common.xml as xmlc
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
-import pyscribus.itemattribute as itemattribute
-import pyscribus.stories as stories
-import pyscribus.styles as pstyles
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.itemattribute as itemattribute
+import pyscribus.model.stories as stories
+import pyscribus.model.styles as pstyles
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 po_type_xml = {
     "image": 2,
@@ -54,16 +57,17 @@
     "symbol": 11,
     "group": 12,
     "table": 16,
 }
 
 # Classes ===============================================================#
 
-# NOTE PageObject est une classe obèse, mais il serait compliqué de gérer
-# autrement les évolutions du SLA dans PyScribus
+# NOTE PageObject is a giant class, but it would be complicated to handle
+# evolutions of SLA in PyScribus otherwise
+
 
 class PageObject(xmlc.PyScribusElement):
     """
     Page object in SLA (``/DOCUMENT/PAGEOBJECT``)
 
     You should rather use :class:`TableObject`, :class:`TextObject`,
     :class:`TextOnPathObject`, :class:`ImageObject`, :class:`LineObject`,
@@ -85,45 +89,43 @@
     """
 
     line_type_xml = {
         "solid": 1,
         "dashed": 2,
         "dotted": 3,
         "dash-dot": 4,
-        "dash-dot-dot": 5
+        "dash-dot-dot": 5,
     }
 
-    line_endcap_xml = {
-        "flat": "0",
-        "square": "16",
-        "round": "32"
-    }
+    line_endcap_xml = {"flat": "0", "square": "16", "round": "32"}
 
-    line_join_xml = {
-        "miter": "0",
-        "bevel": "64",
-        "round": "128"
-    }
+    line_join_xml = {"miter": "0", "bevel": "64", "round": "128"}
 
     image_scaling_type_xml = {
         "free": "0",
         "frame": "1",
     }
 
+    text_flow_xml = {
+        None: False,
+        "1": "shape",
+        "2": "rectangle",
+        "3": "outline"
+    }
+
     shape_type_xml = {
         "rectangle": "0",
         "ellipse": "1",
         "rounded-rectangle": "2",
         "free": "3",
     }
 
     def __init__(
-            self, ptype=False,
-            sla_parent=False, doc_parent=False,
-            **kwargs):
+        self, ptype=False, sla_parent=False, doc_parent=False, **kwargs
+    ):
 
         global po_type_xml
 
         super().__init__()
 
         # --- Page object parents ------------------------------------
 
@@ -139,14 +141,16 @@
         # --- Page object shape and boxes ----------------------------
 
         self.box = dimensions.DimBox()
         self.rotated_box = dimensions.DimBox()
         self.rotated = False
         self.shape = {"type": None, "edited": None}
 
+        self.opacity = dimensions.Dim(float(1), unit="pcdecim")
+
         # Image frame in image object defined there because Scribus
         # does it.
 
         self.image_box = dimensions.LocalDimBox()
         self.image_rotated_box = dimensions.DimBox()
 
         self.image_scale = {
@@ -180,21 +184,22 @@
 
         self.outline = {
             "type": "solid",
             "fill": "Black",
             "stroke": "Black",
             "thickness": dimensions.Dim(0),
             "join": None,
-            "endcap": None
+            "endcap": None,
         }
 
         # --- Page object paths --------------------------------------
 
         self.path = None
         self.copath = None
+        self.path_options = {}
 
         # --- --------------------------------------------------------
 
         if ptype and ptype in po_type_xml.keys():
             self.ptype = ptype
         else:
             self.ptype = None
@@ -203,404 +208,442 @@
 
         if kwargs:
             self._quick_setup(kwargs)
 
     def fromdefault(self):
         self.shape = {"type": "rectangle", "edited": False}
 
-    def fromxml(self, xml, arbitrary_tag=False):
+    def fromxml(self, xml: ET._Element, arbitrary_tag: bool = False):
         """
-        :type xml: lxml._Element
+        :type xml: lxml.etree._Element
         :param xml: XML source of the page object (PAGEOBJECT)
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
         valid_tag = False
 
         if arbitrary_tag:
             if xml.tag == arbitrary_tag:
                 valid_tag = True
         else:
             if xml.tag in ["PAGEOBJECT", "MASTEROBJECT"]:
                 valid_tag = True
 
-        if valid_tag:
-
-            if xml.tag == "MASTEROBJECT":
-                self.on_master_page = True
+        if not valid_tag:
+            return False
 
-            # Page object attributes
+        if xml.tag == "MASTEROBJECT":
+            self.on_master_page = True
 
-            xml_name = xml.get("ANNAME")
-            if xml_name is not None:
-                self.name = xml_name
-            else:
-                self.name = ""
+        # Page object attributes
 
-            own_id = xml.get("ItemID")
-            if own_id is None:
-                if self.name:
-                    raise exceptions.MissingSLAAttribute(
-                        "PAGEOBJECT '{}' must have @ItemID".format(self.name)
-                    )
-                else:
-                    raise exceptions.MissingSLAAttribute(
-                        "PAGEOBJECT must have @ItemID"
-                    )
-            else:
-                self.object_id = own_id
+        xml_name = xml.get("ANNAME")
+        if xml_name is not None:
+            self.name = xml_name
+        else:
+            self.name = ""
 
-            # --- Page object dimensions ---------------------------------
+        own_id = xml.get("ItemID")
+        if own_id is None:
+            if self.name:
+                raise exceptions.MissingSLAAttribute(
+                    "PAGEOBJECT '{}' must have @ItemID".format(self.name)
+                )
 
-            xpos = xml.get("XPOS")
-            ypos = xml.get("YPOS")
-            width = xml.get("WIDTH")
-            height = xml.get("HEIGHT")
-            rotation = xml.get("ROT")
+            raise exceptions.MissingSLAAttribute(
+                "PAGEOBJECT must have @ItemID"
+            )
 
-            valid_box = 0
+        self.object_id = own_id
 
-            for test in [xpos, ypos, width, height]:
-                if test is not None:
-                    valid_box += 1
+        # --- Page object dimensions ---------------------------------
 
-            if valid_box == 4:
+        xpos = xml.get("XPOS")
+        ypos = xml.get("YPOS")
+        width = xml.get("WIDTH")
+        height = xml.get("HEIGHT")
+        rotation = xml.get("ROT")
 
-                self.box.set_box(
-                    top_lx=xpos,
-                    top_ly=ypos,
-                    width=width,
-                    height=height
-                )
+        valid_box = 0
 
-                self.rotated_box = copy.deepcopy(self.box)
+        for test in [xpos, ypos, width, height]:
+            if test is not None:
+                valid_box += 1
 
-                if rotation is not None:
+        if valid_box == 4:
 
-                    try:
-                        rdegree = float(rotation)
+            self.box.set_box(
+                top_lx=xpos, top_ly=ypos, width=width, height=height
+            )
 
-                        if rdegree > 0:
-                            self.rotated_box.rotate(rdegree)
-                        else:
-                            self.rotated_box.rotation.value = 0
+            self.rotated_box = copy.deepcopy(self.box)
 
-                    except ValueError:
-                        pass
+            if rotation is not None:
 
-            # --- Undocumented gbox --------------------------------------
+                try:
+                    rdegree = float(rotation)
 
-            gxpos = xml.get("gXpos")
-            gypos = xml.get("gYpos")
-            gwidth = xml.get("gWidth")
-            gheight = xml.get("gHeight")
+                    if rdegree > 0:
+                        self.rotated_box.rotate(rdegree)
+                    else:
+                        self.rotated_box.rotation.value = 0
 
-            valid_box = 0
+                except ValueError:
+                    pass
 
-            for test in [gxpos, gypos, gwidth, gheight]:
-                if test is not None:
-                    valid_box += 1
+        # --- Undocumented gbox --------------------------------------
 
-            if valid_box == 4:
+        gxpos = xml.get("gXpos")
+        gypos = xml.get("gYpos")
+        gwidth = xml.get("gWidth")
+        gheight = xml.get("gHeight")
 
-                self.gbox.set_box(
-                    top_lx=gxpos,
-                    top_ly=gypos,
-                    width=gwidth,
-                    height=gheight
-                )
+        valid_box = 0
 
-            # ------------------------------------------------------------
+        for test in [gxpos, gypos, gwidth, gheight]:
+            if test is not None:
+                valid_box += 1
 
-            aspectratio = xml.get("RATIO")
-            if aspectratio is not None:
-                try:
-                    is_ratio = int(aspectratio)
-                except ValueError:
-                    is_ratio = 1
+        if valid_box == 4:
 
-                self.image_scale["ratio"] = bool(is_ratio)
+            self.gbox.set_box(
+                top_lx=gxpos, top_ly=gypos, width=gwidth, height=gheight
+            )
 
-            lscx = xml.get("LOCALSCX")
-            if lscx is not None:
-                self.image_scale["horizontal"].value = float(lscx)
+        # ------------------------------------------------------------
 
-            lscy = xml.get("LOCALSCY")
-            if lscy is not None:
-                self.image_scale["vertical"].value = float(lscy)
+        aspectratio = xml.get("RATIO")
+        if aspectratio is not None:
+            try:
+                is_ratio = int(aspectratio)
+            except ValueError:
+                is_ratio = 1
+
+            self.image_scale["ratio"] = bool(is_ratio)
+
+        lscx = xml.get("LOCALSCX")
+        if lscx is not None:
+            self.image_scale["horizontal"].value = float(lscx)
+
+        lscy = xml.get("LOCALSCY")
+        if lscy is not None:
+            self.image_scale["vertical"].value = float(lscy)
+
+        istype = xml.get("SCALETYPE")
+        if istype is not None:
+
+            for human, code in PageObject.image_scaling_type_xml.items():
+                if istype == code:
+                    self.image_scale["type"] = human
+                    break
 
-            istype = xml.get("SCALETYPE")
-            if istype is not None:
+        # --- Object path, copath and shape --------------------------
 
-                for human, code in PageObject.image_scaling_type_xml.items():
-                    if istype == code:
-                        self.image_scale["type"] = human
-                        break
+        editedshape : xml.get("CLIPEDIT")
+        if editedshape is not None:
+            self.shape["edited"] = xmlc.num_to_bool(editedshape)
+
+        shapetype = xml.get("FRTYPE")
+        if shapetype is not None:
+
+            for human, code in PageObject.shape_type_xml.items():
+                if shapetype == code:
+                    self.shape["type"] = human
+                    break
 
-            # --- Object path, copath and shape --------------------------
+        # NOTE FIXME Currently only working for rectangular shapes
 
-            editedshape = xml.get("CLIPEDIT")
-            if editedshape is not None:
-                self.shape["edited"] = xmlc.num_to_bool(editedshape)
-
-            shapetype = xml.get("FRTYPE")
-            if shapetype is not None:
-
-                for human,code in PageObject.shape_type_xml.items():
-                    if shapetype == code:
-                        self.shape["type"] = human
-                        break
+        for case in ["path", "copath"]:
 
-            # NOTE FIXME Currently only working for rectangular shapes
+            att = xml.get(case)
 
-            for case in ["path", "copath"]:
+            if att is None:
+                continue
 
-                att = xml.get(case)
-                if att is not None:
+            if self.ptype in [
+                "line",
+                "polyline",
+                "textonpath",
+                "polygon",
+            ]:
+                continue
 
-                    if self.ptype not in [
-                            "line", "polyline", "textonpath", "polygon"]:
-                        rectpath = RectPath()
+            rectpath = RectPath()
 
-                        success = rectpath.fromxml(att)
-                        if success:
+            success = rectpath.fromxml(att)
+            if success:
 
-                            if case == "path":
-                                self.path = rectpath
-                            else:
-                                self.copath = rectpath
+                if case == "path":
+                    self.path = rectpath
+                else:
+                    self.copath = rectpath
 
-            # --- Linked objects -----------------------------------------
+        # --- Linked objects -----------------------------------------
 
-            next_id = xml.get("NEXTITEM")
-            prev_id = xml.get("BACKITEM")
+        next_id = xml.get("NEXTITEM")
+        prev_id = xml.get("BACKITEM")
 
-            for link_id in zip(["next", "previous"], [next_id, prev_id]):
+        for link_id in zip(["next", "previous"], [next_id, prev_id]):
 
-                if link_id[1] is not None:
-                    if link_id[1] == "-1":
-                        self.linked[link_id[0]] = None
-                    else:
-                        self.linked[link_id[0]] = link_id[1]
+            if link_id[1] is not None:
+                if link_id[1] == "-1":
+                    self.linked[link_id[0]] = None
+                else:
+                    self.linked[link_id[0]] = link_id[1]
 
-            own_page = xml.get("OwnPage")
-            if own_page is not None:
-                try:
-                    if int(own_page):
-                        self.own_page = int(own_page)
-                    else:
-                        self.own_page = False
-                except ValueError:
-                    raise exceptions.InsaneSLAValue(
-                        "Invalid @OwnPage of PAGEOBJECT[@ItemID='{}']".format(
-                            self.object_id
-                        )
+        own_page = xml.get("OwnPage")
+        if own_page is not None:
+            try:
+                if int(own_page):
+                    self.own_page = int(own_page)
+                else:
+                    self.own_page = False
+            except ValueError:
+                raise exceptions.InsaneSLAValue(
+                    "Invalid @OwnPage of PAGEOBJECT[@ItemID='{}']".format(
+                        self.object_id
                     )
+                )
 
-            # --- Layer of the page object -------------------------------
+        # --- Layer of the page object -------------------------------
 
-            layer = xml.get("LAYER")
-            if layer is not None:
+        layer = xml.get("LAYER")
+        if layer is not None:
 
-                try:
-                    layer = int(layer)
+            try:
+                layer = int(layer)
 
-                    if self.doc_parent:
+                if self.doc_parent and self.doc_parent.layers:
 
-                        if self.doc_parent.layers:
+                    layer_found = False
 
-                            layer_found = False
+                    for doc_layer in self.doc_parent.layers:
+                        if layer != doc_layer.level:
+                            continue
 
-                            for doc_layer in self.doc_parent.layers:
+                        self.layer = layer
+                        layer_found = True
+                        break
 
-                                if layer == doc_layer.level:
-                                    self.layer = layer
-                                    layer_found = True
-                                    break
+                    if not layer_found:
+                        raise exceptions.UnknownLayer(layer)
 
-                            if not layer_found:
-                                raise exceptions.UnknownLayer(layer)
+            except TypeError:
+                raise exceptions.InsaneSLAValue(
+                    "PageObject @LAYER value should be an integer."
+                )
 
-                except TypeError:
-                    raise exceptions.InsaneSLAValue(
-                        "PageObject @LAYER value should be an integer."
-                    )
+        # --- Type specific attributes -------------------------------
+        # Moved to ImageObject
+        # Moved to TextObject
+        # Moved to LineObject
+        # Moved to TableObject
+
+        # --- Image in the image frame weirdly defined for all objects
+
+        img_xpos = xml.get("LOCALX")
+        img_ypos = xml.get("LOCALY")
+        img_rotation = xml.get("LOCALROT")
 
-            # --- Type specific attributes -------------------------------
-            # Moved to ImageObject
-            # Moved to TextObject
-            # Moved to LineObject
-            # Moved to TableObject
-
-            # --- Image in the image frame weirdly defined for all objects
-
-            img_xpos = xml.get("LOCALX")
-            img_ypos = xml.get("LOCALY")
-            img_rotation = xml.get("LOCALROT")
-
-            valid_box = 0
-
-            for test in [img_xpos, img_ypos]:
-                if test is not None:
-                    try:
-                        test = float(test)
-                        valid_box += 1
-                    except ValueError:
-                        continue
+        valid_box = 0
 
-            # The DimBox object needs a width and height but we don’t have
-            # that for the included image frame. So we take the dimensions
-            # of the parent object and resize them with image scale attributes
+        for test in [img_xpos, img_ypos]:
+            if test is not None:
+                try:
+                    test = float(test)
+                    valid_box += 1
+                except ValueError:
+                    continue
 
-            # WARNING But all of this is based on a SCALETYPE being free, not frame
+        # The DimBox object needs a width and height but we don’t have
+        # that for the included image frame. So we take the dimensions
+        # of the parent object and resize them with image scale attributes
 
-            if valid_box == 2:
+        # WARNING But all of this is based on a SCALETYPE being free, not
+        # frame.
 
-                if self.image_scale["horizontal"]:
-                    img_width = self.box.dims["width"].value * float(
-                        self.image_scale["horizontal"]
-                    )
+        if valid_box == 2:
 
-                if self.image_scale["vertical"]:
-                    img_height = self.box.dims["height"].value * float(
-                        self.image_scale["vertical"]
-                    )
+            if self.image_scale["horizontal"]:
+                img_width = self.box.dims["width"].value * float(
+                    self.image_scale["horizontal"]
+                )
 
-                self.image_box.set_box(
-                    top_lx=img_xpos,
-                    top_ly=img_ypos,
-                    width=img_width,
-                    height=img_height
+            if self.image_scale["vertical"]:
+                img_height = self.box.dims["height"].value * float(
+                    self.image_scale["vertical"]
                 )
 
-                self.image_rotated_box = copy.deepcopy(self.image_box)
+            self.image_box.set_box(
+                top_lx=img_xpos,
+                top_ly=img_ypos,
+                width=img_width,
+                height=img_height,
+            )
 
-                if img_rotation is not None:
+            self.image_rotated_box = copy.deepcopy(self.image_box)
 
-                    try:
-                        rdegree = float(img_rotation)
+            if img_rotation is not None:
 
-                        if rdegree > 0:
-                            self.image_rotated_box.rotate(rdegree)
-                        else:
-                            self.image_rotated_box.rotation.value = 0
+                try:
+                    rdegree = float(img_rotation)
 
-                    except ValueError:
-                        pass
+                    if rdegree > 0:
+                        self.image_rotated_box.rotate(rdegree)
+                    else:
+                        self.image_rotated_box.rotation.value = 0
 
-            visibleimage = xml.get("PICART")
-            if visibleimage is not None:
-                self.image_box.visible = xmlc.num_to_bool(visibleimage)
+                except ValueError:
+                    pass
 
-            # --- Page object outline ------------------------------------
+        visibleimage = xml.get("PICART")
+        if visibleimage is not None:
+            self.image_box.visible = xmlc.num_to_bool(visibleimage)
 
-            line_type = xml.get("PLINEART")
-            if line_type is not None:
-                for human, code in PageObject.line_type_xml.items():
-                    if line_type == code:
-                        self.outline["type"] = human
-                        break
+        # --- Page object outline ------------------------------------
 
-            fill = xml.get("PCOLOR")
-            if fill is not None:
-                self.outline["fill"] = fill
-            else:
-                self.outline["fill"] = None
+        line_type = xml.get("PLINEART")
+        if line_type is not None:
+            for human, code in PageObject.line_type_xml.items():
+                if line_type == code:
+                    self.outline["type"] = human
+                    break
 
-            stroke = xml.get("PCOLOR2")
-            if stroke is not None:
-                self.outline["stroke"] = stroke
-            else:
-                self.outline["stroke"] = None
+        fill = xml.get("PCOLOR")
+        if fill is not None:
+            self.outline["fill"] = fill
+        else:
+            self.outline["fill"] = None
 
-            thickness = xml.get("PWIDTH")
-            if thickness is not None:
-                self.outline["thickness"].value = float(thickness)
+        stroke = xml.get("PCOLOR2")
+        if stroke is not None:
+            self.outline["stroke"] = stroke
+        else:
+            self.outline["stroke"] = None
 
-            # Outline end/join for polyline and polygon
+        thickness = xml.get("PWIDTH")
+        if thickness is not None:
+            self.outline["thickness"].value = float(thickness)
 
-            if self.ptype in ["polyline", "polygon"]:
+        # Outline end/join for polyline and polygon
 
-                # TODO FIXME Undocumented in polyline, polygon
-                fillrule = xml.get("fillRule")
-                if fillrule is not None:
-                    pass
+        if self.ptype in ["polyline", "polygon"]:
 
-                line_end = xml.get("PLINEEND")
-                if line_end is not None:
-                    for human, code in PageObject.line_endcap_xml.items():
-                        if line_end == code:
-                            self.outline["endcap"] = human
-                            break
+            # TODO FIXME Undocumented in polyline, polygon
+            fillrule = xml.get("fillRule")
+            if fillrule is not None:
+                pass
 
-                line_join = xml.get("PLINEJOIN")
-                if line_join is not None:
-                    for human, code in PageObject.line_join_xml.items():
-                        if line_join == code:
-                            self.outline["join"] = human
-                            break
+            line_end = xml.get("PLINEEND")
+            if line_end is not None:
+                for human, code in PageObject.line_endcap_xml.items():
+                    if line_end == code:
+                        self.outline["endcap"] = human
+                        break
 
-            # --- ICC profiles -------------------------------------------
+            line_join = xml.get("PLINEJOIN")
+            if line_join is not None:
+                for human, code in PageObject.line_join_xml.items():
+                    if line_join == code:
+                        self.outline["join"] = human
+                        break
 
-            if self.ptype in ["image", "render"]:
+        # --- ICC profiles -------------------------------------------
 
-                embedded = xml.get("EMBEDDED")
-                if embedded is not None:
-                    self.embedded_icc["use"] = xmlc.num_to_bool(embedded)
+        if self.ptype in ["image", "render"]:
 
-                img_embedded_icc = xml.get("EPROF")
-                if img_embedded_icc is not None:
-                    self.embedded_icc["profile"] = img_embedded_icc
+            embedded = xml.get("EMBEDDED")
+            if embedded is not None:
+                self.embedded_icc["use"] = xmlc.num_to_bool(embedded)
 
-            # --- Symbol attributes --------------------------------------
+            img_embedded_icc = xml.get("EPROF")
+            if img_embedded_icc is not None:
+                self.embedded_icc["profile"] = img_embedded_icc
 
-            if self.ptype == "symbol":
+        # --- Symbol attributes --------------------------------------
 
-                pattern = xml.get("pattern")
-                if pattern is not None:
-                    self.pattern = pattern
+        if self.ptype == "symbol":
 
-            # --- Page objects specific children -------------------------
-            # Moved in TableObject
-            # Moved in TableObject
-            # Moved in TableObject
-            # NOTE No childs in image object
+            pattern = xml.get("pattern")
+            if pattern is not None:
+                self.pattern = pattern
 
-            #--- FIXME This records undocumented attributes --------------
+        # --- Flow ---------------------------------------------------
 
-            self.undocumented = xmlc.all_undocumented_to_python(xml)
+        if self.ptype in ["polyline", "polygon", "text"]:
+            # No text flow applied = no attribute TEXTFLOWMODE
+            text_flow_mode = xml.get("TEXTFLOWMODE")
 
-            # ------------------------------------------------------------
+            try:
+                self.text_flow = PageObject.text_flow_xml[text_flow_mode]
+            except KeyError:
+                self.text_flow = PageObject.text_flow_xml[None]
+
+        # --- Text on path : show path -------------------------------
+
+        if self.ptype in ["textonpath", "text"]:
+            self.path_options["text_on_path"] = {
+                "show": False,
+                "offset": dimensions.Dim(0)
+            }
+
+            showtextpath = xml.get("PLTSHOW")
+            if showtextpath is not None:
+                self.path_options["text_on_path"]["show"] = xmlc.num_to_bool(showtextpath)
+
+            # BASEOF : Offset for the text from its path for text on a path
+            textpathoffset = xml.get("BASEOF")
+            if textpathoffset is not None:
+                self.path_options["text_on_path"]["offset"].value = float(textpathoffset)
+
+        # --- Opacity of the object ----------------------------------
+
+        opacity = xml.get("TransValue")
+        if opacity is not None:
+            self.opacity.value = float(opacity)
+
+        # --- Page objects specific children -------------------------
+        # Moved in TableObject
+        # Moved in TableObject
+        # Moved in TableObject
+        # NOTE No childs in image object
 
-            return True
-        else:
-            return False
+        # FIXME This records undocumented attributes -----------------
+
+        self.undocumented = xmlc.all_undocumented_to_python(xml)
+
+        # ------------------------------------------------------------
+
+        return True
 
-    def toxml(self, arbitrary_tag=False):
+    def toxml(self, arbitrary_tag: bool = False):
         """
-        :rtype: lxml._Element
-        :returns: Page object as lxml._Element
+        :rtype: lxml.etree._Element
+        :returns: Page object as lxml.etree._Element
         """
 
         global po_type_xml
 
         if arbitrary_tag:
             xml = ET.Element(arbitrary_tag)
         else:
-            if self.on_master_page:
-                xml = ET.Element("MASTEROBJECT")
-            else:
-                xml = ET.Element("PAGEOBJECT")
+            xml = ET.Element(
+                {True: "MASTEROBJECT", False: "PAGEOBJECT"}[
+                    self.on_master_page
+                ]
+            )
 
         xml.attrib["XPOS"] = self.box.coords["top-left"][0].toxmlstr()
         xml.attrib["YPOS"] = self.box.coords["top-left"][1].toxmlstr()
         xml.attrib["WIDTH"] = self.box.dims["width"].toxmlstr()
         xml.attrib["HEIGHT"] = self.box.dims["height"].toxmlstr()
-        xml.attrib["ROT"] = self.rotated_box.rotation.toxmlstr(True)
+
+        if self.rotated_box.rotation.value == 0:
+            xml.attrib["ROT"] = self.rotated_box.rotation.toxmlstr(True)
 
         xml.attrib["ItemID"] = self.object_id
 
         # NOTE OwnPage doit exister quitte à juste être faux (= 0)
         # sinon plantage de Scribus.
         # wiki.scribus.net/canvas/
         # (FR)_Introdution_au_Format_de_fichier_SLA_pour_Scribus_1.4
@@ -608,53 +651,64 @@
         xml.attrib["OwnPage"] = xmlc.bool_or_else_to_num(self.own_page)
 
         # NOTE ANNAME is optional
         if self.name is not None:
             if self.name:
                 xml.attrib["ANNAME"] = self.name
 
-        xml.attrib["LOCALSCX"] = str(self.image_scale["horizontal"])
-        xml.attrib["LOCALSCY"] = str(self.image_scale["vertical"])
+        xml.attrib["LOCALSCX"] = self.image_scale["horizontal"].toxmlstr(True)
+        xml.attrib["LOCALSCY"] = self.image_scale["vertical"].toxmlstr(True)
 
         # Image frame of an image object
 
-        xml.attrib["LOCALX"] = self.image_box.coords["top-left"][0].toxmlstr()
-        xml.attrib["LOCALY"] = self.image_box.coords["top-left"][1].toxmlstr()
+        xml.attrib["LOCALX"] = self.image_box.coords["top-left"][0].toxmlstr(True)
+        xml.attrib["LOCALY"] = self.image_box.coords["top-left"][1].toxmlstr(True)
         xml.attrib["LOCALROT"] = self.image_rotated_box.rotation.toxmlstr(True)
 
         xml.attrib["PICART"] = xmlc.bool_to_num(self.image_box.visible)
 
-        # Undocumented gbox
+        # Undocumented gbox ---------------------------------------------------
 
         xml.attrib["gXpos"] = self.gbox.coords["top-left"][0].toxmlstr()
         xml.attrib["gYpos"] = self.gbox.coords["top-left"][1].toxmlstr()
-        xml.attrib["gWidth"] = self.gbox.dims["width"].toxmlstr()
-        xml.attrib["gHeight"] = self.gbox.dims["height"].toxmlstr()
+        xml.attrib["gWidth"] = self.gbox.dims["width"].toxmlstr(True)
+        xml.attrib["gHeight"] = self.gbox.dims["height"].toxmlstr(True)
+
+        # ---------------------------------------------------------------------
 
         # Page object type
         xml.attrib["PTYPE"] = str(po_type_xml[self.ptype])
 
         # Layer
         xml.attrib["LAYER"] = str(self.layer)
 
+        # --- Opacity of the object ----------------------------------
+
+        if self.opacity.value < float(1):
+            xml.attrib["TransValue"] = self.opacity.toxmlstr(True)
+
         # ------------------------------------------------------------
 
         if self.shape["type"] is None:
             # If the shape type is not defined, we assume the frame has
             # a rectangular shape, as it is the most common
             xml.attrib["FRTYPE"] = PageObject.shape_type_xml["rectangle"]
         else:
-            xml.attrib["FRTYPE"] = PageObject.shape_type_xml[self.shape["type"]]
+            xml.attrib["FRTYPE"] = PageObject.shape_type_xml[
+                self.shape["type"]
+            ]
 
         if self.shape["edited"] is None:
             xml.attrib["CLIPEDIT"] = "0"
         else:
             xml.attrib["CLIPEDIT"] = xmlc.bool_to_num(self.shape["edited"])
 
-        xml.attrib["SCALETYPE"] = PageObject.image_scaling_type_xml[self.image_scale["type"]]
+        xml.attrib["SCALETYPE"] = PageObject.image_scaling_type_xml[
+            self.image_scale["type"]
+        ]
         xml.attrib["RATIO"] = xmlc.bool_to_num(self.image_scale["ratio"])
 
         if self.path is None:
 
             if self.ptype not in ["line", "polyline", "textonpath"]:
                 # If the path for @path doesn't exist because this is a
                 # object made from scratch and not through SLA parsing,
@@ -679,22 +733,30 @@
         # Outline ----------------------------------------------------
 
         xml.attrib["PLINEART"] = str(
             PageObject.line_type_xml[self.outline["type"]]
         )
 
         if self.outline["join"] is not None:
-            xml.attrib["PLINEJOIN"] = PageObject.line_join_xml[self.outline["join"]]
+            xml.attrib["PLINEJOIN"] = PageObject.line_join_xml[
+                self.outline["join"]
+            ]
 
         if self.outline["endcap"] is not None:
-            xml.attrib["PLINEEND"] = PageObject.line_endcap_xml[self.outline["endcap"]]
+            xml.attrib["PLINEEND"] = PageObject.line_endcap_xml[
+                self.outline["endcap"]
+            ]
+
+        if self.outline["fill"] is not None:
+            xml.attrib["PCOLOR"] = self.outline["fill"]
+
+        if self.outline["stroke"] is not None:
+            xml.attrib["PCOLOR2"] = self.outline["stroke"]
 
-        xml.attrib["PCOLOR"] = self.outline["fill"]
-        xml.attrib["PCOLOR2"] = self.outline["stroke"]
-        xml.attrib["PWIDTH"] = self.outline["thickness"].toxmlstr()
+        xml.attrib["PWIDTH"] = self.outline["thickness"].toxmlstr(True)
 
         # ------------------------------------------------------------
 
         if self.ptype in ["image", "render"]:
             xml.attrib["EMBEDDED"] = xmlc.bool_to_num(self.embedded_icc["use"])
 
             if self.embedded_icc["profile"]:
@@ -714,38 +776,63 @@
         #      (if the item doesn't exists, Scribus crashes), or -1
 
         if self.linked["previous"] is None:
             xml.attrib["BACKITEM"] = "-1"
         else:
             xml.attrib["BACKITEM"] = self.linked["previous"]
 
-        #--- FIXME This exports undocumented attributes -------
+        # --- Flow ---------------------------------------------------
 
-        if self.ptype not in ["table", "group", "text"]:
+        if self.ptype in ["polyline", "polygon", "text"]:
+
+            if self.text_flow:
+                # No text flow applied = no attribute TEXTFLOWMODE
+
+                for code, human in PageObject.text_flow_xml.items():
+                    if self.text_flow != human:
+                        continue
+                    xml.attrib["TEXTFLOWMODE"] = str(code)
+
+        # --- Text on path : show path -------------------------------
+
+        if self.ptype in ["textonpath", "text"]:
+            xml.attrib["PLTSHOW"] = xmlc.bool_to_num(
+                self.path_options["text_on_path"]["show"]
+            )
+
+            xml.attrib["BASEOF"] = self.path_options["text_on_path"]["offset"].toxmlstr(True)
+
+        # FIXME This exports undocumented attributes ----------
+
+        if self.ptype not in ["table", "group", "text", "image"]:
 
             try:
                 xml, undoc_attribs = xmlc.all_undocumented_to_xml(
-                    xml, self.undocumented, True,
+                    xml,
+                    self.undocumented,
+                    True,
                     self.ptype + " '{}'".format(self.name.strip()),
                     # FIXME This disable debug for path, copath attributes
                     # ["path", "copath"]
-                    logger=logs.getLogger()
+                    logger=logs.getLogger(),
                 )
 
             except AttributeError:
                 # NOTE If fromxml was not used
                 pass
 
         return xml
 
     def has_attribute(self, name):
         for attribute in self.attributes:
             if attribute.name == name:
                 return True
 
+        return False
+
     def templatable(self):
         is_templatable = False
 
         if self.ptype != "text":
             attribute_pattern = self.sla_parent.templating["attribute-pattern"]
 
             for attribute in self.attributes:
@@ -798,16 +885,27 @@
 
                 if setting_name == "height":
                     self.box.dims["height"].value = float(setting_value)
 
                 if setting_name == "layer":
                     self.layer = setting_value
 
+                if setting_name == "outline_fill":
+                    self.outline["fill"] = setting_value
+
+                if setting_name == "outline_stroke":
+                    self.outline["stroke"] = setting_value
+
+                if setting_name == "object_id":
+                    self.object_id = setting_value
+
+
 # Inherited from PageObject =============================================#
 
+
 class TableObject(PageObject):
     """
     Table frame.
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
@@ -819,70 +917,73 @@
     :ivar integer rows: Number of rows
     :ivar integer columns: Number of columns
     """
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "table", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
         self.rows = 0
         self.columns = 0
 
         self.cells = []
 
         self.style = None
+        self.data_style = None
 
         self.fill = {"color": "None", "shade": None}
 
         self.borders = {
-            "left": None, "right": None,
-            "top": None, "bottom": None
+            "left": None,
+            "right": None,
+            "top": None,
+            "bottom": None,
         }
 
-        #--- Then, quick setup -------------------------------------------
+        # Then, quick setup ----------------------------------------------
 
         PageObject._quick_setup(self, kwargs)
 
-    #--- Cells update methods -----------------------------------------------
+    # Cells update methods --------------------------------------------------
 
     def _update_rowcols_count(self):
         """Update the count of rows and columns."""
 
         self.rows = max([cell.row for cell in self.cells]) + 1
         self.columns = max([cell.column for cell in self.cells]) + 1
 
     def _update_cells_geometry(self, cols, rows):
         """
         Set each cell box according its row's position & height and its
         column's position and width.
         """
 
-        colsdict,rowsdict = {},{}
+        colsdict, rowsdict = {}, {}
 
         for col in cols:
-            col_index,col_x,col_width = col
+            col_index, col_x, col_width = col
             colsdict[col_index] = {"position": col_x, "width": col_width}
 
         for row in rows:
-            row_index,row_y,row_height = row
+            row_index, row_y, row_height = row
             rowsdict[row_index] = {"position": row_y, "height": row_height}
 
         for cell in self.cells:
             row = rowsdict[cell.row]
             column = colsdict[cell.column]
 
             cell.box.set_box(
                 top_lx=column["position"],
                 top_ly=row["position"],
                 width=column["width"],
-                height=row["height"]
+                height=row["height"],
             )
 
-    #--- --------------------------------------------------------------------
+    # -----------------------------------------------------------------------
 
     def _append_row_at_end(self, height=False):
         """
         Append a row at the end of the table.
 
         :type height: boolean,float
         :param height: Height of the new rows
@@ -899,22 +1000,24 @@
         for cell in self.cells:
 
             if cell.column not in columns:
                 columns[cell.column] = {
                     # "x": float(cell.box.coords["top-left"][0]),
                     "x": float(cell.box.getx("top-left")),
                     "width": float(cell.box.dims["width"]),
-                    "borders": cell.borders, "padding": cell.padding,
-                    "fill": cell.fill, "align": cell.align,
-                    "style": cell.style
+                    "borders": cell.borders,
+                    "padding": cell.padding,
+                    "fill": cell.fill,
+                    "align": cell.align,
+                    "style": cell.style,
                 }
 
         # --- Getting the last row y and height ----------------------
 
-        last_y,last_height = None,None
+        last_y, last_height = None, None
 
         for cell in self.cells:
 
             if cell.row == (self.rows - 1):
                 # last_y = float(cell.box.coords["top-left"][1])
                 last_y = float(cell.box.gety("top-left"))
                 last_height = float(cell.box.dims["height"])
@@ -936,44 +1039,50 @@
 
             # --- Adding the cell in each column of the new row ------
 
             new_cells = []
 
             for column_index, datas in columns.items():
                 cell = TableCell(
-                    self, default=True,
-                    column = column_index, row = self.rows,
-                    posx=datas["x"], posy=new_y,
-                    width=datas["width"], height=new_height,
+                    self,
+                    default=True,
+                    column=column_index,
+                    row=self.rows,
+                    posx=datas["x"],
+                    posy=new_y,
+                    width=datas["width"],
+                    height=new_height,
                     fillcolor=datas["fill"]["color"],
                     fillshade=datas["fill"]["shade"],
-                    padding=datas["padding"], borders=datas["borders"],
-                    alignment=datas["align"], style=datas["style"],
+                    padding=datas["padding"],
+                    borders=datas["borders"],
+                    alignment=datas["align"],
+                    style=datas["style"],
                 )
 
                 self.cells.append(cell)
                 new_cells.append(self.cells[-1])
 
             self._update_rowcols_count()
 
             return new_cells
 
         # ------------------------------------------------------------
 
         return False
 
-    def append_row(self, height=False, position=-1):
+    def append_row(self, height=False, position: int = -1):
         """
         Append a row at the end of the table.
 
         :type height: boolean,float
         :param height: Height of the new row
-        :param position: The row is appended after the
-            position-n row. If -1, the row is appended
-            after the last row of the table.
+        :type position: integer
+        :param position: The row is appended after the position-n row.
+            If -1, the row is appended after the last row of the table.
         :rtype: list
         :returns: List of new cells
         """
 
         self._update_rowcols_count()
 
         # --- If position is -1 = end of the table -------------------
@@ -989,30 +1098,30 @@
 
             columns = {}
 
             for cell in self.cells:
 
                 if cell.column not in columns:
                     columns[cell.column] = {
-                        # "x": float(cell.box.coords["top-left"][0]),
                         "x": float(cell.box.getx("top-left")),
                         "width": float(cell.box.dims["width"]),
-                        "borders": cell.borders, "padding": cell.padding,
-                        "fill": cell.fill, "align": cell.align,
-                        "style": cell.style
+                        "borders": cell.borders,
+                        "padding": cell.padding,
+                        "fill": cell.fill,
+                        "align": cell.align,
+                        "style": cell.style,
                     }
 
             # --- Getting the y and height of the row matching position --
 
-            index_row_y,index_row_height = None,None
+            index_row_y, index_row_height = None, None
 
             for cell in self.cells:
 
                 if cell.row == position - 1:
-                    # index_row_y = float(cell.box.coords["top-left"][1])
                     index_row_y = float(cell.box.gety("top-left"))
                     index_row_height = float(cell.box.dims["height"])
 
                     break
 
             # --- Adding the new row -------------------------------------
 
@@ -1049,22 +1158,28 @@
 
                 # --- Adding the cell in each column of the new row ------
 
                 new_cells = []
 
                 for column_index, datas in columns.items():
                     cell = TableCell(
-                        self, default=True,
-                        column = column_index, row = position,
-                        posx=datas["x"], posy=new_y,
-                        width=datas["width"], height=new_height,
+                        self,
+                        default=True,
+                        column=column_index,
+                        row=position,
+                        posx=datas["x"],
+                        posy=new_y,
+                        width=datas["width"],
+                        height=new_height,
                         fillcolor=datas["fill"]["color"],
                         fillshade=datas["fill"]["shade"],
-                        padding=datas["padding"], borders=datas["borders"],
-                        alignment=datas["align"], style=datas["style"],
+                        padding=datas["padding"],
+                        borders=datas["borders"],
+                        alignment=datas["align"],
+                        style=datas["style"],
                     )
 
                     self.cells.append(cell)
                     new_cells.append(self.cells[-1])
 
                 # --------------------------------------------------------
 
@@ -1074,32 +1189,30 @@
 
             # ------------------------------------------------------------
 
             return False
 
         return False
 
-    def append_rows(self, number=1, height=False, position=-1):
+    def append_rows(self, number: int = 1, height=False, position: int = -1):
         """
         Append rows at the end of the table.
 
         :type number: integer
         :param number: Number of colums to append
         :type height: boolean,float
         :param height: Height of the new rows
         :type position: integer
-        :param position: The rows are appended
-            after the position-n row. If -1, the
-            rows are appended after the last
-            row of the table.
+        :param position: The rows are appended after the position-n row.
+            If -1, the rows are appended after the last row of the table.
         :rtype: list
         :returns: List of new cells by rows
         """
 
-        new_cells,added = [],0
+        new_cells, added = [], 0
 
         if position == -1:
             at_end = True
         else:
             at_end = False
             row_index = position
 
@@ -1111,18 +1224,15 @@
                 cells = self.append_row(height, row_index)
                 row_index += 1
 
             if cells:
                 added += 1
                 new_cells.append(cells)
 
-        if added == number:
-            return True
-        else:
-            return False
+        return added == number
 
     def append_column(self, width=False):
         """
         Append a column at the end of the table.
 
         :type width: boolean,float
         :param width: Width of the new column
@@ -1139,27 +1249,28 @@
         for cell in self.cells:
 
             if cell.row not in rows:
                 rows[cell.row] = {
                     # "y": float(cell.box.coords["top-left"][1]),
                     "y": float(cell.box.gety("top-left")),
                     "height": float(cell.box.dims["height"]),
-                    "borders": cell.borders, "padding": cell.padding,
-                    "fill": cell.fill, "align": cell.align,
-                    "style": cell.style
+                    "borders": cell.borders,
+                    "padding": cell.padding,
+                    "fill": cell.fill,
+                    "align": cell.align,
+                    "style": cell.style,
                 }
 
         # --- Getting the last column x and width --------------------
 
-        last_x,last_width = None,None
+        last_x, last_width = None, None
 
         for cell in self.cells:
 
             if cell.column == (self.columns - 1):
-                # last_x = float(cell.box.coords["top-left"][0])
                 last_x = float(cell.box.getx("top-left"))
                 last_width = float(cell.box.dims["width"])
 
                 break
 
         # --- Adding the new column ----------------------------------
 
@@ -1179,275 +1290,291 @@
 
             # --- Adding the cell in each row of the new column ------
 
             new_cells = []
 
             for row_index, datas in rows.items():
                 cell = TableCell(
-                    self, default=True,
-                    column = self.columns, row = row_index,
-                    posx=new_x, posy=datas["y"],
-                    width=new_width, height=datas["height"],
+                    self,
+                    default=True,
+                    column=self.columns,
+                    row=row_index,
+                    posx=new_x,
+                    posy=datas["y"],
+                    width=new_width,
+                    height=datas["height"],
                     fillcolor=datas["fill"]["color"],
                     fillshade=datas["fill"]["shade"],
-                    padding=datas["padding"], borders=datas["borders"],
-                    alignment=datas["align"], style=datas["style"],
+                    padding=datas["padding"],
+                    borders=datas["borders"],
+                    alignment=datas["align"],
+                    style=datas["style"],
                 )
 
                 self.cells.append(cell)
                 new_cells.append(self.cells[-1])
 
             self._update_rowcols_count()
 
             return new_cells
 
         # ------------------------------------------------------------
 
         return False
 
-    def append_columns(self, number=1, width=False):
+    def append_columns(self, number: int = 1, width=False):
         """
         Append columns at the end of the table.
 
         :type number: integer
         :param number: Number of colums to append
         :type width: boolean,float
         :param width: Width of the new columns
         :rtype: list
         :returns: List of new cells by columns
         """
 
-        new_cells,added = [],0
+        new_cells, added = [], 0
 
         for add in range(number):
             cells = self.append_column(width)
 
             if cells:
                 added += 1
                 new_cells.append(cells)
 
-        if added == number:
-            return True
-        else:
-            return False
+        return added == number
 
-    #--- PyScribus standard methods -----------------------------------------
+    # PyScribus standard methods --------------------------------------------
 
     def toxml(self):
         """
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         :returns: Table object as LXML element
         """
 
         xml = PageObject.toxml(self)
 
-        if isinstance(xml, ET._Element):
-            # --- Attributes ---------------------------------------------
+        if not isinstance(xml, ET._Element):
+            return False
 
-            self._update_rowcols_count()
+        # --- Attributes ---------------------------------------------
 
-            # Number of rows and columns ----------------------------
+        if self.style is None:
+            xml.attrib["TableStyle"] = ""
+        else:
+            xml.attrib["TableStyle"] = self.style
 
-            if self.rows > 0:
-                xml.attrib["Rows"] = str(self.rows)
-            else:
-                raise ValueError("Table object has zero rows.")
+        self._update_rowcols_count()
 
-            if self.columns > 0:
-                xml.attrib["Columns"] = str(self.columns)
-            else:
-                raise ValueError("Table object has zero columns.")
+        # Number of rows and columns ----------------------------
 
-            # Columns and rows datas --------------------------------
+        if self.rows > 0:
+            xml.attrib["Rows"] = str(self.rows)
+        else:
+            raise ValueError("Table object has zero rows.")
 
-            rowsh,colsw = {},{}
-            rowsp,colsp = {},{}
+        if self.columns > 0:
+            xml.attrib["Columns"] = str(self.columns)
+        else:
+            raise ValueError("Table object has zero columns.")
 
-            for cell in self.cells:
+        # Columns and rows datas --------------------------------
 
-                if cell.row not in rowsh:
-                    rowsh[cell.row] = cell.box.dims["height"].toxmlstr(True)
+        rowsh, colsw = {}, {}
+        rowsp, colsp = {}, {}
 
-                if cell.row not in rowsp:
-                    rowsp[cell.row] = cell.box.coords["top-left"][1].toxmlstr(True)
+        for cell in self.cells:
 
-                if cell.column not in colsw:
-                    colsw[cell.column] = cell.box.dims["width"].toxmlstr(True)
+            if cell.row not in rowsh:
+                rowsh[cell.row] = cell.box.dims["height"].toxmlstr(True)
 
-                if cell.column not in colsp:
-                    colsp[cell.column] = cell.box.coords["top-left"][0].toxmlstr(True)
+            if cell.row not in rowsp:
+                rowsp[cell.row] = cell.box.coords["top-left"][1].toxmlstr(True)
 
-            for case in [
-                    ["RowPositions", rowsp], ["RowHeights", rowsh],
-                    ["ColumnPositions", colsp], ["ColumnWidths", colsw]]:
+            if cell.column not in colsw:
+                colsw[cell.column] = cell.box.dims["width"].toxmlstr(True)
 
-                xml.attrib[case[0]] = " ".join(
-                    case[1][n] for n in sorted(case[1].keys())
+            if cell.column not in colsp:
+                colsp[cell.column] = cell.box.coords["top-left"][0].toxmlstr(
+                    True
                 )
 
-            #--- FIXME This exports undocumented attributes --------------
+        for case in [
+            ["RowPositions", rowsp],
+            ["RowHeights", rowsh],
+            ["ColumnPositions", colsp],
+            ["ColumnWidths", colsw],
+        ]:
 
-            try:
-                xml, undoc_attribs = xmlc.all_undocumented_to_xml(
-                    xml, self.undocumented, True,
-                    self.ptype + " '{}'".format(self.name.strip()),
-                    logger=logs.getLogger()
-                )
+            xml.attrib[case[0]] = " ".join(
+                case[1][n] for n in sorted(case[1].keys())
+            )
 
-            except AttributeError:
-                # NOTE If fromxml was not used
-                pass
+        # FIXME This exports undocumented attributes -----------------
 
-            # --- Children -----------------------------------------------
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
 
-            # TableData attributes
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
 
-            tabdata = ET.Element("TableData")
+        # --- Children -----------------------------------------------
 
-            if self.style is None:
-                tabdata.attrib["Style"] = ""
-            else:
-                tabdata.attrib["Style"] = self.style
+        # TableData attributes
 
-            tabdata.attrib["FillColor"] = self.fill["color"]
+        tabdata = ET.Element("TableData")
 
-            if self.fill["shade"] is None:
-                tabdata.attrib["FillShade"] = "100"
-            else:
-                tabdata.attrib["FillShade"] = self.fill["shade"].toxmlstr(True)
+        if self.data_style is None:
+            tabdata.attrib["Style"] = ""
+        else:
+            tabdata.attrib["Style"] = self.data_style
 
-            # TableData children
+        tabdata.attrib["FillColor"] = self.fill["color"]
 
-            for side in ["left", "right", "top", "bottom"]:
+        if self.fill["shade"] is None:
+            tabdata.attrib["FillShade"] = "100"
+        else:
+            tabdata.attrib["FillShade"] = self.fill["shade"].toxmlstr(True)
 
-                if self.borders[side] is not None:
-                    bx = self.borders[side].toxml()
-                    tabdata.append(bx)
+        # TableData children
 
-            for cell in self.cells:
-                cx = cell.toxml()
-                tabdata.append(cx)
+        for side in ["left", "right", "top", "bottom"]:
 
-            # Adding TableData as xml child
-            xml.append(tabdata)
+            if self.borders[side] is not None:
+                bx = self.borders[side].toxml()
+                tabdata.append(bx)
 
-            return xml
+        for cell in self.cells:
+            cx = cell.toxml()
+            tabdata.append(cx)
 
-        return False
+        # Adding TableData as xml child
+        xml.append(tabdata)
 
-    def fromxml(self, xml):
+        return xml
+
+    def fromxml(self, xml: ET._Element):
         succeed = PageObject.fromxml(self, xml)
 
-        if succeed:
+        if not succeed:
+            return False
 
-            # --- Attributes ---------------------------------------------
+        # --- Attributes ---------------------------------------------
 
-            # Number of rows and columns
+        tstyle = xml.get("TableStyle")
+        if tstyle is not None:
+            self.style = tstyle
 
-            rows = xml.get("Rows")
-            if rows is not None:
-                self.rows = int(rows)
+        # Number of rows and columns
 
-            cols = xml.get("Columns")
-            if cols is not None:
-                self.columns = int(cols)
+        rows = xml.get("Rows")
+        if rows is not None:
+            self.rows = int(rows)
 
-            # Rows and columns widths and heights -------------------
+        cols = xml.get("Columns")
+        if cols is not None:
+            self.columns = int(cols)
 
-            # Getting rows datas -------------------------------
+        # Rows and columns widths and heights -------------------
 
-            # Y position of the row, with the top-left corner
-            # of the first cell of the first row is at 0
+        # Getting rows datas -------------------------------
 
-            row_y = xml.get("RowPositions")
-            if row_y is not None:
-                row_y = [float(i) for i in row_y.split()]
+        # Y position of the row, with the top-left corner
+        # of the first cell of the first row is at 0
 
-            # Height (dimension, not position)
+        row_y = xml.get("RowPositions")
+        if row_y is not None:
+            row_y = [float(i) for i in row_y.split()]
 
-            row_h = xml.get("RowHeights")
-            if row_h is not None:
-                row_h = [float(i) for i in row_h.split()]
+        # Height (dimension, not position)
 
-            # Getting columns datas ----------------------------
+        row_h = xml.get("RowHeights")
+        if row_h is not None:
+            row_h = [float(i) for i in row_h.split()]
 
-            # X position of the column, with the top-left corner
-            # of the first cell of the first row is at 0
+        # Getting columns datas ----------------------------
 
-            col_x = xml.get("ColumnPositions")
-            if col_x is not None:
-                col_x = [float(i) for i in col_x.split()]
+        # X position of the column, with the top-left corner
+        # of the first cell of the first row is at 0
 
-            # Width (dimension, not position)
+        col_x = xml.get("ColumnPositions")
+        if col_x is not None:
+            col_x = [float(i) for i in col_x.split()]
 
-            col_w = xml.get("ColumnWidths")
-            if col_w is not None:
-                col_w = [float(i) for i in col_w.split()]
+        # Width (dimension, not position)
 
-            # Mixing datas together ----------------------------
-            # cols datas: index, X, width
-            # rows dataa: index, Y, height
+        col_w = xml.get("ColumnWidths")
+        if col_w is not None:
+            col_w = [float(i) for i in col_w.split()]
 
-            cols_datas = [
-                i for i in zip([x for x in range(len(col_x))], col_x, col_w)
-            ]
+        # Mixing datas together ----------------------------
+        # cols datas: index, X, width
+        # rows dataa: index, Y, height
 
-            rows_datas = [
-                i for i in zip([y for y in range(len(row_y))], row_y, row_h)
-            ]
+        cols_datas = [
+            i for i in zip([x for x in range(len(col_x))], col_x, col_w)
+        ]
 
-            # --- Children -----------------------------------------------
+        rows_datas = [
+            i for i in zip([y for y in range(len(row_y))], row_y, row_h)
+        ]
 
-            border_tags = [
-                i for i in pstyles.TableBorder.sides_xml.values()
-            ]
+        # --- Children -----------------------------------------------
 
-            for element in xml:
+        border_tags = [i for i in pstyles.TableBorder.sides_xml.values()]
 
-                if element.tag == "TableData":
+        for element in xml:
 
-                    style = element.get("Style")
-                    if style is not None:
-                        self.style = style
-
-                    fill_color = element.get("FillColor")
-                    if fill_color is not None:
-                        self.fill["color"] = fill_color
-
-                    fill_shade = element.get("FillShade")
-                    if fill_shade is not None:
-                        self.fill["shade"] = dimensions.Dim(
-                            float(fill_shade), unit="pc"
-                        )
+            if element.tag == "TableData":
 
-                    for sub in element:
+                dstyle = element.get("Style")
+                if dstyle is not None:
+                    self.data_style = dstyle
 
-                        if sub.tag in border_tags:
-                            bx = pstyles.TableBorder()
+                fill_color = element.get("FillColor")
+                if fill_color is not None:
+                    self.fill["color"] = fill_color
 
-                            success = bx.fromxml(sub)
-                            if success:
-                                self.borders[bx.side] = bx
+                fill_shade = element.get("FillShade")
+                if fill_shade is not None:
+                    self.fill["shade"] = dimensions.Dim(
+                        float(fill_shade), unit="pc"
+                    )
 
-                        if sub.tag == "Cell":
-                            cx = TableCell(self)
+                for sub in element:
 
-                            success = cx.fromxml(sub)
-                            if success:
-                                self.cells.append(cx)
+                    if sub.tag in border_tags:
+                        bx = pstyles.TableBorder()
 
-            # ------------------------------------------------------------
+                        success = bx.fromxml(sub)
+                        if success:
+                            self.borders[bx.side] = bx
 
-            self._update_cells_geometry(cols_datas, rows_datas)
+                    if sub.tag == "Cell":
+                        cx = TableCell(self)
 
-            self._update_rowcols_count()
+                        success = cx.fromxml(sub)
+                        if success:
+                            self.cells.append(cx)
 
-            return True
+        # ------------------------------------------------------------
 
-        return False
+        self._update_cells_geometry(cols_datas, rows_datas)
+
+        self._update_rowcols_count()
+
+        return True
 
 
 class GroupObject(PageObject):
     """
     Group of page objects.
 
     :type sla_parent: pyscribus.sla.SLA
@@ -1459,118 +1586,117 @@
 
     :ivar list group_objects: Page objects contained in this group.
     """
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "group", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
         self.group_objects = []
 
         self.group_box = dimensions.DimBox()
 
-        #--- Then, quick setup -------------------------------------------
+        # Then, quick setup ----------------------------------------------
 
         PageObject._quick_setup(self, kwargs)
 
     def toxml(self):
         """
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         :returns: Table object as LXML element
         """
 
         xml = PageObject.toxml(self)
 
-        if isinstance(xml, ET._Element):
-            xml.attrib["groupWidth"] = self.group_box.dims["width"].toxmlstr()
-            xml.attrib["groupHeight"] = self.group_box.dims["height"].toxmlstr()
+        if not isinstance(xml, ET._Element):
+            return False
 
-            # TODO FIXME Undocumented : @groupClips
+        xml.attrib["groupWidth"] = self.group_box.dims["width"].toxmlstr()
+        xml.attrib["groupHeight"] = self.group_box.dims["height"].toxmlstr()
 
-            #--- FIXME This exports undocumented attributes --------------
+        # TODO FIXME Undocumented : @groupClips
 
-            try:
-                xml, undoc_attribs = xmlc.all_undocumented_to_xml(
-                    xml, self.undocumented, True,
-                    self.ptype + " '{}'".format(self.name.strip()),
-                    logger=logs.getLogger()
-                )
+        # FIXME This exports undocumented attributes -----------------
 
-            except AttributeError:
-                # NOTE If fromxml was not used
-                pass
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
 
-            # --- Children -----------------------------------------------
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
 
-            for group_object in self.group_objects:
-                grx = group_object.toxml()
+        # --- Children -----------------------------------------------
 
-                if isinstance(grx, ET._Element):
-                    xml.append(grx)
+        for group_object in self.group_objects:
+            grx = group_object.toxml()
 
-            return xml
+            if isinstance(grx, ET._Element):
+                xml.append(grx)
 
-        return False
+        return xml
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         succeed = PageObject.fromxml(self, xml)
 
         # TODO Undocumented : @groupClips
 
-        if succeed:
-            # --- Group box ----------------------------------------------
+        if not succeed:
+            return False
 
-            # NOTE Group box have the same values of PageObject.box, but
-            # is defined with other attributes
+        # --- Group box ----------------------------------------------
 
-            grxpos = xml.get("XPOS")
-            grypos = xml.get("YPOS")
-            grwidth = xml.get("groupWidth")
-            grheight = xml.get("groupHeight")
+        # NOTE Group box have the same values of PageObject.box, but
+        # is defined with other attributes
 
-            valid_box = 0
+        grxpos = xml.get("XPOS")
+        grypos = xml.get("YPOS")
+        grwidth = xml.get("groupWidth")
+        grheight = xml.get("groupHeight")
 
-            for test in [grxpos, grypos, grwidth, grheight]:
-                if test is not None:
-                    valid_box += 1
+        valid_box = 0
 
-            if valid_box == 4:
+        for test in [grxpos, grypos, grwidth, grheight]:
+            if test is not None:
+                valid_box += 1
 
-                self.group_box.set_box(
-                    top_lx=grxpos,
-                    top_ly=grypos,
-                    width=grwidth,
-                    height=grheight
-                )
+        if valid_box == 4:
 
-            # ------------------------------------------------------------
+            self.group_box.set_box(
+                top_lx=grxpos, top_ly=grypos, width=grwidth, height=grheight
+            )
+
+        # ------------------------------------------------------------
 
-            for element in xml:
+        for element in xml:
 
-                element_ptype = element.get("PTYPE")
-                if element_ptype is not None:
+            element_ptype = element.get("PTYPE")
 
-                    try:
-                        po = new_from_type(
-                            element_ptype, self.sla_parent,
-                            self.doc_parent
-                        )
+            if element_ptype is not None:
 
-                        success = po.fromxml(element)
+                try:
+                    po = new_from_type(
+                        element_ptype, self.sla_parent, self.doc_parent
+                    )
 
-                        if success:
-                            self.group_objects.append(po)
+                    success = po.fromxml(element)
 
-                    except ValueError:
-                        pass
+                    if success:
+                        self.group_objects.append(po)
 
-            return True
+                except ValueError:
+                    pass
 
-        return False
+        return True
 
 
 class SymbolObject(PageObject):
     """
     Symbol object.
 
     :type sla_parent: pyscribus.sla.SLA
@@ -1580,19 +1706,19 @@
     :type kwargs: dict
     :param kwargs: Quick setting (see kwargs table)
     """
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "symbol", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
         self.pattern = None
 
-        #--- Then, quick setup -------------------------------------------
+        # Then, quick setup ----------------------------------------------
 
         PageObject._quick_setup(self, kwargs)
 
 
 class TextObject(PageObject):
     """
     Text frame object
@@ -1624,45 +1750,38 @@
     |            | text.                           |           |
     |            |                                 |           |
     |            | Must be "top", "center",        |           |
     |            | "center".                       |           |
     +------------+---------------------------------+-----------+
     """
 
-    vertical_alignment_xml = {
-        "top": "0",
-        "center": "1",
-        "bottom": "2"
-    }
+    vertical_alignment_xml = {"top": "0", "center": "1", "bottom": "2"}
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "text", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
         self.stories = []
 
-        self.columns = {
-            "gap": dimensions.Dim(0),
-            "count": 0
-        }
+        self.columns = {"gap": dimensions.Dim(0), "count": 0}
 
         self.is_autotext = False
 
         self.padding = {
             "left": dimensions.Dim(0),
             "right": dimensions.Dim(0),
             "bottom": dimensions.Dim(0),
             "top": dimensions.Dim(0),
         }
 
         self.alignment = None
         self.vertical_alignment = "top"
 
-        #--- Then, quick setup -------------------------------------------
+        # Then, quick setup ----------------------------------------------
 
         self._quick_setup(kwargs)
 
     def _quick_setup(self, settings):
         """
         Method for defining page object settings from class
         instanciation kwargs.
@@ -1678,216 +1797,298 @@
 
                 if setting_name == "valign":
                     setting_value = setting_value.lower()
 
                     if setting_value in TextObject.vertical_alignment_xml:
                         self.vertical_alignment = setting_value
                     else:
+                        valid_values = ", ".join(
+                            [
+                                "'{}'".format(v)
+                                for v in TextObject.vertical_alignment_xml.values()
+                            ]
+                        )
+
                         raise exceptions.QuickSetupInvalidValue(
                             "valign setting value must be in [{}].".format(
-                                ", ".join(
-                                    [
-                                        "'{}'".format(v)
-                                        for v in TextObject.vertical_alignment_xml.values()
-                                    ]
-                                )
+                                valid_values
                             )
                         )
 
                 if setting_name == "columns":
                     self.columns["count"] = int(setting_value)
 
                 if setting_name == "columnsgap":
                     self.columns["gap"].value = float(setting_value)
 
-    def fromdefault(self, default="with-story"):
-        story = stories.Story()
-        story.fromdefault()
-        self.stories.append(story)
-        self.have_stories = True
-
-        self.columns = {
-            "gap": dimensions.Dim(0),
-            "count": 1
+    def fromdefault(self, default: str = "with-story"):
+        # Page object default
+
+        # FIXME Those two line are hacks
+        self.text_flow = PageObject.text_flow_xml["2"]
+        self.path_options["text_on_path"] = {
+            "show": False,
+            "offset": dimensions.Dim(0)
         }
 
+        self.outline["fill"] = None
+        self.outline["stroke"] = None
+
+        self.columns = {"gap": dimensions.Dim(0), "count": 1}
+
+        # Stories default
+
+        if default == "with-story":
+            story = stories.Story()
+            story.fromdefault()
+            self.stories.append(story)
+            self.have_stories = True
+
     def templatable(self):
-        stories = []
+        temp_stories = []
 
         if self.have_stories and self.stories:
 
             for story in self.stories:
 
                 if story.templatable():
 
-                    stories.append(story)
+                    temp_stories.append(story)
 
-        return stories
+        return temp_stories
 
     def fromxml(self, xml):
         succeed = PageObject.fromxml(self, xml)
 
-        if succeed:
-
-            # --- Attributes ---------------------------------------------
-
-            # NOTE FIXME
-            # PLTSHOW |(optional) Set to 1 if the path of a Text on a path
-            #         |should be shown
-            # BASEOF  |(optional) Offset for the text from its path for text
-            #         |on a path
-
-            # NOTE FIXME
-            # Undocumented :
-            #
-            # textPathType
-            # textPathFlipped
-            # FLOP
-
-            valign = xml.get("VAlign")
-            if valign is not None:
-                for human, code in TextObject.vertical_alignment_xml.items():
-                    if valign == code:
-                        self.vertical_alignment = human
-                        break
+        if not succeed:
+            return False
 
-            autotext = xml.get("AUTOTEXT")
-            if autotext is not None:
-                self.is_autotext = xmlc.num_to_bool(autotext)
-
-            for case in [
-                ["left", "EXTRA"], ["right", "REXTRA"],
-                ["bottom", "BEXTRA"], ["top", "TEXTRA"]]:
-
-                padding_arg = xml.get(case[1])
-                if padding_arg is not None:
-                    self.padding[case[0]].value = float(padding_arg)
-
-            columns = xml.get("COLUMNS")
-            if columns is not None:
-                self.columns["count"] = int(columns)
-
-            columnsgap = xml.get("COLGAP")
-            if columnsgap is not None:
-                self.columns["gap"].value = float(columnsgap)
-
-            alignment = xml.get("ALIGN")
-            if alignment is not None:
-                for human, code in xmlc.alignment.items():
-                    if alignment == code:
-                        self.alignment = human
-                        break
+        # --- Attributes ---------------------------------------------
 
-            # --- Childs -------------------------------------------------
+        # NOTE FIXME
+        # BASEOF  |(optional) Offset for the text from its path for text
+        #         |on a path
+
+        # NOTE FIXME
+        # Undocumented :
+        #
+        # textPathType
+        # textPathFlipped
+        # FLOP
+
+        valign = xml.get("VAlign")
+        if valign is not None:
+            for human, code in TextObject.vertical_alignment_xml.items():
+                if valign == code:
+                    self.vertical_alignment = human
+                    break
 
-            for element in xml:
+        autotext = xml.get("AUTOTEXT")
+        if autotext is not None:
+            self.is_autotext = xmlc.num_to_bool(autotext)
+
+        for case in [
+            ["left", "EXTRA"],
+            ["right", "REXTRA"],
+            ["bottom", "BEXTRA"],
+            ["top", "TEXTRA"],
+        ]:
+
+            padding_arg = xml.get(case[1])
+            if padding_arg is not None:
+                self.padding[case[0]].value = float(padding_arg)
+
+        columns = xml.get("COLUMNS")
+        if columns is not None:
+            self.columns["count"] = int(columns)
+
+        columnsgap = xml.get("COLGAP")
+        if columnsgap is not None:
+            self.columns["gap"].value = float(columnsgap)
+
+        alignment = xml.get("ALIGN")
+        if alignment is not None:
+            for human, code in xmlc.alignment.items():
+                if alignment == code:
+                    self.alignment = human
+                    break
 
-                if element.tag == "PageItemAttributes":
+        # --- Childs -------------------------------------------------
 
-                    for sub in element:
+        for element in xml:
 
-                        if sub.tag == "ItemAttribute":
-                            iatt = itemattribute.PageObjectAttribute()
+            if element.tag == "PageItemAttributes":
 
-                            success = iatt.fromxml(sub)
-                            if success:
-                                self.attributes.append(iatt)
+                for sub in element:
 
-                if element.tag == "WeldEntry":
-                    wo = WeldEntry()
-                    success = wo.fromxml(element)
+                    if sub.tag == "ItemAttribute":
+                        iatt = itemattribute.PageObjectAttribute()
 
-                    if wo:
-                        # TODO FIXME Comment gérér les WeldEntry dans les
-                        # instances PageObject ?
-                        pass
+                        success = iatt.fromxml(sub)
+                        if success:
+                            self.attributes.append(iatt)
 
-                if element.tag == "StoryText":
-                    story = stories.Story()
+            if element.tag == "WeldEntry":
+                wo = WeldEntry()
+                success = wo.fromxml(element)
+
+                if wo:
+                    # TODO FIXME Comment gérér les WeldEntry dans les
+                    # instances PageObject ?
+                    pass
 
-                    story.sla_parent = self.sla_parent
-                    story.doc_parent = self.doc_parent
+            if element.tag == "StoryText":
+                story = stories.Story()
 
-                    success = story.fromxml(element)
-                    if success:
-                        if not self.stories:
-                            self.have_stories = True
+                story.sla_parent = self.sla_parent
+                story.doc_parent = self.doc_parent
 
-                        self.stories.append(story)
+                success = story.fromxml(element)
+                if success:
+                    if not self.stories:
+                        self.have_stories = True
 
-            return True
+                    self.stories.append(story)
 
-        return False
+        return True
 
     def toxml(self):
         """
         :rtype: lxml.etree._Element
-        :returns: Table object as LXML element
+        :returns: Text object as LXML element
         """
 
         xml = PageObject.toxml(self)
 
-        if isinstance(xml, ET._Element):
-            #--- Attributes ----------------------------------------------
-
-            xml.attrib["COLUMNS"] = str(self.columns["count"])
-            xml.attrib["COLGAP"] = self.columns["gap"].toxmlstr()
-
-            if self.alignment is not None:
-                xml.attrib["ALIGN"] = xmlc.alignment[self.alignment]
-
-            xml.attrib["VAlign"] = TextObject.vertical_alignment_xml[self.vertical_alignment]
+        if not isinstance(xml, ET._Element):
+            return False
 
-            # Padding
+        # Attributes -------------------------------------------------
 
-            for case in [
-                ["left", "EXTRA"], ["right", "REXTRA"],
-                ["bottom", "BEXTRA"], ["top", "TEXTRA"]]:
+        xml.attrib["COLUMNS"] = str(self.columns["count"])
+        xml.attrib["COLGAP"] = self.columns["gap"].toxmlstr(True)
 
-                xml.attrib[case[1]] = self.padding[case[0]].toxmlstr(True)
+        if self.alignment is not None:
+            xml.attrib["ALIGN"] = xmlc.alignment[self.alignment]
 
-            xml.attrib["AUTOTEXT"] = xmlc.bool_to_num(self.is_autotext)
+        xml.attrib["VAlign"] = TextObject.vertical_alignment_xml[
+            self.vertical_alignment
+        ]
 
-            #--- FIXME This exports undocumented attributes --------------
+        # Padding
 
-            try:
-                xml, undoc_attribs = xmlc.all_undocumented_to_xml(
-                    xml, self.undocumented, True,
-                    self.ptype + " '{}'".format(self.name.strip()),
-                    logger=logs.getLogger()
-                )
+        for case in [
+            ["left", "EXTRA"],
+            ["right", "REXTRA"],
+            ["bottom", "BEXTRA"],
+            ["top", "TEXTRA"],
+        ]:
+
+            xml.attrib[case[1]] = self.padding[case[0]].toxmlstr(True)
+
+        xml.attrib["AUTOTEXT"] = xmlc.bool_to_num(self.is_autotext)
+
+        # FIXME This exports undocumented attributes -----------------
+
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
 
-            except AttributeError:
-                # NOTE If fromxml was not used
-                pass
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
 
-            # --- Children -----------------------------------------------
+        # --- Children -----------------------------------------------
 
-            if self.have_stories:
+        if self.have_stories:
 
-                for story in self.stories:
-                    sx = story.toxml()
-                    xml.append(sx)
+            for story in self.stories:
+                story_xml = story.toxml()
+                xml.append(story_xml)
 
-            return xml
+        return xml
 
-        return False
 
+# FIXME TODO Maybe rebase TextObject and TextOnPathObject on a common class
+# instead of copying some parts into TextOnPathObject
 
 class TextOnPathObject(PageObject):
     """
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
     :param doc_parent: SLA DOCUMENT instance
     """
 
     def __init__(self, sla_parent=False, doc_parent=False):
         PageObject.__init__(self, "textonpath", sla_parent, doc_parent)
 
+        self.stories = []
+
+    def fromxml(self, xml):
+        succeed = PageObject.fromxml(self, xml)
+
+        for element in xml:
+
+            if element.tag == "StoryText":
+                story = stories.Story()
+
+                story.sla_parent = self.sla_parent
+                story.doc_parent = self.doc_parent
+
+                success = story.fromxml(element)
+                if success:
+                    if not self.stories:
+                        self.have_stories = True
+
+                    self.stories.append(story)
+
+        return True
+
+    def toxml(self):
+        """
+        :rtype: lxml.etree._Element
+        :returns: TextOnPath object as LXML element
+        """
+
+        xml = PageObject.toxml(self)
+
+        if not isinstance(xml, ET._Element):
+            return False
+
+        # FIXME This exports undocumented attributes -----------------
+
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
+
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
+
+        # --- Children -----------------------------------------------
+
+        if self.have_stories:
+
+            for story in self.stories:
+                story_xml = story.toxml()
+                xml.append(story_xml)
+
+        return xml
+
 
 class ImageObject(PageObject):
     """
     Image frame object
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
@@ -1913,57 +2114,164 @@
     +------------+---------------------------------+---------------+
 
     :ivar string filepath: File path of the image
     :ivar string data: Data if the incorporated image
     :ivar string data_type: Filetype of the incorporated image
     """
 
+    render_xml = {
+        "0": "perceptual",
+        "1": "rel_colorimetric",
+        "2": "saturation",
+        "3": "abs_colorimetric",
+    }
+
+    compression_method_xml = {
+        "0": "auto",
+        "1": "jpeg",
+        "2": "flate",
+        "3": "none",
+    }
+
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "image", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
-        self.data = "" # ImageData
+        self.data = ""  # ImageData
         self.data_type = ""
-        self.filepath = "" # PFILE
+        self.filepath = ""  # PFILE
 
-        #--- Then, quick setup -------------------------------------------
+        self.render_intent = ImageObject.render_xml["0"]
+
+        self.page_number = 0
+        self.is_inline = False
+
+        self.compression = {
+            "method": "auto",
+            "__method": None,
+        }
+
+        # Then, quick setup ----------------------------------------------
 
         self._quick_setup(kwargs)
 
+    def toxml(self):
+        """
+        :rtype: lxml.etree._Element
+        :returns: Table object as LXML element
+        """
+
+        xml = PageObject.toxml(self)
+
+        xml.attrib["Pagenumber"] = str(self.page_number)
+
+        # Compression method ------------------------------
+
+        # @CMethod and @COMPRESSIONMETHOD follow the same syntax
+        cmethod_att = self.compression["__method"]
+
+        if cmethod_att is not None:
+
+            for code, human in ImageObject.compression_method_xml.items():
+                if human == self.compression["method"]:
+                    xml.attrib[cmethod_att] = code
+                    break
+
+        # -------------------------------------------------
+
+        for code, human in ImageObject.render_xml.items():
+            if self.render_intent == human:
+                xml.attrib["IRENDER"] = code
+
+        if self.is_inline:
+            xml.attrib["isInlineImage"] = xmlc.bool_to_num(self.is_inline)
+
+        # FIXME This exports undocumented attributes -----------------
+
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
+
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
+
+        return xml
+
     def fromxml(self, xml):
         succeed = PageObject.fromxml(self, xml)
 
-        if succeed:
+        if not succeed:
+            return False
 
-            # --- Attributes ---------------------------------------------
+        # --- Attributes ---------------------------------------------
 
-            ipath = xml.get("PFILE")
-            idata_ext = xml.get("inlineImageExt")
+        ipath = xml.get("PFILE")
+        idata_ext = xml.get("inlineImageExt")
 
-            idata = xml.get("ImageData")
-            if idata is not None:
-                if idata:
-                    self.data = idata
-
-            idata_ext = xml.get("inlineImageExt")
-            if idata_ext is not None:
-                if idata_ext:
-                    self.data_type = idata_ext
-
-            ipath = xml.get("PFILE")
-            if ipath is not None:
-                if ipath:
-                    self.filepath = ipath
+        # Compression method ------------------------------
 
-            # ------------------------------------------------------------
+        # @CMethod and @COMPRESSIONMETHOD follow the same syntax
 
-            return True
+        cmethod = xml.get("CMethod")
+        cmethod_long = xml.get("COMPRESSIONMETHOD")
 
-        return False
+        for att, value in [
+            ["COMPRESSIONMETHOD", cmethod_long], ["CMethod", cmethod]
+        ]:
+            if value is None:
+                continue
+
+            self.compression["method"] = ImageObject.compression_method_xml[value]
+            self.compression["__method"] = att
+
+        # -------------------------------------------------
+
+        irender = xml.get("IRENDER")
+        if irender is not None:
+            for code, human in ImageObject.render_xml.items():
+                if irender == code:
+                    self.render_intent = human
+
+        is_inline = xml.get("isInlineImage")
+        if is_inline is not None:
+            self.is_inline = xmlc.num_to_bool(is_inline)
+
+        pgnumber = xml.get("Pagenumber")
+        if pgnumber is not None:
+            try:
+                pgnumber = int(pgnumber)
+                self.page_number = pgnumber
+            except ValueError:
+                self.page_number = 0
+
+        idata = xml.get("ImageData")
+        if idata is not None:
+            if idata:
+                self.data = idata
+
+        idata_ext = xml.get("inlineImageExt")
+        if idata_ext is not None:
+            if idata_ext:
+                self.data_type = idata_ext
+
+        ipath = xml.get("PFILE")
+        if ipath is not None:
+            if ipath:
+                self.filepath = ipath
+
+        # ------------------------------------------------------------
+
+        return True
 
     def _quick_setup(self, settings):
         """
         Method for defining page object settings from class
         instanciation kwargs.
 
         :type settings: dict
@@ -1989,30 +2297,29 @@
     :type doc_parent: pyscribus.document.Document
     :param doc_parent: SLA DOCUMENT instance
     """
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "line", sla_parent, doc_parent)
 
-        #--- Specific attributes to this subclass ------------------------
+        # Specific attributes to this subclass ---------------------------
 
         self.outline["thickness"].value = float(1)
 
-        #--- Then, quick setup -------------------------------------------
+        # Then, quick setup ----------------------------------------------
 
         PageObject._quick_setup(self, kwargs)
 
     def fromxml(self, xml):
         succeed = PageObject.fromxml(self, xml)
 
-        if succeed:
-
-            return True
+        if not succeed:
+            return False
 
-        return False
+        return True
 
 
 class PolylineObject(PageObject):
     """
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
@@ -2056,45 +2363,44 @@
         self.buffer = None
 
     # -----------------------------------------------------------------------
 
     def fromxml(self, xml):
         succeed = PageObject.fromxml(self, xml)
 
-        if succeed:
-
-            # ------------------------------------------------------------
+        if not succeed:
+            return False
 
-            for child in xml:
+        # ------------------------------------------------------------
 
-                if child.tag == "LATEX":
-                    bfr = RenderBuffer()
+        for child in xml:
 
-                    success = bfr.fromxml(child)
-                    if success:
-                        self.buffer = bfr
+            if child.tag == "LATEX":
+                bfr = RenderBuffer()
 
-            # ------------------------------------------------------------
+                success = bfr.fromxml(child)
+                if success:
+                    self.buffer = bfr
 
-            return True
+        # ------------------------------------------------------------
 
-        return False
+        return True
 
     def toxml(self):
         xml = PageObject.toxml(self)
 
-        if xml is not None:
-            # --- Children -----------------------------------------------
+        if xml is None:
+            return False
 
-            bfrx = self.buffer.toxml()
-            xml.append(bfrx)
+        # --- Children -----------------------------------------------
 
-            return xml
+        bfrx = self.buffer.toxml()
+        xml.append(bfrx)
 
-        return False
+        return xml
 
     # --- RenderBuffer methods aliases --------------------------------------
 
     def has_package(self, name):
         """
         Check if package name exists in the LaTeX preamble of the render frame
         buffer.
@@ -2167,16 +2473,18 @@
 
     .. seealso:: :class:`RenderObject`
     """
 
     def __init__(self, sla_parent=False, doc_parent=False):
         RenderObject.__init__(self, sla_parent, doc_parent)
 
+
 # Cell object for table =================================================#
 
+
 class TableCell(xmlc.PyScribusElement):
     """
     Cell in a table object (PAGEOBJECT/TableData/Cell)
 
     :type pgo_parent: pyscribus.pageobjects.PageObject
     :param pgo_parent: Parent page object instance.
     :type kwargs: dict
@@ -2306,21 +2614,25 @@
         # Appearance of the cell -----------------------------------------
 
         self.style = None
 
         self.fill = {"color": "None", "shade": None}
 
         self.borders = {
-            "left": None, "right": None,
-            "top": None, "bottom": None
+            "left": None,
+            "right": None,
+            "top": None,
+            "bottom": None,
         }
 
         self.padding = {
-            "left": None, "right": None,
-            "top": None, "bottom": None
+            "left": None,
+            "right": None,
+            "top": None,
+            "bottom": None,
         }
 
         self.align = None
 
         # Content of the cell --------------------------------------------
 
         self.story = None
@@ -2330,28 +2642,26 @@
         if kwargs:
             self._quick_setup(kwargs)
 
     def fromdefault(self):
 
         if self.pgo_parent:
             self.story = stories.Story(
-                self.pgo_parent.sla_parent,
-                self.pgo_parent.doc_parent,
-                self
+                self.pgo_parent.sla_parent, self.pgo_parent.doc_parent, self
             )
         else:
             self.story = stories.Story()
 
         self.story.fromdefault()
 
         self.padding = {
             "left": dimensions.Dim(1),
             "right": dimensions.Dim(1),
             "top": dimensions.Dim(1),
-            "bottom": dimensions.Dim(1)
+            "bottom": dimensions.Dim(1),
         }
 
         self.align = "top"
 
     def _quick_setup(self, settings):
         """
         Method for defining table cell settings from class instanciation
@@ -2380,44 +2690,36 @@
 
             if isinstance(setting_value, list):
                 setting_len = len(setting_value)
 
                 if setting_len == 1:
 
                     for side in ["top", "right", "bottom", "left"]:
-                        objattribute[side].value = float(
-                            setting_value[0]
-                        )
+                        objattribute[side].value = float(setting_value[0])
 
                 if setting_len == 2:
                     sides = zip(
-                        [["top", "bottom"], ["right", "left"]],
-                        setting_value
+                        [["top", "bottom"], ["right", "left"]], setting_value
                     )
 
                     for side in sides:
                         for s in side[0]:
                             objattribute[s].value = float(side[1])
 
                 if setting_len == 3:
                     objattribute["top"].value = float(setting_value[0])
 
                     for side in ["right", "left"]:
-                        objattribute[side].value = float(
-                            setting_value[1]
-                        )
+                        objattribute[side].value = float(setting_value[1])
 
-                    objattribute["bottom"].value = float(
-                        setting_value[2]
-                    )
+                    objattribute["bottom"].value = float(setting_value[2])
 
                 if setting_len == 4:
                     sides = zip(
-                        ["top", "right", "bottom", "left"],
-                        setting_value
+                        ["top", "right", "bottom", "left"], setting_value
                     )
 
                     for side in sides:
                         objattribute[side[0]].value = float(side[1])
 
             return objattribute
 
@@ -2445,29 +2747,35 @@
                         self.align = setting_value
                     else:
                         self.align = "top"
 
                 # Borders -----------------------------------------------------
 
                 if setting_name in [
-                        "rightborder", "leftborder",
-                        "topborder", "bottomborder"]:
+                    "rightborder",
+                    "leftborder",
+                    "topborder",
+                    "bottomborder",
+                ]:
                     side = setting_name.split("border")[0]
                     self.borders[side].value = float(setting_value)
 
                 if setting_name == "borders":
                     self.borders = shortcut_geometry_setting(
                         self.borders, setting_value
                     )
 
                 # Padding -----------------------------------------------------
 
                 if setting_name in [
-                        "rightpadding", "leftpadding",
-                        "toppadding", "bottompadding"]:
+                    "rightpadding",
+                    "leftpadding",
+                    "toppadding",
+                    "bottompadding",
+                ]:
                     side = setting_name.split("padding")[0]
                     self.padding[side].value = float(setting_value)
 
                 if setting_name == "padding":
                     self.padding = shortcut_geometry_setting(
                         self.padding, setting_value
                     )
@@ -2490,111 +2798,109 @@
 
                 if setting_name == "width":
                     self.box.dims["width"].value = float(setting_value)
 
                 if setting_name == "height":
                     self.box.dims["height"].value = float(setting_value)
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         """
         Parses XML of a SLA table cell.
 
-        :type xml: lxml._Element
-        :param xml: SLA table cell as lxml._Element
+        :type xml: lxml.etree._Element
+        :param xml: SLA table cell as lxml.etree._Element
 
         :rtype: bool
         :returns: bool
         """
 
-        if xml.tag == "Cell":
-            border_tags = [
-                i for i in pstyles.TableBorder.sides_xml.values()
-            ]
+        if xml.tag != "Cell":
+            return False
 
-            # Position of the cell -----------------------------------
+        border_tags = [i for i in pstyles.TableBorder.sides_xml.values()]
 
-            row = xml.get("Row")
-            column = xml.get("Column")
+        # Position of the cell -----------------------------------
 
-            if row is None or column is None:
-                raise exceptions.InsaneSLAValue(
-                    "A table cell has no @Row or @Column attribute."
-                )
-            else:
-                self.row = int(row)
-                self.column = int(column)
+        row = xml.get("Row")
+        column = xml.get("Column")
 
-            # Cell attributes ----------------------------------------
+        if row is None or column is None:
+            raise exceptions.InsaneSLAValue(
+                "A table cell has no @Row or @Column attribute."
+            )
 
-            style = xml.get("Style")
-            if style is not None:
-                self.style = style
+        self.row = int(row)
+        self.column = int(column)
 
-            align = xml.get("TextVertAlign")
-            if align is not None:
+        # Cell attributes ----------------------------------------
 
-                for human,code in TableCell.vertical_align.items():
-                    if align == code:
-                        self.align = human
-                        break
+        style = xml.get("Style")
+        if style is not None:
+            self.style = style
 
-            fill_color = xml.get("FillColor")
-            if fill_color is not None:
-                self.fill["color"] = fill_color
+        align = xml.get("TextVertAlign")
+        if align is not None:
 
-            fill_shade = xml.get("FillShade")
-            if fill_shade is not None:
-                self.fill["shade"] = dimensions.Dim(float(fill_shade), unit="pc")
+            for human, code in TableCell.vertical_align.items():
+                if align == code:
+                    self.align = human
+                    break
 
-            for side in ["left", "right", "top", "bottom"]:
-                att_name = "{}Padding".format(side.capitalize())
+        fill_color = xml.get("FillColor")
+        if fill_color is not None:
+            self.fill["color"] = fill_color
+
+        fill_shade = xml.get("FillShade")
+        if fill_shade is not None:
+            self.fill["shade"] = dimensions.Dim(float(fill_shade), unit="pc")
 
-                att = xml.get(att_name)
-                if att is not None:
-                    self.padding[side] = dimensions.Dim(float(att))
+        for side in ["left", "right", "top", "bottom"]:
+            att_name = "{}Padding".format(side.capitalize())
 
-            for element in xml:
+            att = xml.get(att_name)
+            if att is not None:
+                self.padding[side] = dimensions.Dim(float(att))
 
-                # Story of the cell --------------------------------------
+        for element in xml:
 
-                if element.tag == "StoryText":
+            # Story of the cell --------------------------------------
 
-                    if self.pgo_parent:
-                        story = stories.Story(
-                            self.pgo_parent.sla_parent,
-                            self.pgo_parent.doc_parent,
-                            self
-                        )
-                    else:
-                        story = stories.Story(pgo_parent=self)
+            if element.tag == "StoryText":
 
-                    success = story.fromxml(element)
+                if self.pgo_parent:
+                    story = stories.Story(
+                        self.pgo_parent.sla_parent,
+                        self.pgo_parent.doc_parent,
+                        self,
+                    )
+                else:
+                    story = stories.Story(pgo_parent=self)
 
-                    if success:
-                        self.story = story
+                success = story.fromxml(element)
 
-                # Borders of the cell if they are different of the table -
-                # borders.
+                if success:
+                    self.story = story
 
-                if element.tag in border_tags:
-                    bx = pstyles.TableBorder()
-                    success = bx.fromxml(element)
+            # Borders of the cell if they are different of the table -
+            # borders.
 
-                    if success:
-                        self.borders[bx.side] = bx
+            if element.tag in border_tags:
+                bx = pstyles.TableBorder()
+                success = bx.fromxml(element)
 
-            return True
+                if success:
+                    self.borders[bx.side] = bx
 
-        return False
+        return True
 
     def toxml(self):
         """
         Return the cell as XML element.
 
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         """
 
         xml = ET.Element("Cell")
 
         # Attributes ---------------------------------------------
 
         xml.attrib["Row"] = str(self.row)
@@ -2639,16 +2945,18 @@
         sx = self.story.toxml()
         xml.append(sx)
 
         # --------------------------------------------------------
 
         return xml
 
+
 # Render buffer and render properties ===================================#
 
+
 class RenderBuffer(xmlc.PyScribusElement):
     """
     Object for render frame's (RenderObject) content.
 
     :ivar list properties: List of properties
     :ivar string content: Content of the buffer
 
@@ -2682,35 +2990,36 @@
             RenderProperty("font", ""),
             RenderProperty("fontsize", "11pt"),
         ]
 
         # NOTE Standard printing DPI
         self.dpi.value = 300
 
-    def has_package(self, name):
+    def has_package(self, name: str):
         """
         Check if package name exists in the LaTeX preamble.
 
         :type name: str
         :param name: Name of the package
         :rtype: boolean
         :returns: True if the package exists
         :raise pyscribus.exceptions.UnknownRenderBufferProperty: If the LaTeX
             preamble property (HeadersRenderProperty) doesn't exists.
         """
-        for prop in properties:
+        for prop in self.properties:
 
             if isinstance(prop, HeadersRenderProperty):
                 return prop.has_package(name)
 
         raise exceptions.UnknownRenderBufferProperty(
-            "Property additionalheaders doesn't exists in render buffer object."
+            "Property additionalheaders doesn't exists in render buffer "
+            "object."
         )
 
-    def append_package(self, name, options=""):
+    def append_package(self, name: str, options: str = ""):
         """
         Append a package in the LaTeX preamble.
 
         :type name: str
         :param name: Name of the package
         :type options: str
         :param options: Package's options
@@ -2727,15 +3036,15 @@
         .. note:: As LaTeX additional headers is managed with
             :class:`HeadersRenderProperty`, it is better to use this method
             than editing ``RenderBuffer.properties``.
 
 
         """
 
-        for prop in properties:
+        for prop in self.properties:
 
             if isinstance(prop, HeadersRenderProperty):
                 prop.append_package(name, options)
 
                 return True
 
         return False
@@ -2754,68 +3063,65 @@
         for prop in self.properties:
 
             if prop.name == "fontsize":
                 prop.raw_value = "{}pt".format(float(fontsize))
 
                 return True
 
-        self.properties.append(
-            RenderProperty("fontsize", float(fontsize))
-        )
+        self.properties.append(RenderProperty("fontsize", float(fontsize)))
 
         return True
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         """
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
-        if xml.tag == "LATEX":
-            # Attributes
+        if xml.tag != "LATEX":
+            return False
+
+        # Attributes
 
-            dpi = xml.get("DPI")
-            if dpi is not None:
-                self.dpi.value = float(dpi)
+        dpi = xml.get("DPI")
+        if dpi is not None:
+            self.dpi.value = float(dpi)
 
-            use_preamble = xml.get("USE_PREAMBLE")
-            if use_preamble is not None:
-                self.use_preamble = xmlc.num_to_bool(use_preamble)
+        use_preamble = xml.get("USE_PREAMBLE")
+        if use_preamble is not None:
+            self.use_preamble = xmlc.num_to_bool(use_preamble)
 
-            configfile = xml.get("ConfigFile")
-            if configfile is not None:
-                self.configfile = configfile
+        configfile = xml.get("ConfigFile")
+        if configfile is not None:
+            self.configfile = configfile
 
-            # Properties
+        # Properties
 
-            for element in xml:
+        for element in xml:
 
-                if element.tag == "PROPERTY":
+            if element.tag == "PROPERTY":
 
-                    if "name" in element.attrib:
+                po = False
 
-                        if element.attrib["name"] == "additionalheaders":
-                            po = HeadersRenderProperty()
-                        else:
-                            po = RenderProperty()
+                if "name" in element.attrib:
 
+                    if element.attrib["name"] == "additionalheaders":
+                        po = HeadersRenderProperty()
                     else:
-                        po = False
+                        po = RenderProperty()
 
-                    if po:
-                        success = po.fromxml(element)
+                if po:
+                    success = po.fromxml(element)
 
-                        if success:
-                            self.properties.append(po)
+                    if success:
+                        self.properties.append(po)
 
-            # TODO Content
+        # TODO Content
 
-            return True
-        else:
-            return False
+        return True
 
     def toxml(self):
         xml = ET.Element("LATEX")
 
         xml.attrib["ConfigFile"] = self.configfile
         xml.attrib["DPI"] = self.dpi.toxmlstr()
         xml.attrib["USE_PREAMBLE"] = xmlc.bool_to_num(self.use_preamble)
@@ -2824,76 +3130,79 @@
             px = prop.toxml()
             xml.append(px)
 
         xml.text = self.content
 
         return xml
 
+
 class RenderProperty(xmlc.PyScribusElement):
     """
     Render frame / object property in SLA.
 
     :type name: str
     :param name: Name of the property
     :type value: str
     :param value: Value of the property
 
     .. note:: If you want to change the property value type, use
         RenderProperty.value. RenderProperty.raw_value keep property
         value as it was at instanciation.
 
-    .. note:: Use HeadersRenderProperty if your property name is "additionalheaders".
+    .. note:: Use HeadersRenderProperty if your property name is
+        "additionalheaders".
 
     .. seealso:: :class:`HeadersRenderProperty`
     """
 
-    def __init__(self, name="", value=False):
+    def __init__(self, name: str = "", value=False):
         xmlc.PyScribusElement.__init__(self)
 
         self.name = name
         self._set_value(value)
 
     def _set_value(self, value):
         self.raw_value = value
         self.value = copy.deepcopy(value)
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         """
         Define render property from lxml element.
 
-        :type xml: lxml._Element
-        :param xml: Render property as lxml._Element
+        :type xml: lxml.etree._Element
+        :param xml: Render property as lxml.etree._Element
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
-        if xml.tag == "PROPERTY":
-            name = xml.get("name")
-            if name is not None:
-                self.name = name
-
-            value = xml.get("value")
-            if value is not None:
-                self._set_value(value)
-
-            return True
-        else:
+        if xml.tag != "PROPERTY":
             return False
 
+        name = xml.get("name")
+        if name is not None:
+            self.name = name
+
+        value = xml.get("value")
+        if value is not None:
+            self._set_value(value)
+
+        return True
+
     def toxml(self):
         """
-        :returns: lxml._Element representation of render frame property
-        :rtype: lxml._Element
+        :returns: lxml.etree._Element representation of render frame property
+        :rtype: lxml.etree._Element
         """
         xml = ET.Element("PROPERTY")
         xml.attrib["name"] = self.name
         xml.attrib["value"] = self.raw_value
 
         return xml
 
+
 class HeadersRenderProperty(RenderProperty):
     """
     Render frame / object property in SLA for LaTeX preamble.
 
     :type value: str
     :param value: Value of the property
 
@@ -2907,23 +3216,23 @@
         RenderProperty.__init__(self, "additionalheaders", value)
 
         self.packages = []
 
         if value:
             self.packages = value.split("&#10;")
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element):
         success = RenderProperty.fromxml(self, xml)
 
         if success:
             self.packages = self.value.split("&#10;")
 
         return success
 
-    def has_package(self, name):
+    def has_package(self, name: str):
         """
         Check if package name exists in the LaTeX preamble.
 
         :type name: str
         :param name: Name of the package
         :rtype: boolean
         :returns: True if the package exists
@@ -2933,86 +3242,87 @@
             pn = package.split("{")[-1].split("}")[0]
 
             if pn == name:
                 return True
 
         return False
 
-    def append_package(self, name, options=""):
+    def append_package(self, name: str, options: str = ""):
         """
         Append a package in the LaTeX preamble.
 
         :type name: str
         :param name: Name of the package
         :type options: str
         :param options: Package's options
         :rtype: boolean
         :returns: True if package appending succeed
         """
 
-        ps = "\\" + "usepackage"
+        package_import = "\\" + "usepackage"
 
         if options:
-            ps += "[{}]".format(options)
+            package_import += f"[{options}]"
 
-        ps += "{" + name + "}"
+        package_import += "{" + name + "}"
 
-        if ps not in self.packages:
-            self.packages.append(ps)
+        if package_import not in self.packages:
+            self.packages.append(package_import)
 
         return True
 
     def toxml(self):
         xml = RenderProperty.toxml(self)
 
         # NOTE Override value attributes with packages
         xml.attrib["value"] = "&#10;".join(self.packages)
 
         return xml
 
 
 class WeldEntry(xmlc.PyScribusElement):
-
     def __init__(self):
         xmlc.PyScribusElement.__init__(self)
 
         self.target = False
         # TODO Savoir si c’est des Dim
         self.coords = {"x": 0, "y": 0}
 
-    def fromxml(self, xml):
-        if xml.tag == "WeldEntry":
-            wx,wy = xml.get("WX"),xml.get("WY")
+    def fromxml(self, xml: ET._Element):
+        if xml.tag != "WeldEntry":
+            return False
 
-            target = xml.get("Target")
-            if target is not None:
-                # TODO FIXME Il faudrait vérifier qu’un objet avec cet ID
-                # existe, mais généralement, il est à la suite, donc hors
-                # de ce qui constitue encore le document lors du parsing
-                self.target = target
+        wx, wy = xml.get("WX"), xml.get("WY")
 
-            return True
-        else:
-            return False
+        target = xml.get("Target")
+        if target is not None:
+            # TODO FIXME Il faudrait vérifier qu’un objet avec cet ID
+            # existe, mais généralement, il est à la suite, donc hors
+            # de ce qui constitue encore le document lors du parsing
+            self.target = target
+
+        return True
 
     def toxml(self):
         xml = ET.Element("WeldEntry")
         # TODO Savoir si c’est des Dim
         xml["WX"] = str(self.coords["x"])
         xml["WY"] = str(self.coords["y"])
 
         return xml
 
     def fromdefault(self):
         # TODO Savoir si c’est des Dim
         self.coords = {"x": 0, "y": 0}
         self.target = False
 
+
 # Paths =================================================================#
 
+
 class RectPath:
     """
     Path object for easiest manipulation of @path / @copath of rectangular
     shapes.
 
     Translate SVG path @d strings like :
 
@@ -3035,15 +3345,15 @@
 
             self.points.append(new_point)
 
             return True
 
         return False
 
-    def fromxml(self, xmlstring):
+    def fromxml(self, xmlstring: str):
         # NOTE
         # svg.path library use complex number, which I don’t know anything
         # about, but fortunately, I can check xmlstring for similarities
         # without having to do a PhD in maths.
 
         self.points = []
 
@@ -3051,25 +3361,24 @@
 
         self.raw = xmlstring
         self.svg_path = parsed_path
 
         for s in parsed_path._segments:
 
             if isinstance(s, svg.path.Move) or isinstance(s, svg.path.Line):
-                x = float(s.end.real)
-                y = float(s.end.imag)
+                x, y = float(s.end.real), float(s.end.imag)
                 px = PathPoint(x, y, fromsla=True)
                 self.points.append(px)
 
             if isinstance(s, svg.path.Close):
                 break
 
         return True
 
-    def frombox(self, box):
+    def frombox(self, box: dimensions.DimBox):
         """
         Set the points from a DimBox.
 
         :type box: pyscribus.dimensions.DimBox
         :param box: Box of a page, page object
         :rtype: boolean
         :returns: True if point setting succeed.
@@ -3078,22 +3387,22 @@
         # Reset of points list
         self.points = []
 
         # Getting width and height
         width = box.dims["width"].value
         height = box.dims["height"].value
 
-        #--- Making the four points of the rectangle ----------------
+        # Making the four points of the rectangle -------------------
 
-        tr = PathPoint(width, 0) # Top-right
-        br = PathPoint(width, height) # Bottom-right
-        bl = PathPoint(0, height) # Bottom-left
-        tl = PathPoint(0, 0) # Top-Left / Origin point
+        tr = PathPoint(width, 0)  # Top-right
+        br = PathPoint(width, height)  # Bottom-right
+        bl = PathPoint(0, height)  # Bottom-left
+        tl = PathPoint(0, 0)  # Top-Left / Origin point
 
-        #--- Adding the points clockwise ----------------------------
+        # Adding the points clockwise -------------------------------
 
         for point in [tr, br, bl, tl]:
             self.points.append(point)
 
         return True
 
     def toxml(self):
@@ -3113,16 +3422,16 @@
 
             if xml:
                 xml.append("Z")
 
             xml = " ".join(xml)
 
             return xml
-        else:
-            return False
+
+        return False
 
 
 class PathPoint:
     """
     Point of a rectangular path in @path/@copath page objects.
 
     :type x: float
@@ -3130,24 +3439,24 @@
     :type y: float
     :param y: y
     :type fromsla: boolean
     :param fromsla: Adjusts x and y value if these value are not immediately
         from SLA sources.
     """
 
-    def __init__(self, x=0, y=0, fromsla=False):
+    def __init__(self, x: float = 0, y: float = 0, fromsla: bool = False):
 
         if fromsla:
             self.x = x
             self.y = y
         else:
             self.x = self._round_coord(x)
             self.y = self._round_coord(y)
 
-    def _round_coord(self, n):
+    def _round_coord(self, n: float):
         """
         Round up the float n to the third decimal.
 
         :rtype: float
         """
 
         return math.ceil(n * 1000) / 1000
@@ -3155,23 +3464,21 @@
     def is_origin(self):
         """
         Is this path point the origin point ?
 
         :rtype: boolean
         """
 
-        if self.x == float(0) and self.y == float(0):
-            return True
-        else:
-            return False
+        return self.x == float(0) and self.y == float(0)
 
     def toxmlstr(self, move=False):
         """
         Returns SVG path @d command version of self.
 
+        :type move: boolean
         :rtype: str
         :returns: SVG path command
         """
 
         if float(self.x) == int(self.x):
             x = int(self.x)
         else:
@@ -3180,54 +3487,59 @@
         if float(self.y) == int(self.y):
             y = int(self.y)
         else:
             y = self.y
 
         if move:
             return "M{} {}".format(x, y)
-        else:
-            return "L{} {}".format(x, y)
+
+        return "L{} {}".format(x, y)
 
     def __repr__(self):
         return self.toxmlstr()
 
+
 # Variables globales 2 ==================================================#
 
+
 po_type_classes = {
     "image": ImageObject,
     "text": TextObject,
     "line": LineObject,
     "polygon": PolygonObject,
     "polyline": PolylineObject,
     "textonpath": TextOnPathObject,
     "render": RenderObject,
     "table": TableObject,
     "group": GroupObject,
-    "symbol": SymbolObject
+    "symbol": SymbolObject,
 }
 
 # Fonctions =============================================================#
 
-def adjust_path_d(d):
+
+def adjust_path_d(d: str):
     """
     Adjusts SVG path @d returned by svg.path Path.d() to what Scribus
     actually wrotes in SLA files.
     """
     d = d.replace("M 0,", "M0 ")
     d = d.replace("L 0,0 ", "L0 0 ")
     d = d.replace("L ", "L")
     d = d.replace(",", " ")
 
     return d
 
+
 # NOTE This function to avoid document module managing page objects
 # classes selections. We just need to modify po_type_xml, po_type_classes
 # and PageObject class to extend page object valid types.
 
-def new_from_type(ptype, sla_parent=False, doc_parent=False, **kwargs):
+
+def new_from_type(ptype: str, sla_parent=False, doc_parent=False, **kwargs):
     """
     Returns an instance of the correct class of page object according
     to ptype value.
 
     Although it is not a good idea for readability, you can make new
     page objects only with new_from_type() instead of instanciating
     the appropriate class of page object.
@@ -3283,17 +3595,17 @@
             po.sla_parent = sla_parent
 
         if doc_parent:
             po.doc_parent = doc_parent
 
         return po
 
-    else:
-        raise ValueError(
-            "Invalid ptype for pageobjects.from_pageobject_type(): {}".format(
-                ptype
-            )
+    raise ValueError(
+        "Invalid ptype for pageobjects.from_pageobject_type(): {}".format(
+            ptype
         )
+    )
 
     # -------------------------------------------------------------------------
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/pages.py` & `pyscribus-backported-0.3/pyscribus/model/pages.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,44 +17,42 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
 Classes for SLA Pages / Master pages.
 """
 
-# Scribus pages are  arranged in a vast scratch space,  where 1 unit ==
+# " Scribus pages are  arranged in a vast scratch space,  where 1 unit ==
 # 1/72 inch.  Positive x is to  the right, and positive  y is downward.
 # The positions, width and height in  the elements are in scratch space
 # coordinates  with the  exception  of POCOOR  and COCOOR  coordinates,
-# which are in the rotated and translated space of a PAGEOBJECT.
+# which are in the rotated and translated space of a PAGEOBJECT. "
 
 # Imports ===============================================================#
 
 # To avoid Sphinx complaints from methods annotations referencing same class
 from __future__ import annotations
 
 from typing import Optional, NoReturn, Literal
 
 from enum import Enum, IntEnum
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.logs as logs
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as mathc
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.logs as logs
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as mathc
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
-# Classes ===============================================================#
-
 PageOrientation = Literal["portrait", "landscape"]
 
 # FIXME Replace with Size(StrEnum) introduced in Python 3.11at some point
 # in which the values are separated by commas
 
 xml_size = {
     "A4": 'A4',
@@ -95,15 +93,15 @@
     effect_type_xml = {
         "none": "0",
         "masks": "1",
         "box": "2",
         "dissolve": "3",
         "glitter": "4",
         "break": "5",
-        "delete": "6"
+        "delete": "6",
     }
 
     # NOTE These directions are in the correct order, but Scribus only allows
     # the user to select "left-to-right" in its GUI.
     effect_direction_xml = {
         "left-to-right": "0",
         "top-to-bottom": "1",
@@ -129,31 +127,28 @@
 
         self.orientation = "portrait"
 
         self.paper_size = ""
 
         self.number = -1
 
-        #--- FIXME Tester pour savoir comment constituer les listes ------
+        # FIXME Tester pour savoir comment constituer les listes ---------
 
-        self.guides = {
-            "horizontal": [],
-            "vertical": []
-        }
+        self.guides = {"horizontal": [], "vertical": []}
 
         # ----------------------------------------------------------------
 
         # @LEFT - For multipage spreads, which page in the spread is the left most
         self.is_leftest = False
 
         # FIXME Not documented -------------------------------------------
 
         # PRESET="0"
 
-        #--- Auto guides -------------------------------------------------
+        # Auto guides ----------------------------------------------------
 
         self.auto_guides = {
             "lines": {
                 # @AGhorizontalAutoCount
                 "count": 0,
                 # @AGhorizontalAutoGap
                 "gap": dimensions.Dim(0),
@@ -175,41 +170,41 @@
                 "posx": dimensions.Dim(0),
                 "posy": dimensions.Dim(0),
                 "width": dimensions.Dim(0),
                 "height": dimensions.Dim(0),
             }
         }
 
-        #--- PDF effects -------------------------------------------------
+        # PDF effects ----------------------------------------------------
 
         self.effect = {
             # @pageEffectDuration
             "duration": dimensions.Dim(1, unit="sec"),
             # @pageViewDuration
             "view-duration": dimensions.Dim(1, unit="sec"),
             # @effectType
             "type": "none",
             # @Dm
             "mobile-lines": "horizontal",
             # @M
             "source": "internal",
             # @Di
-            "direction": "left-to-right"
+            "direction": "left-to-right",
         }
 
-        #--- FIXME Not documented ----------------------------------------
+        # FIXME Not documented -------------------------------------------
 
         # Same as DOCUMENT/PDF/Effekte (PDF display effects) attributes ?
 
-        #-----------------------------------------------------------------
+        # ----------------------------------------------------------------
 
         if kwargs:
             self._quick_setup(kwargs)
 
-    def _quick_setup(self, settings):
+    def _quick_setup(self, settings: dict) -> NoReturn:
         """
         Method for defining (master)page settings from class
         instanciation kwargs.
 
         :type settings: dict
         :param settings: Kwargs dictionnary
         """
@@ -218,32 +213,33 @@
             xmlc.PyScribusElement._quick_setup(self, settings)
 
             for setting_name, setting_value in settings.items():
 
                 # (Master) page box -------------------------------------------
 
                 if setting_name == "posx":
-                    # self.box.coords["top-left"][0].value = float(setting_value)
                     self.box.setx("top-left", float(setting_value))
 
                 if setting_name == "posy":
-                    # self.box.coords["top-left"][1].value = float(setting_value)
                     self.box.sety("top-left", float(setting_value))
 
                 if setting_name == "width":
                     self.box.dims["width"].value = float(setting_value)
 
                 if setting_name == "height":
                     self.box.dims["height"].value = float(setting_value)
 
                 # Borders -----------------------------------------------------
 
                 if setting_name in [
-                        "rightborder", "leftborder",
-                        "topborder", "bottomborder"]:
+                    "rightborder",
+                    "leftborder",
+                    "topborder",
+                    "bottomborder",
+                ]:
                     side = setting_name.split("border")[0]
                     self.borders[side].value = float(setting_value)
 
                 if setting_name == "borders":
                     # NOTE We solve borders settings like CSS margin property
                     # If only one value : same border for all sides
                     # If two values: vertical and horizontal borders
@@ -259,15 +255,15 @@
                                 self.borders[side].value = float(
                                     setting_value[0]
                                 )
 
                         if setting_len == 2:
                             sides = zip(
                                 [["top", "bottom"], ["right", "left"]],
-                                setting_value
+                                setting_value,
                             )
 
                             for side in sides:
                                 for s in side[0]:
                                     self.borders[s].value = float(side[1])
 
                         if setting_len == 3:
@@ -281,64 +277,61 @@
                             self.borders["bottom"].value = float(
                                 setting_value[2]
                             )
 
                         if setting_len == 4:
                             sides = zip(
                                 ["top", "right", "bottom", "left"],
-                                setting_value
+                                setting_value,
                             )
 
                             for side in sides:
                                 self.borders[side[0]].value = float(side[1])
 
                 # -------------------------------------------------------------
 
-    def set_orientation(self, orientation):
+    def set_orientation(self, orientation: PageOrientation) -> bool:
         """
         Set (master) page orientation.
 
-        :param orientation: "portrait" or "landscape"
         :type orientation: string
-        :returns: boolean
+        :param orientation: "portrait" or "landscape"
         :rtype: boolean
+        :returns: boolean
         """
 
         if orientation.lower() in PageAbstract.orientation_xml.keys():
             self.orientation = orientation.lower()
             # FIXME TODO Modify (master) page box accordingly
 
             return True
 
-        else:
-            raise ValueError(
-                "orientation parameter of set_orientation must be "\
-                "portrait' or 'landscape'"
-            )
+        raise ValueError(
+            "orientation parameter of set_orientation must be "
+            "portrait' or 'landscape'"
+        )
 
-    def fromxml(self, xml, master=False):
+    def fromxml(self, xml: ET.Element, master: bool = False) -> bool:
         """
         Set (master) page attributes according to LXML Element
 
+        :type xml: lxml.etree._Element
         :param xml: (Master) page source as XML element
-        :type xml: lxml._Element
-        :param master: If the page is a master page or not
         :type master: boolean
-        :returns: boolean
+        :param master: If the page is a master page or not
         :rtype: boolean
+        :returns: boolean
         """
-        if master:
-            tag = "MASTERPAGE"
-        else:
-            tag = "PAGE"
+
+        tag = {True: "MASTERPAGE", False: "PAGE"}[bool(master)]
 
         if xml.tag != tag:
             return False
 
-        #--- Box settings -------------------------------------
+        # Box settings ----------------------------------------
 
         posx = xml.get("PAGEXPOS")
         posy = xml.get("PAGEYPOS")
         dim_width = xml.get("PAGEWIDTH")
         dim_height = xml.get("PAGEHEIGHT")
 
         valid_box = 0
@@ -346,80 +339,82 @@
         for test in [posx, posy, dim_width, dim_height]:
             if test is not None:
                 valid_box += 1
 
         if valid_box == 4:
 
             self.box.set_box(
-                top_lx=posx, top_ly=posy,
-                width=dim_width, height=dim_height
+                top_lx=posx, top_ly=posy, width=dim_width, height=dim_height
             )
 
-        #--- Name / Master page name --------------------------
+        is_leftest = xml.get("LEFT")
+        if is_leftest is not None:
+            self.is_leftest = xmlc.num_to_bool(is_leftest)
+
+        # Name / Master page name -----------------------------
 
         self.name = xml.get("NAM")
         self.master_name = xml.get("MNAM")
 
-        is_leftest = xml.get("LEFT")
-        if is_leftest is not None:
-            self.is_leftest = xmlc.num_to_bool(is_leftest)
+        # Page number -----------------------------------------
 
         page_number = xml.get("NUM")
 
         if page_number is not None:
             # NOTE Page 0 is the first page so we adjust to a human
             # readable count
             self.number = int(page_number) + 1
 
-        #--- Paper size name and orientation ------------------
+        # Paper size name and orientation ---------------------
 
         paper_size = xml.get("Size")
         if paper_size is not None:
             self.paper_size = paper_size
 
         orientation = xml.get("Orientation")
         if orientation is not None:
 
-            for h,x in PageAbstract.orientation_xml.items():
+            for h, x in PageAbstract.orientation_xml.items():
                 if orientation == x:
                     self.orientation = h
                     break
 
-        #--- Borders ------------------------------------------
+        # Borders ---------------------------------------------
 
         for b in ["left", "top", "bottom", "right"]:
             att = "BORDER{}".format(b.upper())
             self.borders[b] = dimensions.Dim(float(xml.get(att)))
 
-        #--- Guides -------------------------------------------
+        # Guides ----------------------------------------------
 
         for guide_type in ["vertical", "horizontal"]:
 
             att_name = "{}Guides".format(guide_type.capitalize())
 
             att = xml.get(att_name)
-            if att is not None:
-                if att:
-                    # NOTE Example of att value : "42.5197 56.6929 "
 
-                    guides_list = []
-                    guides_values = [g.strip() for g in att.split(" ")]
+            if att is None:
+                continue
 
-                    for g in guides_values:
+            if not att:
+                continue
 
-                        if g:
+            # NOTE Example of att value : "42.5197 56.6929 "
 
-                            guides_list.append(
-                                dimensions.Dim(float(g))
-                            )
+            guides_list = []
+            guides_values = [g.strip() for g in att.split(" ")]
+
+            for g in guides_values:
 
-                    # self.guides[guide_type] = att
-                    self.guides[guide_type] = guides_list
+                if g:
+                    guides_list.append(dimensions.Dim(float(g)))
 
-        #--- Auto guides --------------------------------------
+            self.guides[guide_type] = guides_list
+
+        # Auto guides -----------------------------------------
 
         for case in [["lines", "horizontal"], ["columns", "vertical"]]:
             ag_count = xml.get("AG{}AutoCount".format(case[1]))
             ag_gap = xml.get("AG{}AutoGap".format(case[1]))
             ag_origin = xml.get("AG{}AutoRefer".format(case[1]))
 
             if ag_count is not None:
@@ -428,35 +423,43 @@
 
             if ag_gap is not None:
                 ag_gap = float(ag_gap)
                 self.auto_guides[case[0]]["gap"].value = ag_gap
 
             if ag_origin is not None:
 
-                for human,code in PageAbstract.autoguides_origin_xml.items():
+                for human, code in PageAbstract.autoguides_origin_xml.items():
                     if ag_origin == code:
                         self.auto_guides[case[0]]["origin"] = human
 
         ag_selection = xml.get("AGSelection")
         if ag_selection is not None:
             agx, agy, agw, agh = [float(dim) for dim in ag_selection.split()]
 
             self.auto_guides["selection"]["posx"].value = agx
             self.auto_guides["selection"]["posy"].value = agy
             self.auto_guides["selection"]["width"].value = agw
             self.auto_guides["selection"]["height"].value = agh
 
-        #--- PDF effects -------------------------------------------------
+        # PDF effects ----------------------------------------------------
 
         duration = xml.get("pageEffectDuration")
         if duration is not None:
+            # FIXME Maybe a hack
+            if duration == "None":
+                duration = 1
+
             self.effect["duration"].value = int(duration)
 
         view_duration = xml.get("pageViewDuration")
         if view_duration is not None:
+            # FIXME Maybe a hack
+            if view_duration == "None":
+                view_duration = 1
+
             self.effect["view-duration"].value = int(view_duration)
 
         effect_type = xml.get("effectType")
         if effect_type is not None:
             for human, code in PageAbstract.effect_type_xml.items():
                 if effect_type == code:
                     self.effect["type"] = human
@@ -479,36 +482,33 @@
         effect_direction = xml.get("Di")
         if effect_direction is not None:
             for human, code in PageAbstract.effect_direction_xml.items():
                 if effect_direction == code:
                     self.effect["direction"] = human
                     break
 
-        #--- FIXME This records undocumented attributes -------
+        # FIXME This records undocumented attributes ----------
 
         self.undocumented = xmlc.all_undocumented_to_python(xml)
 
         return True
 
-    def toxml(self, master=False):
+    def toxml(self, master: bool = False) -> ET.Element:
         """
         Returns (master) page as LXML Element
 
-        :param master: If the page is a master page or not
         :type master: bool
+        :param master: If the page is a master page or not
+        :rtype: lxml.etree._Element
         :returns: xml
-        :rtype: lxml._Element
         """
 
-        #--- Appropriate tag if master page or page -----------
+        # Appropriate tag if master page or page --------------
 
-        if master:
-            tag = "MASTERPAGE"
-        else:
-            tag = "PAGE"
+        tag = {True: "MASTERPAGE", False: "PAGE"}[bool(master)]
 
         xml = ET.Element(tag)
 
         # Position and dimensions -----------------------------
 
         xml.attrib["PAGEXPOS"] = self.box.coords["top-left"][0].toxmlstr()
         xml.attrib["PAGEYPOS"] = self.box.coords["top-left"][1].toxmlstr()
@@ -520,67 +520,72 @@
 
         # Borders ---------------------------------------------
 
         for b in ["left", "right", "top", "bottom"]:
             att = "BORDER{}".format(b.upper())
             xml.attrib[att] = self.borders[b].toxmlstr(True)
 
-         #--- Page number --------------------------------------
+        # Page number -----------------------------------------
 
         if self.number > 0:
             # NOTE Page 0 is the first page so we adjust back
             # from human counting to computer counting
             xml.attrib["NUM"] = str(self.number - 1)
 
-        #--- Page name and master page name -------------------
+        # Page name and master page name ----------------------
 
         xml.attrib["NAM"] = self.name
         xml.attrib["MNAM"] = self.master_name
 
-        #--- (Master) page size name and orientation ----------
+        # (Master) page size name and orientation -------------
 
         xml.attrib["Size"] = self.paper_size
-        xml.attrib["Orientation"] = PageAbstract.orientation_xml[self.orientation]
+        xml.attrib["Orientation"] = PageAbstract.orientation_xml[
+            self.orientation
+        ]
 
-        #--- Guides -------------------------------------------
+        # Guides ----------------------------------------------
 
-        for guide_type,guides in self.guides.items():
+        for guide_type, guides in self.guides.items():
             att_name = "{}Guides".format(guide_type.capitalize())
 
             # NOTE Example of att value : "42.5197 56.6929 "
 
             guides_str = " ".join([g.toxmlstr(True) for g in guides])
 
             if guides_str.strip():
                 xml.attrib[att_name] = guides_str
             else:
                 xml.attrib[att_name] = ""
 
-        #--- Auto guides --------------------------------------
+        # Auto guides -----------------------------------------
 
-        for case in [["lines", "horizontal"], ["columns", "vertical"]]:
+        for items, orientation in [
+                ["lines", "horizontal"], ["columns", "vertical"]]:
             # Page lines / columns count
             # AGhorizontalAutoCount="2"
             # AGverticalAutoCount="3"
-            count_att = "AG{}AutoCount".format(case[1])
+            count_att = f"AG{orientation}AutoCount"
 
             # Page lines / columns gap (gouttière)
             # AGhorizontalAutoGap="17.007874015748"
             # AGverticalAutoGap="22.6771653543307"
-            gap_att = "AG{}AutoGap".format(case[1])
+            gap_att = f"AG{orientation}AutoGap"
 
             # Page lines / columns origin
             # 0 = Page 1 = Margins
             # AGhorizontalAutoRefer="0"
             # AGverticalAutoRefer="0"
-            orig_att = "AG{}AutoRefer".format(case[1])
+            orig_att = f"AG{orientation}AutoRefer"
 
-            xml.attrib[count_att] = str(self.auto_guides[case[0]]["count"])
-            xml.attrib[gap_att] = self.auto_guides[case[0]]["gap"].toxmlstr()
-            xml.attrib[orig_att] = PageAbstract.autoguides_origin_xml[self.auto_guides[case[0]]["origin"]]
+            xml.attrib[count_att] = str(self.auto_guides[items]["count"])
+            xml.attrib[gap_att] = self.auto_guides[items]["gap"].toxmlstr(True)
+            xml.attrib[orig_att] = PageAbstract.autoguides_origin_xml[
+                self.auto_guides[items]["origin"]
+            ]
 
         # Check if auto guides if different from default value
         # If the X, Y, W, H of the selection are 0, then it is not custom
 
         custom_ag_selection = [
             dim.value
             for dim in self.auto_guides["selection"].values()
@@ -600,41 +605,49 @@
             ag_selection = "0 0 0 0"
 
         xml.attrib["AGSelection"] = ag_selection
 
         # --- PDF effects -------------------------------------------------
 
         xml.attrib["pageEffectDuration"] = self.effect["duration"].toxmlstr()
-        xml.attrib["pageViewDuration"] = self.effect["view-duration"].toxmlstr()
-        xml.attrib["effectType"] = PageAbstract.effect_type_xml[self.effect["type"]]
-        xml.attrib["Dm"] = PageAbstract.effect_mobile_line_xml[self.effect["mobile-lines"]]
+        xml.attrib["pageViewDuration"] = self.effect[
+            "view-duration"
+        ].toxmlstr()
+        xml.attrib["effectType"] = PageAbstract.effect_type_xml[
+            self.effect["type"]
+        ]
+        xml.attrib["Dm"] = PageAbstract.effect_mobile_line_xml[
+            self.effect["mobile-lines"]
+        ]
         xml.attrib["M"] = PageAbstract.effect_source_xml[self.effect["source"]]
-        xml.attrib["Di"] = PageAbstract.effect_direction_xml[self.effect["direction"]]
+        xml.attrib["Di"] = PageAbstract.effect_direction_xml[
+            self.effect["direction"]
+        ]
 
-        #--- FIXME This exports undocumented attributes -------
+        # --- FIXME This exports undocumented attributes -------
 
         try:
             xml, undoc_attribs = xmlc.all_undocumented_to_xml(
                 xml, self.undocumented, True, tag, logger=logs.getLogger()
             )
 
         except AttributeError:
             # NOTE If fromxml was not used
             pass
 
         return xml
 
-    def fromdefault(self, master=False, default=False):
+    def fromdefault(self, master: bool = False, default: Optional[str]=False) -> NoReturn:
         """
         Set (master) page attributes according to known defaults.
 
-        :param master: If the page is a master page or not
-        :param default: Name of the set of defaults ("a4", "letter")
         :type master: bool
+        :param master: If the page is a master page or not
         :type default: str
+        :param default: Name of the set of defaults ("a4", "letter")
         """
 
         for border in self.borders.values():
             border.value = 40
 
         dim_default = "a4"
 
@@ -646,17 +659,18 @@
 
         self.master_name = "Normal"
 
         self.box.dims["width"].fromdefault("{}-width".format(dim_default))
         self.box.dims["height"].fromdefault("{}-height".format(dim_default))
 
         self.box.set_box(
-            top_lx=100.0, top_ly=20.0,
+            top_lx=100.0,
+            top_ly=20.0,
             width=self.box.dims["width"].value,
-            height=self.box.dims["height"].value
+            height=self.box.dims["height"].value,
         )
 
 
 class Page(PageAbstract):
     """
     Page in SLA
 
@@ -716,51 +730,51 @@
     +--------------+---------------------------------+------------+
     """
 
     def __init__(self, **kwargs):
         PageAbstract.__init__(self)
         PageAbstract._quick_setup(self, kwargs)
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         Returns page as LXML Element
 
         :returns: xml
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         """
         return PageAbstract.toxml(self, False)
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         Set page attributes according to LXML Element
 
+        :type xml: lxml.etree._Element
         :param xml: Page source as XML element
-        :type xml: lxml._Element
-        :returns: bool
         :rtype: bool
+        :returns: bool
         """
         return PageAbstract.fromxml(self, xml, False)
 
-    def fromdefault(self, default=False):
+    def fromdefault(self, default: Optional[str]=False) -> NoReturn:
         """
         Set page attributes according to known defaults.
 
-        :param default: Name of the set of defaults ("a4", "letter")
         :type default: str
+        :param default: Name of the set of defaults ("a4", "letter")
         """
         PageAbstract.fromdefault(self, False, default)
 
-    def set_orientation(self, orientation):
+    def set_orientation(self, orientation: PageOrientation) -> bool:
         """
         Set page orientation.
 
-        :param orientation: "portrait" or "landscape"
         :type orientation: str
-        :returns: bool
+        :param orientation: "portrait" or "landscape"
         :rtype: bool
+        :returns: bool
         """
         return PageAbstract.set_orientation(self, orientation)
 
 
 class MasterPage(PageAbstract):
     """
     Master page in SLA
@@ -821,201 +835,208 @@
     +--------------+---------------------------------+------------+
     """
 
     def __init__(self, **kwargs):
         PageAbstract.__init__(self)
         PageAbstract._quick_setup(self, kwargs)
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         Returns master page object as LXML Element
 
         :returns: xml
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         """
         return PageAbstract.toxml(self, True)
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         Set master page attributes according to LXML Element
 
+        :type xml: lxml.etree._Element
         :param xml: Master page source as XML element
-        :type xml: lxml._Element
-        :returns: bool
         :rtype: bool
+        :returns: bool
         """
         return PageAbstract.fromxml(self, xml, True)
 
-    def fromdefault(self, default=False):
+    def fromdefault(self, default: Optional[str]=False) -> NoReturn:
         """
         Set master page attributes according to known defaults.
 
         :param default: Name of the set of defaults ("a4", "letter")
         :type default: str
         """
         PageAbstract.fromdefault(self, True, default)
 
-    def set_orientation(self, orientation):
+    def set_orientation(self, orientation: PageOrientation):
         """
         Set master page orientation.
 
-        :param orientation: "portrait" or "landscape"
         :type orientation: str
-        :returns: bool
+        :param orientation: "portrait" or "landscape"
         :rtype: bool
+        :returns: bool
         """
         return PageAbstract.set_orientation(self, orientation)
 
 
 class PageSet(xmlc.PyScribusElement):
     """
     Page set object.
 
     DOCUMENT/PageSets/Set
     """
 
     DEFAULTS = {
         "Single Page": {"first": 0, "rows": 1, "columns": 1, "names": []},
         "Facing Pages": {
-            "first": 1, "rows": 1, "columns": 2,
-            "names": ["Left Page", "Right Page"]
+            "first": 1,
+            "rows": 1,
+            "columns": 2,
+            "names": ["Left Page", "Right Page"],
         },
         "3-Fold": {
-            "first": 0, "rows": 1, "columns": 3,
-            "names": ["Left Page", "Middle", "Right Page"]
+            "first": 0,
+            "rows": 1,
+            "columns": 3,
+            "names": ["Left Page", "Middle", "Right Page"],
         },
         "4-Fold": {
-            "first": 0, "rows": 1, "columns": 4,
+            "first": 0,
+            "rows": 1,
+            "columns": 4,
             "names": [
-                "Left Page", "Middle Left", "Middle Right", "Right Page"
-            ]
-        }
+                "Left Page",
+                "Middle Left",
+                "Middle Right",
+                "Right Page",
+            ],
+        },
     }
 
     def __init__(self):
         xmlc.PyScribusElement.__init__(self)
 
         self.pyscribus_defaults = [k for k in PageSet.DEFAULTS.keys()]
 
         self.name = ""
         self.first_page = 0
         self.rows = 0
         self.columns = 0
         self.pages = []
 
-    def fromdefault(self, default):
-        """
-        """
+    def fromdefault(self, default: str) -> bool:
 
         if default in self.pyscribus_defaults:
 
             accurate = PageSet.DEFAULTS[default]
 
             self.name = default
             self.rows = accurate["rows"]
             self.pages = accurate["names"]
             self.columns = accurate["columns"]
             self.first_page = accurate["first"]
 
             return True
-        else:
-            return False
 
-    def toxml(self):
+        return False
+
+    def toxml(self) -> ET.Element:
         """
+        :rtype: lxml.etree._Element
         :returns: xml
-        :rtype: lxml._Element
         """
 
         xml = ET.Element("Set")
 
-        #------------------------------------------------------
+        # -----------------------------------------------------
 
         xml.attrib["Name"] = self.name
         xml.attrib["FirstPage"] = str(self.first_page)
         xml.attrib["Rows"] = str(self.rows)
         xml.attrib["Columns"] = str(self.columns)
 
-        #--- Page names ---------------------------------------
+        # Page names ------------------------------------------
 
         if self.pages:
 
-            for n in self.pages:
+            for page_name in self.pages:
 
                 pnx = ET.Element("PageNames")
-                pnx.attrib["Name"] = n
+                pnx.attrib["Name"] = page_name
                 xml.append(pnx)
 
-        #--- FIXME This exports undocumented attributes -------
+        # FIXME This exports undocumented attributes ----------
 
         try:
             xml = xmlc.undocumented_to_xml(xml, self.undocumented, no_none=True)
         except AttributeError:
             # NOTE If fromxml was not used
             pass
 
         return xml
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element) -> bool:
         """
+        :type xml: lxml.etree._Element
         :param xml: Page set as XML element
-        :type xml: lxml._Element
-        :returns: bool
         :rtype: bool
+        :returns: bool
         """
 
-        if xml.tag == "Set":
+        if xml.tag != "Set":
             return False
 
-        #------------------------------------------------------
+        # -----------------------------------------------------
 
         name = xml.get("Name")
         if name is not None:
             self.name = name
 
-        #------------------------------------------------------
+        # -----------------------------------------------------
 
         for att in ["FirstPage", "Rows", "Columns"]:
 
             atx = xml.get(att)
-            if atx is not None:
 
-                try:
-                    atx = int(atx)
-                except ValueError:
-                    raise exceptions.InsaneSLAValue(
-                        "Page set @{} must be a number.".format(
-                            atx
-                        )
-                    )
+            if atx is None:
+                continue
+
+            try:
+                atx = int(atx)
+            except ValueError:
+                raise exceptions.InsaneSLAValue(
+                    "Page set @{} must be a number.".format(atx)
+                )
 
         first = xml.get("FirstPage")
         if first is not None:
             self.first_page = int(first)
 
         rows = xml.get("Rows")
         if rows is not None:
             self.rows = int(rows)
 
         columns = xml.get("Columns")
         if columns is not None:
             self.columns = int(columns)
 
-        #--- Page names ---------------------------------------
+        # Page names ------------------------------------------
 
         for child in xml:
             if child.tag == "PageNames":
-                n = child.get("Name")
+                page_name = child.get("Name")
 
-                if n not in self.pages:
-                    self.pages.append(n)
+                if page_name not in self.pages:
+                    self.pages.append(page_name)
 
-        #--- FIXME This records undocumented attributes -------
+        # FIXME This records undocumented attributes ----------
 
-        self.undocumented = undocumented_to_python(
+        self.undocumented = xmlc.undocumented_to_python(
             xml, ["GapBelow", "GapHorizontal", "GapVertical"]
         )
 
         return True
 
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/__init__.py` & `pyscribus-backported-0.3/pyscribus/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """
-PyScribus submodule for paper sizes
+PyScribus
+
+SLA file model
 """
 
+from pyscribus.model.sla import SLA
+
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
-__version__ = "0.1"
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/afnor.py` & `pyscribus-backported-0.3/pyscribus/model/papers/afnor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,118 +30,143 @@
 Petit Aigle, Grand Aigle, Grand Monde, Univers
 
 For more common and international paper sizes, see iso216paper module.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
+
 class Cloche(FloatEnum):
     WIDTH = 300 / PICA_TO_MM
     HEIGHT = 400 / PICA_TO_MM
 
+
 class Pot(FloatEnum):
     """
     Pot paper size. Same as Ecolier.
     """
 
     WIDTH = 310 / PICA_TO_MM
     HEIGHT = 400 / PICA_TO_MM
 
+
 class Ecolier(FloatEnum):
     """
     Ecolier paper size. Same as Pot.
     """
 
     WIDTH = 310 / PICA_TO_MM
     HEIGHT = 400 / PICA_TO_MM
 
+
 class Telliere(FloatEnum):
     WIDTH = 340 / PICA_TO_MM
     HEIGHT = 440 / PICA_TO_MM
 
+
 class CouronneEcriture(FloatEnum):
     WIDTH = 360 / PICA_TO_MM
     HEIGHT = 460 / PICA_TO_MM
 
+
 class CouronneEdition(FloatEnum):
     WIDTH = 370 / PICA_TO_MM
     HEIGHT = 470 / PICA_TO_MM
 
+
 class Roberto(FloatEnum):
     WIDTH = 390 / PICA_TO_MM
     HEIGHT = 500 / PICA_TO_MM
 
+
 class Ecu(FloatEnum):
     WIDTH = 400 / PICA_TO_MM
     HEIGHT = 520 / PICA_TO_MM
 
+
 class Coquille(FloatEnum):
     WIDTH = 440 / PICA_TO_MM
     HEIGHT = 560 / PICA_TO_MM
 
+
 class Carre(FloatEnum):
     WIDTH = 450 / PICA_TO_MM
     HEIGHT = 560 / PICA_TO_MM
 
+
 class Cavalier(FloatEnum):
     WIDTH = 460 / PICA_TO_MM
     HEIGHT = 620 / PICA_TO_MM
 
+
 class Raisin(FloatEnum):
     WIDTH = 500 / PICA_TO_MM
     HEIGHT = 650 / PICA_TO_MM
 
+
 class DemiRaisin(FloatEnum):
     WIDTH = 325 / PICA_TO_MM
     HEIGHT = 500 / PICA_TO_MM
 
+
 class DoubleRaisin(FloatEnum):
     WIDTH = 650 / PICA_TO_MM
     HEIGHT = 1000 / PICA_TO_MM
 
+
 class Jesus(FloatEnum):
     WIDTH = 560 / PICA_TO_MM
     HEIGHT = 720 / PICA_TO_MM
 
+
 class PetitJesus(FloatEnum):
     WIDTH = 550 / PICA_TO_MM
     HEIGHT = 700 / PICA_TO_MM
 
+
 class GrandJesus(FloatEnum):
     WIDTH = 560 / PICA_TO_MM
     HEIGHT = 760 / PICA_TO_MM
 
+
 class Soleil(FloatEnum):
     WIDTH = 600 / PICA_TO_MM
     HEIGHT = 800 / PICA_TO_MM
 
+
 class ColombierAffiche(FloatEnum):
     WIDTH = 600 / PICA_TO_MM
     HEIGHT = 800 / PICA_TO_MM
 
+
 class ColombierCommercial(FloatEnum):
     WIDTH = 630 / PICA_TO_MM
     HEIGHT = 900 / PICA_TO_MM
 
+
 class PetitAigle(FloatEnum):
     WIDTH = 700 / PICA_TO_MM
     HEIGHT = 940 / PICA_TO_MM
 
+
 class GrandAigle(FloatEnum):
     WIDTH = 750 / PICA_TO_MM
     HEIGHT = 1060 / PICA_TO_MM
 
+
 class GrandMonde(FloatEnum):
     WIDTH = 900 / PICA_TO_MM
     HEIGHT = 1260 / PICA_TO_MM
 
+
 class Univers(FloatEnum):
     WIDTH = 1000 / PICA_TO_MM
     HEIGHT = 1300 / PICA_TO_MM
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/ansi.py` & `pyscribus-backported-0.3/pyscribus/model/papers/ansi.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,55 +23,62 @@
 ANSI A to E formats.
 
 Yes, this is the module for Letter paper sizes, as Letter = ANSI A.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM, INCH_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM, INCH_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
 # NOTE Dimensions are first converted into milimeters
 #      because inches makes no sense to my european being.
 
+
 class Letter(FloatEnum):
     """Letter format. Same as ANSI A."""
 
     WIDTH = (8.5 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (11 * INCH_TO_MM) / PICA_TO_MM
 
+
 class A(FloatEnum):
     """ANSI A."""
 
     WIDTH = (8.5 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (11 * INCH_TO_MM) / PICA_TO_MM
 
+
 class B(FloatEnum):
     """ANSI B."""
 
     WIDTH = (11 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (17 * INCH_TO_MM) / PICA_TO_MM
 
+
 class C(FloatEnum):
     """ANSI C."""
 
     WIDTH = (17 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (22 * INCH_TO_MM) / PICA_TO_MM
 
+
 class D(FloatEnum):
     """ANSI D."""
 
     WIDTH = (22 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (34 * INCH_TO_MM) / PICA_TO_MM
 
+
 class E(FloatEnum):
     """ANSI E."""
 
     WIDTH = (34 * INCH_TO_MM) / PICA_TO_MM
     HEIGHT = (44 * INCH_TO_MM) / PICA_TO_MM
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/iso216.py` & `pyscribus-backported-0.3/pyscribus/model/papers/iso216.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,108 +26,132 @@
 
 See iso269paper module for C format.
 See iso217paper module for RA, SRA formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
 # A format --------------------------------------
 
+
 class A0(FloatEnum):
     WIDTH = 841 / PICA_TO_MM
     HEIGHT = 1189 / PICA_TO_MM
 
+
 class A1(FloatEnum):
     WIDTH = 594 / PICA_TO_MM
     HEIGHT = 841 / PICA_TO_MM
 
+
 class A2(FloatEnum):
     WIDTH = 420 / PICA_TO_MM
     HEIGHT = 594 / PICA_TO_MM
 
+
 class A3(FloatEnum):
     WIDTH = 297 / PICA_TO_MM
     HEIGHT = 420 / PICA_TO_MM
 
+
 class A4(FloatEnum):
     WIDTH = 210 / PICA_TO_MM
     HEIGHT = 297 / PICA_TO_MM
 
+
 class A5(FloatEnum):
     WIDTH = 148 / PICA_TO_MM
     HEIGHT = 210 / PICA_TO_MM
 
+
 class A6(FloatEnum):
     WIDTH = 105 / PICA_TO_MM
     HEIGHT = 148 / PICA_TO_MM
 
+
 class A7(FloatEnum):
     WIDTH = 74 / PICA_TO_MM
     HEIGHT = 105 / PICA_TO_MM
 
+
 class A8(FloatEnum):
     WIDTH = 52 / PICA_TO_MM
     HEIGHT = 74 / PICA_TO_MM
 
+
 class A9(FloatEnum):
     WIDTH = 37 / PICA_TO_MM
     HEIGHT = 52 / PICA_TO_MM
 
+
 class A10(FloatEnum):
     WIDTH = 26 / PICA_TO_MM
     HEIGHT = 37 / PICA_TO_MM
 
+
 # B format --------------------------------------
 
+
 class B0(FloatEnum):
     WIDTH = 1000 / PICA_TO_MM
     HEIGHT = 1414 / PICA_TO_MM
 
+
 class B1(FloatEnum):
     WIDTH = 707 / PICA_TO_MM
     HEIGHT = 1000 / PICA_TO_MM
 
+
 class B2(FloatEnum):
     WIDTH = 500 / PICA_TO_MM
     HEIGHT = 707 / PICA_TO_MM
 
+
 class B3(FloatEnum):
     WIDTH = 353 / PICA_TO_MM
     HEIGHT = 500 / PICA_TO_MM
 
+
 class B4(FloatEnum):
     WIDTH = 250 / PICA_TO_MM
     HEIGHT = 353 / PICA_TO_MM
 
+
 class B5(FloatEnum):
     WIDTH = 176 / PICA_TO_MM
     HEIGHT = 250 / PICA_TO_MM
 
+
 class B6(FloatEnum):
     WIDTH = 125 / PICA_TO_MM
     HEIGHT = 176 / PICA_TO_MM
 
+
 class B7(FloatEnum):
     WIDTH = 88 / PICA_TO_MM
     HEIGHT = 125 / PICA_TO_MM
 
+
 class B8(FloatEnum):
     WIDTH = 62 / PICA_TO_MM
     HEIGHT = 88 / PICA_TO_MM
 
+
 class B9(FloatEnum):
     WIDTH = 44 / PICA_TO_MM
     HEIGHT = 62 / PICA_TO_MM
 
+
 class B10(FloatEnum):
     WIDTH = 31 / PICA_TO_MM
     HEIGHT = 44 / PICA_TO_MM
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/iso217.py` & `pyscribus-backported-0.3/pyscribus/model/papers/iso217.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 See iso216paper module for A, B formats.
 See iso269paper module for C format (including DL).
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Raw A -----------------------------------------
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/iso269.py` & `pyscribus-backported-0.3/pyscribus/model/papers/iso269.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,66 +24,80 @@
 
 See iso216paper module for A, B formats.
 See iso217paper module for RA, SRA formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
+
 class C0(FloatEnum):
     WIDTH = 917 / PICA_TO_MM
     HEIGHT = 1297 / PICA_TO_MM
 
+
 class C1(FloatEnum):
     WIDTH = 648 / PICA_TO_MM
     HEIGHT = 917 / PICA_TO_MM
 
+
 class C2(FloatEnum):
     WIDTH = 458 / PICA_TO_MM
     HEIGHT = 648 / PICA_TO_MM
 
+
 class C3(FloatEnum):
     WIDTH = 324 / PICA_TO_MM
     HEIGHT = 458 / PICA_TO_MM
 
+
 class C4(FloatEnum):
     WIDTH = 229 / PICA_TO_MM
     HEIGHT = 324 / PICA_TO_MM
 
+
 class C5(FloatEnum):
     WIDTH = 162 / PICA_TO_MM
     HEIGHT = 229 / PICA_TO_MM
 
+
 class C6(FloatEnum):
     WIDTH = 114 / PICA_TO_MM
     HEIGHT = 162 / PICA_TO_MM
 
+
 class C76(FloatEnum):
     WIDTH = 81 / PICA_TO_MM
     HEIGHT = 162 / PICA_TO_MM
 
+
 class C7(FloatEnum):
     WIDTH = 81 / PICA_TO_MM
     HEIGHT = 114 / PICA_TO_MM
 
+
 class C8(FloatEnum):
     WIDTH = 57 / PICA_TO_MM
     HEIGHT = 81 / PICA_TO_MM
 
+
 class C9(FloatEnum):
     WIDTH = 40 / PICA_TO_MM
     HEIGHT = 57 / PICA_TO_MM
 
+
 class C10(FloatEnum):
     WIDTH = 28 / PICA_TO_MM
     HEIGHT = 40 / PICA_TO_MM
 
+
 class DL(FloatEnum):
     WIDTH = 110 / PICA_TO_MM
     HEIGHT = 220 / PICA_TO_MM
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/papers/newspaper.py` & `pyscribus-backported-0.3/pyscribus/model/papers/newspaper.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,34 +21,40 @@
 Often used newspapers sizes.
 
 Berliner, Belgian, Tabloid, Broadsheet formats.
 """
 
 # Imports ===============================================================#
 
-from pyscribus.common.math import FloatEnum, PICA_TO_MM
+from pyscribus.model.common.math import FloatEnum, PICA_TO_MM
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
+
 class Berliner(FloatEnum):
     WIDTH = 320 / PICA_TO_MM
     HEIGHT = 470 / PICA_TO_MM
 
+
 class Broadsheet(FloatEnum):
     WIDTH = 410 / PICA_TO_MM
     HEIGHT = 575 / PICA_TO_MM
 
+
 class Belgian(FloatEnum):
     WIDTH = 365 / PICA_TO_MM
     HEIGHT = 520 / PICA_TO_MM
 
+
 class Belgian50(FloatEnum):
     WIDTH = 370 / PICA_TO_MM
     HEIGHT = 500 / PICA_TO_MM
 
+
 class Tabloid(FloatEnum):
     WIDTH = 290 / PICA_TO_MM
     HEIGHT = 410 / PICA_TO_MM
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/patterns.py` & `pyscribus-backported-0.3/pyscribus/model/patterns.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,29 +19,33 @@
 
 """
 PyScribus classes for patterns.
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
-import pyscribus.pageobjects as pageobjects
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
+import pyscribus.model.pageobjects as pageobjects
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class Pattern(PyScribusElement):
     """
     Pattern in SLA (Pattern)
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
@@ -62,77 +66,68 @@
 
         self.sla_parent = sla_parent
         self.doc_parent = doc_parent
 
         # NOTE We do not set a dimensions.DimBox because patterns is not meant
         # to be used directly on the page
 
-        self.dims = {
-            "width": None,
-            "height": None
-        }
+        self.dims = {"width": None, "height": None}
 
-        self.scale = {
-            "x": None,
-            "y": None
-        }
+        self.scale = {"x": None, "y": None}
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         """
 
-        if xml.tag == "Pattern":
-
-            name = xml.get("Name")
-            if name is not None:
-                self.name = name
+        if xml.tag != "Pattern":
+            return False
 
-            for dim in ["width", "height"]:
+        name = xml.get("Name")
+        if name is not None:
+            self.name = name
 
-                att = xml.get(dim)
-                if att is not None:
-                    self.dims[dim] = dimensions.Dim(float(att))
+        for dim in ["width", "height"]:
 
-            for scale in ["x", "x"]:
-                att_name = "scale{}".format(scale.upper())
+            att = xml.get(dim)
+            if att is not None:
+                self.dims[dim] = dimensions.Dim(float(att))
 
-                att = xml.get(att_name)
-                if att is not None:
-                    self.scale[scale] = dimensions.Dim(float(att), unit="pcdecim")
+        for scale in ["x", "x"]:
+            att_name = "scale{}".format(scale.upper())
 
-            # TODO FIXME xoffset yoffset
+            att = xml.get(att_name)
+            if att is not None:
+                self.scale[scale] = dimensions.Dim(float(att), unit="pcdecim")
 
-            for element in xml:
+        # TODO FIXME xoffset yoffset
 
-                if element.tag == "PatternItem":
-                    pie = PatternItem(self.sla_parent, self.doc_parent)
+        for element in xml:
 
-                    success = pie.fromxml(element)
-                    if success:
-                        self.items.append(pie)
+            if element.tag == "PatternItem":
+                pie = PatternItem(self.sla_parent, self.doc_parent)
 
-            return True
+                success = pie.fromxml(element)
+                if success:
+                    self.items.append(pie)
 
-        return False
+        return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         """
 
         xml = ET.Element("Pattern")
 
         if self.name is not None:
             xml.attrib["Name"] = self.name
 
         for dim in ["width", "height"]:
             if self.dims[dim] is None:
                 raise ValueError(
-                    "Pattern {} must have a(n) {}.".format(
-                        self.name, dim
-                    )
+                    "Pattern {} must have a(n) {}.".format(self.name, dim)
                 )
             else:
                 xml.attrib[dim] = self.dims[dim].toxmlstr()
 
         for scale in ["x", "y"]:
             att_name = "scale{}".format(scale.upper())
 
@@ -150,40 +145,42 @@
         return xml
 
 
 class PatternItem(pageobjects.PageObject):
     """
     Pattern item in SLA (Pattern/PatternItem)
 
-    (Pattern items are encoded as polygon page objects with a different XML tag)
+    (Pattern items are encoded as polygon page objects with a different XML
+    tag)
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
     :param doc_parent: SLA DOCUMENT instance
     """
 
     # <PatternItem XPOS="0.187499995780351" YPOS="0.187499995780351" OwnPage="-1" ItemID="204434288" PTYPE="6" WIDTH="6.55552657556513" HEIGHT="4.82126570393049" FRTYPE="3" CLIPEDIT="1" PWIDTH="0.374999991560701" PCOLOR="FromSVG#de4344" PCOLOR2="FromSVG#de4344" PLINEART="1" PLINEJOIN="128" ANNAME=" path861" TEXTFLOWMODE="1" path="M3.6e-7 4.44089e-16 L6.55553 2.41063 L0 4.82127 C1.0473 3.39803 1.04126 1.45079 3.6e-7 0 L3.6e-7 4.44089e-16 Z" copath="M3.6e-7 4.44089e-16 L6.55553 2.41063 L0 4.82127 C1.0473 3.39803 1.04126 1.45079 3.6e-7 0 L3.6e-7 4.44089e-16 Z" gXpos="0.187499995780351" gYpos="0.187499995780351" gWidth="6.93052656712583" gHeight="5.19626569549119" LAYER="0"/>
 
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
-        pageobjects.PageObject.__init__(self, "polygon", sla_parent, doc_parent)
+        pageobjects.PageObject.__init__(
+            self, "polygon", sla_parent, doc_parent
+        )
         pageobjects.PageObject._quick_setup(self, kwargs)
 
-    def fromxml(self, xml):
-        """
-        """
+    def fromxml(self, xml: ET.Element) -> bool:
 
         success = pageobjects.PageObject.fromxml(
             self, xml, arbitrary_tag="PatternItem"
         )
 
         return success
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         """
 
         xml = pageobjects.PageObject.toxml(arbitrary_tag="PatternItem")
 
         return xml
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/stories.py` & `pyscribus-backported-0.3/pyscribus/model/stories.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,82 +29,138 @@
 import copy
 
 from typing import Union, NoReturn, List
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.exceptions as exceptions
-import pyscribus.marks as marks
-import pyscribus.notes as notes
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.marks as marks
+import pyscribus.model.notes as notes
 
-from pyscribus.common.xml import *
+from pyscribus.model.common.xml import *
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class StoryEnding(PyScribusElement):
     """
     Ending marker in Scribus stories (trail)
     """
 
     def __init__(self, **kwargs):
         super().__init__()
         self.alignment = None
         self.parent = None
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("trail")
 
         if self.alignment is not None:
             xml.attrib["ALIGN"] = self.alignment
 
         if self.parent is not None:
             xml.attrib["PARENT"] = self.parent
 
         return xml
 
-    def fromxml(self, xml):
-        if xml.tag == "trail":
-
-            align = xml.get("ALIGN")
-            if align is not None:
-                # TODO use human values...
-                self.alignment = align
-
-            parent = xml.get("PARENT")
-            if parent is not None:
-                self.parent = parent
+    def fromxml(self, xml: ET.Element) -> bool:
+        if xml.tag != "trail":
+            return False
 
-            return True
+        align = xml.get("ALIGN")
+        if align is not None:
+            # TODO use human values...
+            self.alignment = align
+
+        parent = xml.get("PARENT")
+        if parent is not None:
+            self.parent = parent
 
-        return False
+        return True
 
 
-class StoryDefaultStyle(OrphanElement):
+class StoryDefaultStyle(PyScribusElement):
     """
     Default style marker in Scribus stories (DefaultStyle)
     """
 
     def __init__(self):
-        OrphanElement.__init__(self, "DefaultStyle")
+        super().__init__()
+
+        self.parent_paragraph = None
+        self.parent_character = None
+
+    def fromxml(self, xml: ET.Element) -> bool:
+        """
+        :rtype: boolean
+        :returns: True if XML parsing succeed
+        """
+
+        if xml.tag != "DefaultStyle":
+            return False
+
+        para_parent = xml.get("PARENT")
+        if para_parent is not None:
+            self.parent_paragraph = para_parent
+
+        chara_parent = xml.get("CPARENT")
+        if chara_parent is not None:
+            self.parent_character = chara_parent
+
+        return True
+
+    def toxml(self) -> ET.Element:
+        """
+        :rtype: lxml.etree._Element
+        :returns: XML representation of default style marker.
+        """
+
+        xml = ET.Element("DefaultStyle")
+
+        if self.parent_paragraph is not None:
+            xml.attrib["PARENT"] = self.parent_paragraph
+
+        if self.parent_character is not None:
+            xml.attrib["CPARENT"] = self.parent_character
+
+        return xml
 
 
 class StoryLineBreak(OrphanElement):
     """
     Line break marker in Scribus stories (breakline)
     """
 
     def __init__(self):
         OrphanElement.__init__(self, "breakline")
 
 
+class StoryFrameBreak(OrphanElement):
+    """
+    Frame break marker in Scribus stories (breakframe)
+    """
+
+    def __init__(self):
+        OrphanElement.__init__(self, "breakframe")
+
+
+class StoryColumnBreak(OrphanElement):
+    """
+    Column break marker in Scribus stories (breakcol)
+    """
+
+    def __init__(self):
+        OrphanElement.__init__(self, "breakcol")
+
+
 class NonBreakingHyphen(OrphanElement):
     """
     Non breaking hyphen in Scribus stories (nbhyphen)
     """
 
     def __init__(self):
         OrphanElement.__init__(self, "nbhyphen")
@@ -134,19 +190,20 @@
     def __init__(self, parent=False, doc_parent=False):
         super().__init__()
 
         self.parent = parent
 
         self.doc_parent = False
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "PARAGEND|{}".format(self.parent)
 
-    def fromxml(self, xml, check_style=True):
+    def fromxml(self, xml: ET.Element, check_style: bool = True) -> bool:
         parentpar = xml.get("PARENT")
+
         if parentpar is None:
             self.parent = False
         else:
             self.parent = parentpar
 
             if check_style and self.parent:
 
@@ -160,15 +217,15 @@
                             break
 
                     if not checked:
                         raise exceptions.UnknownStyleInStory(self.parent)
 
         return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("para")
 
         if self.parent:
             xml.attrib["PARENT"] = self.parent
 
         return xml
 
@@ -227,28 +284,37 @@
 
        frag = stories.StoryFragment(
            text="Lorem ipsum", fontsize=7, fontcolor="Grey"
        )
 
     """
 
+    font_xml = [
+        ["name", "FONT"],
+        ["color", "FCOLOR"],
+        ["opacity", "FSHADE"],
+        ["size", "FONTSIZE"]
+    ]
+
     def __init__(self, **kwargs):
         super().__init__()
 
         self.text = ""
 
         # To not export to XML. This is defined by the following
         # StoryParagraphEnding in Story.sequence
         self.paragraph_style = False
 
+        self.parent_character = None
+
         self.font = {
             "name": False,
             "size": False,
             "color": False,
-            "opacity": False
+            "opacity": False,
         }
 
         # Features
         self.features = {
             "inherit": False,
             "smallcaps": False,
             "allcaps": False,
@@ -258,15 +324,15 @@
             "underline": False,
             "underlinewords": False,
         }
 
         if kwargs:
             self._quick_setup(kwargs)
 
-    def _quick_setup(self, settings):
+    def _quick_setup(self, settings: dict) -> NoReturn:
         """
         Method for defining story fragment settings from class
         instanciation kwargs.
 
         :type settings: dict
         :param settings: Kwargs dictionnary
         """
@@ -297,226 +363,394 @@
                 if setting_name in self.features.keys():
 
                     if setting_value:
                         self.features[setting_name] = True
                     else:
                         self.features[setting_name] = False
 
-    def fromdefault(self):
+    def fromdefault(self) -> NoReturn:
         self.text = ""
 
         self.paragraph_style = False
 
         self.font = {
             "name": False,
             "size": False,
             "color": False,
-            "opacity": False
+            "opacity": False,
         }
 
         self.features = {
             "inherit": False,
             "smallcaps": False,
             "allcaps": False,
             "superscript": False,
             "strike": False,
             "subscript": False,
             "underline": False,
             "underlinewords": False,
         }
 
-    def __iadd__(self, fragment):
+    def __iadd__(self, fragment) -> StoryFragment:
         """
         += operator can be used to join another fragment text.
 
         The second term **inherits the features of the first**.
         """
         if isinstance(fragment, StoryFragment):
             self.text += fragment.text
             return self
-        else:
-            raise TypeError()
 
-    def __repr__(self):
-        def font_repr(f):
-            if f:
-                return f
-            else:
-                return ""
+        raise TypeError()
 
-        def features_repr(f):
-            return [k for k in f if f[k]]
+    def __repr__(self) -> str:
+        def font_repr(font):
+            return {True: font, False: ""}[bool(font)]
+
+        def features_repr(features: dict) -> list:
+            return [k for k in features if features[k]]
 
         return "FRAGMENT|{}|{}|{}".format(
             font_repr(self.font["name"]),
             self.text,
-            features_repr(self.features)
+            features_repr(self.features),
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.text
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         xml = ET.Element("ITEXT")
 
         have_features = len([f for f in self.features.values() if f])
 
         if have_features:
             features = []
 
-            for f,v in self.features.items():
-                if v:
-                    features.append(f)
+            for feature_name, feature_value in self.features.items():
+                if feature_value:
+                    features.append(feature_name)
 
             features = " ".join(features)
 
             xml.attrib["FEATURES"] = features
 
-        for case in zip(
-                    ["name", "color", "opacity", "size"],
-                    ["FONT", "FCOLOR", "FSHADE", "FONTSIZE"],
-                    ):
-            if self.font[case[0]]:
-                xml.attrib[case[1]] = self.font[case[0]]
+        for human, attr_name in StoryFragment.font_xml:
+
+            if self.font[human]:
+                xml.attrib[attr_name] = self.font[human]
+
+        if self.parent_character is not None:
+            xml.attrib["CPARENT"] = self.parent_character
 
         xml.attrib["CH"] = self.text
 
         return xml
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET._Element) -> bool:
         fragtext = xml.get("CH")
-        if fragtext is not None:
+        if fragtext is None:
+            return False
 
-            # NOTE Don't do any strip, rstrip to @CH, as it may
-            # contains legitimate spaces
-            self.text = fragtext
-
-            features = xml.get("FEATURES")
-            if features is not None:
-                self.set_features(features)
-
-            for case in zip(
-                        ["name", "color", "opacity", "size"],
-                        ["FONT", "FCOLOR", "FSHADE", "FONTSIZE"],
-                        ):
-
-                att = xml.get(case[1])
-                if att is not None:
-                    self.font[case[0]] = att
+        chara_parent = xml.get("CPARENT")
+        if chara_parent is not None:
+            self.parent_character = chara_parent
 
-            # TODO Reste de l’implémentation, puis :
+        # NOTE Don't do any strip, rstrip to @CH, as it may
+        # contains legitimate spaces
+        self.text = fragtext
 
-            return True
-        else:
-            return False
+        features = xml.get("FEATURES")
+        if features is not None:
+            self.set_features(features)
+
+        for human, attr_name in StoryFragment.font_xml:
+
+            att = xml.get(attr_name)
+            if att is not None:
+                self.font[human] = att
+
+        # TODO Reste de l’implémentation, puis :
+
+        return True
 
-    def set_features(self, features):
+    def set_features(self, features: str) -> NoReturn:
         # TODO
 
         features = features.split()
 
         for feature in features:
             if feature in self.features.keys():
                 self.features[feature] = True
 
 
+class TemporaryFragment(StoryFragment):
+    """
+    Special character in Scribus stories inserted with ITEXT XML element.
+
+    This story sequence element will be merged at save time or at insertion
+    into the story sequence if `inherit` parameter is used.
+
+    :type kwargs: dict
+    :param kwargs: Quick setting (see StoryFragment.__init__ kwargs table)
+
+    :ivar string text: Text content
+
+    .. seealso:: pyscribus.stories.StoryFragment.__init__
+    .. seealso:: pyscribus.stories.Story.append
+    """
+
+    def __init__(self, text: str, **kwargs):
+        super().__init__()
+
+        self.text = text
+
+        if kwargs:
+            self._quick_setup(kwargs)
+
+    def _quick_setup(self, settings: dict) -> NoReturn:
+        """
+        Method for defining story fragment settings from class
+        instanciation kwargs.
+
+        :type settings: dict
+        :param settings: Kwargs dictionnary
+        """
+
+        if settings:
+            # TemporaryFragment is used as base class for predefined
+            # StoryFragment instances. It's text attribute is set at
+            # instanciation, not with quick setup.
+            if "text" in settings:
+                settings.pop("text")
+
+            StoryFragment._quick_setup(self, settings)
+
+
+class NarrowNonBreakingSpace(TemporaryFragment):
+    """
+    Narrow no break space.
+
+    (French « espace fine insécable »)
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(" ", **kwargs)
+
+
+class EnSpace(TemporaryFragment):
+    """
+    (French « espace demi-quadratin »)
+    """
+
+    def __init__(self, **kwargs):
+        # Not the author of this library social account.
+        super().__init__(" ", **kwargs)
+
+
+class EmSpace(TemporaryFragment):
+    """
+    (French « espace quadratin »)
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(" ", **kwargs)
+
+
+class ThinSpace(TemporaryFragment):
+    """
+    Thin space.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(" ", **kwargs)
+
+
+class ThreePerEmSpace(TemporaryFragment):
+    """
+    1/3 em space. Also called thick space.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(" ", **kwargs)
+
+
+class ThickSpace(ThreePerEmSpace):
+    """
+    Thick space. Alias for ThreePerEmSpace.
+    """
+
+
+class FourPerEmSpace(TemporaryFragment):
+    """
+    1/4 em space. Also called mid space.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(" ", **kwargs)
+
+
+class MidSpace(FourPerEmSpace):
+    """
+    Mid space. Alias for FourPerEmSpace.
+    """
+
+
+class HairSpace(TemporaryFragment):
+    """
+    Hair space. Also called very thin space.
+    """
+
+    def __init__(self, **kwargs):
+        # "BEHOLD, Hair space, the dimension of metalheads!"
+        super().__init__(" ", **kwargs)
+
+
+class VeryThinSpace(HairSpace):
+    """
+    Very thin space. Alias for HairSpace.
+    """
+
+
+class UnicodeJoiner(TemporaryFragment):
+    """
+    Unicode zero width joiner (U+200D)
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__("‍", **kwargs)
+
+
+class UnicodeNonJoiner(TemporaryFragment):
+    """
+    Unicode zero width non-joiner (U+200C)
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__("‌", **kwargs)
+
+
 class StoryVariable(PyScribusElement):
     """
     Variable in a Scribus story (var).
 
     :type name: string
     :param name: Name of the variable. Must be in StoryVariable.var_names.
 
     :ivar string name: Name of the variable
     """
 
     var_names = ["pgno", "pgco"]
 
-    def __init__(self, name=""):
+    def __init__(self, name: str = ""):
         super().__init__()
 
-        if nam in StoryVariable.var_names or nam == "":
+        if name in StoryVariable.var_names or name == "":
             self.name = name
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         :rtype: lxml.etree._Element
         :returns: XML representation of story variable
         """
 
         element = ET.Element("var")
 
         element.attrib["name"] = self.name
 
         return element
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         :rtype: boolean
         :returns: True if XML parsing succeed
         """
 
-        if xml.tag == "var":
+        if xml.tag != "var":
+            return False
 
-            nam = xml.get("name")
-            if nam is None:
-                return False
-            else:
-                if nam in StoryVariable.var_names:
-                    self.name = nam
+        nam = xml.get("name")
+        if nam is None:
+            return False
 
-            return True
+        if nam in StoryVariable.var_names:
+            self.name = nam
 
-        else:
-            return False
+        return True
 
 
 class PageNumberVariable(StoryVariable):
     """
     Page number variable in a Scribus story
     """
 
     def __init__(self):
         super().__init__("pgno")
 
+
 class PageCountVariable(StoryVariable):
     """
     Count of total pages variable in a Scribus story
     """
 
     def __init__(self):
         super().__init__("pgco")
 
+
 # Variables globales 2 ==================================================#
 
+
 variable_classes = {
     "pgno": PageNumberVariable,
     "pgco": PageCountVariable,
 }
 
+NonEndingSequenceElement = Union[
+    StoryFragment,
+    StoryParagraphEnding,
+    StoryLineBreak,
+    StoryFrameBreak,
+    StoryColumnBreak,
+    TemporaryFragment,
+    NarrowNonBreakingSpace,
+    EnSpace,
+    ThinSpace,
+    ThreePerEmSpace,
+    ThickSpace,
+    FourPerEmSpace,
+    MidSpace,
+    HairSpace,
+    VeryThinSpace,
+    UnicodeJoiner,
+    UnicodeNonJoiner,
+]
+
 # Parsing functions =====================================================#
 
+
 def sequencefromhtml(
-        html,
-        font={
-            "italic": "Arial Italic",
-            "bold": "Arial Bold",
-            "bold-italic": "Arial Bold Italic"},
-        alternate_emphasis=False,
-        sla_document=False):
+    html,
+    font={
+        "italic": "Arial Italic",
+        "bold": "Arial Bold",
+        "bold-italic": "Arial Bold Italic",
+    },
+    alternate_emphasis: bool = False,
+    sla_document=False,
+) -> list:
     """
     :type html: string
     :param html: Paragraph text in PSM (PyScribus Story Markup)
     :type font: dict
     :param font: Fonts used for text emphasis
     :type alternate_emphasis: boolean
     :param alternate_emphasis: Nested emphasis returns to regular font.
     :type sla_document: pyscribus.document.Document
-    :param sla_document: Instance of PyScribus Document where notes & marks will
-        be stored.
+    :param sla_document: Instance of PyScribus Document where notes & marks
+        will be stored.
     :rtype: list
     :returns: List of pyscribus.stories.Story sequence elements
     """
 
     def tag_to_data(fragment, tag):
         """
         Modify fragment font and features according to tag value.
@@ -524,48 +758,41 @@
 
         if tag in ["em", "i"]:
             fragment.font = font["italic"]
 
         if tag in ["b", "strong"]:
             fragment.font = font["bold"]
 
-        if tag in ["sup"]:
-            fragment.features["superscript"] = True
-
-        if tag in ["sub"]:
-            fragment.features["subscript"] = True
-
-        if tag in ["u"]:
-            fragment.features["underline"] = True
-
-        if tag in ["sc"]:
-            fragment.features["smallcaps"] = True
+        for tags, feature_key in [
+            [["sup"], "superscript"],
+            [["sub"], "subscript"],
+            [["u"], "underline"],
+            [["sc"], "smallcaps"],
+        ]:
+            if tag in tags:
+                fragment.features[feature_key] = True
 
         return fragment
 
     def attrib_to_data(fragment, element):
         """
         Read @style attribute of element and modify fragment features
         accordingly.
         """
 
         if element.tag == "span":
 
             if "style" in element.attrib:
-                css = [
-                    r.strip()
-                    for r
-                    in element.attrib["style"].split(";")
-                ]
+                css = [r.strip() for r in element.attrib["style"].split(";")]
 
                 for rule in css:
 
                     # Little cleaning -> CSS property name and value
-                    rule = rule.replace(": ",":").split(":")
-                    name,value = rule[0],":".join(rule[1:])
+                    rule = rule.replace(": ", ":").split(":")
+                    name, value = rule[0], ":".join(rule[1:])
 
                     if name == "font-variant":
 
                         if value == "small-caps":
                             fragment.features["smallcaps"] = True
 
                     if name == "text-transform":
@@ -584,63 +811,76 @@
         """
         Parse note XML data wether it comes from a <note> or a
         <span class="note"> element.
         """
         nid = element.get("id")
 
         if nid is None:
-            raise ValueError(
-                "<note> without @id."
-            )
-        else:
-            # Mark of the note in the story ----------------------
+            raise ValueError("<note> without @id.")
 
-            story_note = marks.StoryNoteMark(label=nid)
-            story_note.fromdefault()
+        # Mark of the note in the story ----------------------
 
-            # Note content in DOCUMENT ---------------------------
+        story_note = marks.StoryNoteMark(label=nid)
+        story_note.fromdefault()
 
-            # TODO FIXME Now that the mark is in the story,
-            # we must add the note content into the DOCUMENT
-            # <Notes>
+        # Note content in DOCUMENT ---------------------------
 
-            if sla_document:
-                document_note = notes.Note()
-                document_note.fromdefault()
-                document_note.parent_mark = nid
+        # TODO FIXME Now that the mark is in the story,
+        # we must add the note content into the DOCUMENT
+        # <Notes>
 
-                # TODO FIXME Handle note style
-                # TODO FIXME Handle note text
+        if sla_document:
+            document_note = notes.Note()
+            document_note.fromdefault()
+            document_note.parent_mark = nid
 
-                sla_document.notes.append(document_note)
+            # TODO FIXME Handle note style
+            # TODO FIXME Handle note text
 
-            # Mark of the note in the DOCUMENT marks -------------
+            sla_document.notes.append(document_note)
 
-            if sla_document:
-                document_mark = marks.DocumentMark()
-                document_mark.fromdefault("note")
-                document_mark.label = nid
-                sla_document.marks.append(document_mark)
+        # Mark of the note in the DOCUMENT marks -------------
 
-            # ----------------------------------------------------
+        if sla_document:
+            document_mark = marks.DocumentMark()
+            document_mark.fromdefault("note")
+            document_mark.label = nid
+            sla_document.marks.append(document_mark)
 
-            sequence.append(story_note)
+        # ----------------------------------------------------
+
+        sequence.append(story_note)
 
         return sequence, sla_document
 
-    def parse_element(element, sequence, font, previous, alternate_emphasis, sla_document):
+    def parse_element(
+        element, sequence, font, previous, alternate_emphasis, sla_document
+    ):
+
         global variable_classes
 
-        if element.tag in ["em", "i", "span", "b", "strong", "sup", "sub", "u", "sc"]:
+        if element.tag in [
+            "em",
+            "i",
+            "span",
+            "b",
+            "strong",
+            "sup",
+            "sub",
+            "u",
+            "sc",
+        ]:
             is_fragment = True
 
         if element.tag == "note":
             is_fragment = False
 
-            sequence, sla_document = parse_note(element, sequence, sla_document)
+            sequence, sla_document = parse_note(
+                element, sequence, sla_document
+            )
 
         if element.tag in ["pgno", "pgco"]:
             is_fragment = False
 
             variable = Story.variable_classes[element.tag]()
             sequence.append(variable)
 
@@ -652,29 +892,31 @@
 
             if "class" in element.attrib:
                 element_classes = [
                     cn.strip()
                     for cn in element.attrib["class"].strip().split()
                 ]
 
-                # Get the count of incompatible classes in span @class attribute
-                # So <span class="pgno note"></span> will not work.
+                # Get the count of incompatible classes in span @class
+                # attribute, so <span class="pgno note"></span> will not work.
+
                 main_class = len(
                     [
                         c
                         for c in ["pgno", "pgco", "note"]
                         if c in element_classes
                     ]
                 )
 
                 if main_class <= 1:
 
                     for element_class in element_classes:
-                        # NOTE This iteration to check multiple classes in @class
-                        # attribute, if a precision of a class is needed.
+                        # NOTE This iteration to check multiple classes in
+                        # @class attribute, if a precision of a class is
+                        # needed.
 
                         if element_class in ["pgno", "pgco"]:
                             is_fragment = False
 
                             variable = Story.variable_classes[element_class]()
                             sequence.append(variable)
 
@@ -686,17 +928,16 @@
                             sequence, sla_document = parse_note(
                                 element, sequence, sla_document
                             )
 
                             break
                 else:
                     raise ValueError(
-                        "Incompatible classes in span element @class : '{}'".format(
-                            ",".join(element_classes)
-                        )
+                        "Incompatible classes in span element "
+                        "@class : '{}'".format(",".join(element_classes))
                     )
 
         if is_fragment:
             fragment = StoryFragment(text=element.text)
 
             read_tag = True
 
@@ -723,15 +964,15 @@
 
                 sequence = parse_element(
                     sub_element,
                     sequence,
                     font,
                     element,
                     alternate_emphasis,
-                    sla_document
+                    sla_document,
                 )
 
         if element.tail is not None:
             tail_fragment = StoryFragment(text=element.tail)
             tail_fragment = tag_to_data(tail_fragment, previous.tag)
             tail_fragment = attrib_to_data(tail_fragment, previous)
 
@@ -767,26 +1008,28 @@
 
             sequence = parse_element(
                 element,
                 sequence,
                 font,
                 parsed,
                 alternate_emphasis,
-                sla_document
+                sla_document,
             )
 
     if parsed.tail is not None:
         sequence.append(StoryFragment(text=parsed.tail))
 
     # ---------------------------------------------------------------
 
     return sequence
 
+
 # Story class ===========================================================#
 
+
 class Story(PyScribusElement):
     """
     Story in SLA (StoryText). A text buffer.
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: Parent SLA instance.
     :type doc_parent: pyscribus.document.Document
@@ -794,36 +1037,37 @@
     :type pgo_parent: pyscribus.pageobjects.PageObject
     :param pgo_parent: Parent page object instance.
 
     :ivar pyscribus.sla.SLA sla_parent: Parent SLA instance.
     :ivar pyscribus.document.Document doc_parent: Parent Document instance.
     :ivar list sequence: List of instances of StoryFragment,
         StoryParagraphEnding, StoryLineBreak, StoryDefaultStyle,
-        NonBreakingHyphen, StoryVariable
+        NonBreakingHyphen, StoryVariable, TemporaryFragment derivated,
+        StoryFrameBreak, StoryColumnBreak
     """
 
     def __init__(self, sla_parent=False, doc_parent=False, pgo_parent=False):
         super().__init__()
 
         self.sequence = []
 
         self.sla_parent = sla_parent
         self.doc_parent = doc_parent
         self.pgo_parent = pgo_parent
 
-    def _without_ending(self):
+    def _without_ending(self) -> list:
         temp = []
 
         if self.sequence:
             if isinstance(self.sequence[-1], StoryEnding):
                 temp = self.sequence[:-1]
 
         return temp
 
-    def append_paragraph(self, **kwargs):
+    def append_paragraph(self, **kwargs) -> bool:
         """
         Append a paragraph at the end of the story.
 
         :type kwargs: dict
         :param kwargs: kwargs
 
         +-------------------+--------------+---------+--------------------------+
@@ -842,16 +1086,16 @@
         +-------------------+--------------+---------+--------------------------+
         |alternate_emphasis | boolean      | False   | Nice emphasis, as nested |
         |                   |              |         | italic in italic becames |
         |                   |              |         | regular. Same for bold   |
         |                   |              |         | nested in bold.          |
         +-------------------+--------------+---------+--------------------------+
 
-        As there is only one paragraph added by append_paragraph, the <p> element,
-        enclosing the paragraph, can be omitted in text argument.
+        As there is only one paragraph added by append_paragraph, the <p>
+        element, enclosing the paragraph, can be omitted in text argument.
 
         :Example:
 
         .. code:: python
 
            story.append_paragraph(
                text="Le chant du cygne est très beau.", style="Normal"
@@ -866,20 +1110,21 @@
 
         """
 
         self._append_paragraph(kwargs)
 
         return True
 
-    def append_paragraphs(self, paragraphs=[]):
+    def append_paragraphs(self, paragraphs: list = []) -> bool:
         """
         Append multiple paragraphs at the end of the story.
 
         :type paragraphs: list
-        :param paragraphs: List of Story.append_paragraph() kwargs dictionnaries.
+        :param paragraphs: List of Story.append_paragraph() kwargs
+            dictionnaries.
 
         :Example:
 
         .. code:: python
 
            story.append_paragraphs(
               [
@@ -902,41 +1147,41 @@
 
         if paragraphs:
 
             for paragraph in paragraphs:
                 self._append_paragraph(paragraph)
 
             return True
-        else:
-            return False
 
-    def _append_paragraph(self, kwargs):
+        return False
+
+    def _append_paragraph(self, kwargs: dict) -> NoReturn:
         """
         Private method to append paragraph.
 
         Used by append_paragraph() and append_paragraphs()
 
         :type kwargs: dict
         :param paragraphs: kwargs of Story.append_paragraph()
         """
 
         # kwargs processing -------------------------------
 
-        style,source,inherit_style = False,False,False
+        style, source, inherit_style = False, False, False
         alternate_emphasis = False
 
         ending = True
 
-        font={
+        font = {
             "bold": "Arial Bold",
             "italic": "Arial Italic",
-            "bold-italic": "Arial Bold Italic"
+            "bold-italic": "Arial Bold Italic",
         }
 
-        for param,value in kwargs.items():
+        for param, value in kwargs.items():
 
             if param == "text":
                 source = value
 
             if param == "ending":
                 ending = bool(value)
 
@@ -967,15 +1212,15 @@
 
         # -------------------------------------------------
 
         sequence = sequencefromhtml(
             source,
             font=font,
             alternate_emphasis=alternate_emphasis,
-            sla_document=self.doc_parent
+            sla_document=self.doc_parent,
         )
 
         if ending:
             para = StoryParagraphEnding()
 
             if style or inherit_style:
                 ps = False
@@ -998,161 +1243,230 @@
 
             sequence.append(para)
 
         temp = self._without_ending()
         self.sequence = temp + sequence
         self.end_contents()
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         Return the story as XML element.
 
-        :rtype: lxml._Element
+        :rtype: lxml.etree._Element
         """
 
         xml = ET.Element("StoryText")
 
         for element in self.sequence:
             ex = element.toxml()
             xml.append(ex)
 
         return xml
 
-    def fromxml(self, xml, check_style=True):
+    def fromxml(self, xml: ET.Element, check_style: bool = True) -> bool:
         """
         Parses XML of a SLA Story.
 
-        :type xml: lxml._Element
-        :param xml: SLA Story as lxml._Element
+        :type xml: lxml.etree._Element
+        :param xml: SLA Story as lxml.etree._Element
         :type check_style: bool
         :param check_style: Check if story paragraphs use known paragraph
             styles of Story.doc_parent Document. True by default.
 
         .. note:: You might set check_style to False if you want to parse
             stories independantly of any given SLA & Document instances.
 
         :rtype: bool
         :returns: bool
 
         """
 
         global variable_classes
 
-        if xml.tag == "StoryText":
+        if xml.tag != "StoryText":
+            return False
 
-            for element in xml:
+        for element in xml:
 
-                if element.tag == "DefaultStyle":
-                    self.sequence.append(StoryDefaultStyle())
+            if element.tag == "DefaultStyle":
+                default_xml = StoryDefaultStyle()
+                success = default_xml.fromxml(element)
 
-                if element.tag == "ITEXT":
+                if success:
+                    self.sequence.append(default_xml)
 
-                    frag = StoryFragment()
-                    success = frag.fromxml(element)
+            if element.tag == "ITEXT":
 
-                    if success:
-                        self.sequence.append(frag)
+                frag = StoryFragment()
+                success = frag.fromxml(element)
 
-                # End of a paragraph
+                if success:
+                    self.sequence.append(frag)
 
-                if element.tag == "para":
-                    para = StoryParagraphEnding(self.doc_parent)
-                    success = para.fromxml(element, check_style)
+            # End of a paragraph
 
-                    if success:
+            if element.tag == "para":
+                para = StoryParagraphEnding(self.doc_parent)
+                success = para.fromxml(element, check_style)
 
-                        # NOTE @PARENT carries the style name of the preceding
-                        # StoryFragment / <ITEXT> in the sequence
+                if success:
 
-                        if para.parent:
+                    # NOTE @PARENT carries the style name of the preceding
+                    # StoryFragment / <ITEXT> in the sequence
 
-                            # NOTE Empty lines in the story are just <para>
-                            # following each others. So we only set the
-                            # paragraph_style of the preceding fragment…
-                            # if there *is* a fragment to begin with.
+                    if para.parent:
 
-                            if isinstance(self.sequence[-1], StoryFragment):
-                                self.sequence[-1].paragraph_style = para.parent
+                        # NOTE Empty lines in the story are just <para>
+                        # following each others. So we only set the
+                        # paragraph_style of the preceding fragment…
+                        # if there *is* a fragment to begin with.
 
-                        self.sequence.append(para)
+                        if isinstance(self.sequence[-1], StoryFragment):
+                            self.sequence[-1].paragraph_style = para.parent
 
-                # Line break in a paragraph
+                    self.sequence.append(para)
 
-                if element.tag == "breakline":
-                    self.sequence.append(StoryLineBreak())
+            # Line break in a paragraph
 
-                # Non breaking hyphen
+            if element.tag == "breakline":
+                self.sequence.append(StoryLineBreak())
 
-                if element.tag == "nbhyphen":
-                    self.sequence.append(NonBreakingHyphen())
+            # Column break in a paragraph
 
-                # Non breaking space
+            if element.tag == "breakcol":
+                self.sequence.append(StoryColumnBreak())
 
-                if element.tag == "nbspace":
-                    self.sequence.append(NonBreakingSpace())
+            # Frame break in a paragraph
 
-                # Mark
+            if element.tag == "breakframe":
+                self.sequence.append(StoryFrameBreak())
 
-                if element.tag == "MARK":
-                    # TODO Selon @type, un StoryNoteMark ou autre
-                    pass
+            # Non breaking hyphen
 
-                # Variable
+            if element.tag == "nbhyphen":
+                self.sequence.append(NonBreakingHyphen())
 
-                if element.tag == "var":
+            # Non breaking space
 
-                    var_name = element.get("name")
+            if element.tag == "nbspace":
+                self.sequence.append(NonBreakingSpace())
 
-                    if var_name is not None:
-                        var_instance = Story.variable_classes[var_name]()
-                        self.sequence.append(var_instance)
+            # Mark
 
-                # Story end
+            if element.tag == "MARK":
+                new_mark = marks.story_mark_from_xml(xml)
 
-                if element.tag == "trail":
-                    story_ending = StoryEnding()
-                    success = story_ending.fromxml(element)
+                if new_mark:
+                    self.sequence.append(new_mark)
 
-                    if success:
-                        self.sequence.append(story_ending)
-                    break
+            # Variable
 
-            return True
+            if element.tag == "var":
 
-        return False
+                var_name = element.get("name")
+
+                if var_name is not None:
+                    var_instance = Story.variable_classes[var_name]()
+                    self.sequence.append(var_instance)
+
+            # Story end
 
-    def fromdefault(self):
+            if element.tag == "trail":
+                story_ending = StoryEnding()
+                success = story_ending.fromxml(element)
+
+                if success:
+                    self.sequence.append(story_ending)
+                break
+
+        return True
+
+    def fromdefault(self) -> NoReturn:
         """
         Set a default story
         """
 
         self.sequence = [StoryDefaultStyle(), StoryEnding()]
 
-    def append(self, element):
+    def append(
+        self,
+        element: NonEndingSequenceElement,
+        inherit: bool = False,
+    ) -> bool:
         """
         Append a element to the Story sequence.
 
         .. warning:: Don't use append() to append a StoryEnding, use
             end_contents() instead.
 
-        :type element: StoryFragment, StoryParagraphEnding, StoryLineBreak, StoryDefaultStyle
+        :type element: StoryFragment, StoryParagraphEnding, StoryLineBreak,
+            StoryDefaultStyle, TemporaryFragment derivated, StoryFrameBreak,
+            StoryColumnBreak
         :param element: Element to add to the story sequence
         :rtype: bool
         :returns: bool
 
         .. seealso:: pyscribus.stories.end_contents
         """
 
+        # Getting the story sequence without StoryEnding -----------------
+
         temp = self._without_ending()
-        self.sequence = temp + [element]
-        self.end_contents()
 
+        # Not a TemporaryFragment : we dont care about inherit -----------
+
+        if not isinstance(element, TemporaryFragment):
+            self.sequence = temp + [element]
+            self.end_contents()
+            return True
+
+        # Handle inherit as it is a TemporaryFragment --------------------
+
+        if not inherit:
+            self.sequence = temp + [element]
+            self.end_contents()
+            return True
+
+        if isinstance(temp[-1], StoryFragment):
+            # If the last sequence element is a story fragment
+            # we simply add the TemporaryFragment text to that
+            # last sequence.
+            temp[-1].text += element.text
+        else:
+            # If the last sequence element of the story is not a
+            # StoryFragment, it can't be a StoryEnding, because we
+            # already removed it.
+            # So the last item can be :
+            #   - a special character
+            #   - a <DefaultStyle>
+            #   - a mark (marks.StoryMarkAbstract subclasses)
+
+            for seq_element in reversed(temp):
+                if isinstance(seq_element, StoryDefaultStyle):
+                    # If it is a <DefaultStyle>, there is nothing to
+                    # inherit from.
+                    self.sequence = temp + [StoryFragment(text=element.text)]
+                    break
+
+                # NOTE We dont care about marks
+
+                if isinstance(seq_element, StoryFragment):
+                    # If it is a StoryFragment, we use it's formatting
+                    # settings to make a new story fragment.
+                    new_fragment = copy.deepcopy(seq_element)
+                    new_fragment.text = element.text
+                    self.sequence = temp + [new_fragment]
+                    break
+
+        # Ending the story sequence --------------------------------------
+
+        self.end_contents()
         return True
 
-    def end_contents(self, no_trailing_paragraph=False):
+    def end_contents(self, no_trailing_paragraph: bool = False) -> NoReturn:
         """
         Ends the story's content by making sure that the story sequence
         is valid.
 
         .. note:: It is better to use this method than appending a
             :class:`StoryEnding` instance directly into the story sequence.
 
@@ -1169,28 +1483,28 @@
                 self.sequence.pop(-1)
 
         if story_ending is None:
             self.sequence.append(StoryEnding())
         else:
             self.sequence.append(story_ending)
 
-    def init_contents(self):
+    def init_contents(self) -> NoReturn:
         self.sequence = [StoryDefaultStyle()]
 
-    def bypars(self):
+    def bypars(self) -> list:
         """
         Return a list of list of Story.sequence elements organized as human
         paragraphs.
 
         :returns: list of lists
         :rtype: ilst
         """
 
-        pars = [] # List of paragraphs
-        tmp = [] # Temporary list of paragraph elements
+        pars = []  # List of paragraphs
+        tmp = []  # Temporary list of paragraph elements
 
         for element in self.sequence:
 
             # End of the story -> last paragraph is added to the list
 
             if isinstance(element, StoryEnding):
                 if tmp:
@@ -1204,113 +1518,23 @@
                 if tmp:
                     tmp.append(element)
                     pars.append(tmp)
                     tmp = []
 
             # Paragraph content -------------------------------------
 
-            for class_test in [StoryFragment, StoryDefaultStyle,
-                    NonBreakingSpace, NonBreakingHyphen, StoryVariable]:
+            for class_test in [
+                StoryFragment,
+                StoryDefaultStyle,
+                NonBreakingSpace,
+                NonBreakingHyphen,
+                StoryVariable,
+            ]:
 
                 if isinstance(element, class_test):
                     tmp.append(element)
                     break
 
         return pars
 
-    def rawtext(self):
-        """
-        Returns a text string equivalent to *what Scribus story editor
-        saves* as txt file.
-
-        :rtype: string
-        """
-        text = ""
-
-        for par in self.bypars():
-
-            for element in par:
-
-                # NOTE Text formatting is not saved
-                if isinstance(element, StoryFragment):
-                    text += element.text
-
-                if isinstance(element, NonBreakingSpace):
-                    text += " "
-
-                # NOTE Line breaks are exported by Scribus... as spaces
-                if isinstance(element, StoryLineBreak):
-                    text += " "
-
-                if isinstance(element, StoryParagraphEnding):
-                    text += "\n"
-
-        return text
-
-    def templatable(self):
-        """
-        Return elements of Story sequence that are available for templating.
-
-        :rtype: list
-        :returns: List of pyscribus.stories.StoryFragment
-        """
-
-        contents = []
-
-        pattern = self.sla_parent.templating["intext-pattern"]
-
-        for element in self.sequence:
-
-            if isinstance(element, StoryFragment):
-
-                if pattern.findall(element.text):
-                    contents.append(element)
-
-        return contents
-
-    def feed_templatable(self, datas: dict) -> Union[bool, List[StoryFragment]]:
-        """
-        Feed template-able datas into this story.
-
-        :returns: List of modified elements in this story, or False
-        :rtype: Union[bool, list]
-        """
-
-        elements = self.templatable()
-
-        if elements:
-            modified = []
-
-            for element in elements:
-
-                for template_key, template_value in datas.items():
-
-                    if template_key not in element.text:
-                        continue
-
-                    new_value = None
-
-                    if isinstance(datas[template_key], list):
-                        # We have %key% -> ["Value1", "Value2", …]
-                        # So the first occurrence of %key% is "Value1", the
-                        # second "Value2", etc.
-
-                        if len(datas[template_key]):
-                            new_value = datas[template_key].pop(0)
-                    else:
-                        # We have %key% -> "Value"
-                        new_value = template_value
-
-                    if new_value is None:
-                        continue
-
-                    element.text = element.text.replace(
-                        template_key, new_value
-                    )
-
-                    modified.append(element)
-
-            return modified
-
-        return False
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/styles.py` & `pyscribus-backported-0.3/pyscribus/model/styles.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,31 +29,32 @@
 from typing import Union, Optional, NoReturn, Literal
 from enum import IntEnum
 from pathlib import Path
 
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
-import pyscribus.common.math as mathc
-import pyscribus.logs as logs
-import pyscribus.exceptions as exceptions
-import pyscribus.dimensions as dimensions
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.common.math as mathc
+import pyscribus.model.logs as logs
+import pyscribus.model.exceptions as exceptions
+import pyscribus.model.dimensions as dimensions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 StringOrPath = Union[str, Path]
 BoolOrElement = Union[bool, ET.Element]
 
 LeadingMode = Literal["fixed", "automatic", "grid"]
 
 # Classes ===============================================================#
 
+
 class TextDirection(IntEnum):
     """
     Enum for (paragraph) STYLE/@DIRECTION values.
     """
 
     LTR = 0
     RTL = 1
@@ -66,15 +67,15 @@
         "document": "0",
         "section": "1",
         "story": "2",
         "page": "3",
         "form": "4",
     }
 
-    def __init__(self, default: bool=False):
+    def __init__(self, default: bool = False):
         super().__init__()
 
         if default:
             self.fromdefault()
         else:
             self.name = ""
             self.set_type("footnote")
@@ -92,15 +93,15 @@
         # if numtype.lower() in NoteStyle.keys():
         if numtype.lower() in xmlc.num_type_xml.keys():
             self.num_type = numtype.lower()
             return True
 
         return False
 
-    def set_type(self, note_type: str="footnote") -> NoReturn:
+    def set_type(self, note_type: str = "footnote") -> NoReturn:
         if note_type.lower() == "footnote":
             self.is_endnotes = False
             self.is_footnotes = True
         else:
             self.is_endnotes = True
             self.is_footnotes = False
 
@@ -254,35 +255,36 @@
         if self.style_type in ["paragraph", "character"]:
             # TODO FIXME Handle font features as a dict instead
             # of a list, like in other styles
             # Features: -clig, inherit
 
             self.font = {
                 "name": "",
-                "size": 0,
+                "size": dimensions.Dim(0, unit="pt"),
                 "features": [],
                 "color": "",
                 "alignment": "left",
                 "strike": {"width": None, "offset": None},
                 "underline": {"width": None, "offset": None},
                 "shadow": {"hoffset": None, "voffset": None},
                 # NOTE There is no offset setting for outline, obviously
                 "outline": {"width": None},
+                "kerning": None,
             }
 
             # NOTE Weird, but FONTFEATURES is not the same as FEATURES
             # even if it has obviously an effect on fonts...
             self.features = {}
 
             self.lang = None
             self.shortcut = None
 
             self.background = {
                 "color": "None",
-                "shade": dimensions.Dim(100, unit="pc", integer=True)
+                "shade": dimensions.Dim(100, unit="pc", integer=True),
             }
 
         if self.style_type in ["table", "cell", "character", "paragraph"]:
             self.fill = {"color": None, "shade": None}
 
         if self.style_type in ["table", "cell"]:
             self.borders = []
@@ -295,15 +297,15 @@
             self.character_parent = ""
 
             self.space = {
                 "after": None,
                 "before": None,
             }
 
-            self.leading = {"mode": None, "value": dimensions.Dim(0)}
+            self.leading = {"mode": "fixed", "value": dimensions.Dim(0)}
 
         if default:
             self.fromdefault()
 
         if kwargs:
             self._quick_setup(kwargs)
 
@@ -356,21 +358,23 @@
 
         return False
 
     def fromdefault(self) -> bool:
         self.name = StyleAbstract.default_name[self.style_type]
 
         if self.style_type in ["paragraph", "character"]:
-            self.font = StyleAbstract.default_font
+            self.font |= StyleAbstract.default_font
 
         # TODO Le reste
 
         return True
 
-    def fromxml(self, xml: ET.Element, onlybool: bool=False) -> BoolOrElement:
+    def fromxml(
+        self, xml: ET.Element, onlybool: bool = False
+    ) -> BoolOrElement:
 
         if xml.tag != StyleAbstract.type_xml[self.style_type]:
             return False
 
         # Name -------------------------------------------------
 
         if self.style_type in ["paragraph", "table", "cell", "character"]:
@@ -394,22 +398,15 @@
 
         # Specific attributes for table ------------------------
 
         if self.style_type == "table":
             pass
 
         # Specific attributes for cell -------------------------
-
-        if self.style_type == "cell":
-
-            for case in ["left", "right", "top", "bottom"]:
-                att = xml.get("{}Padding".format(case.capitalize()))
-
-                if att is not None:
-                    self.padding[case] = att
+        # Moved in CellStyle
 
         # Common attributes to paragraphs + characters ---------
 
         if self.style_type in ["paragraph", "character"]:
 
             bshade_att = self._choose_att(StyleAbstract.bg_shade_xml)
             bcolor_att = self._choose_att(StyleAbstract.bg_color_xml)
@@ -426,15 +423,15 @@
 
             font = xml.get("FONT")
             if font is not None:
                 self.font["name"] = font
 
             font_size = xml.get("FONTSIZE")
             if font_size is not None:
-                self.font["size"] = float(font_size)
+                self.font["size"].value = float(font_size)
 
             font_features = xml.get("FONTFEATURES")
             if font_features is not None:
                 self.font["features"] = font_features.split(",")
 
             font_color = xml.get("FCOLOR")
             if font_color is not None:
@@ -483,14 +480,20 @@
 
             outline_width = xml.get("TXTOUT")
             if outline_width is not None:
                 self.font["outline"]["width"] = dimensions.Dim(
                     float(outline_width), unit="pcdecim"
                 )
 
+            kerning = xml.get("KERN")
+            if kerning is not None:
+                self.font["kerning"] = dimensions.Dim(
+                    float(kerning), unit="pc"
+                )
+
             # Lang ---------------------------------------------------
 
             lang = xml.get("LANGUAGE")
             if lang is not None:
                 if lang:
                     self.lang = lang
 
@@ -504,15 +507,15 @@
                     self.parent = parent
 
             # Shortcut -----------------------------------------------
 
             shortcut_att = self._choose_att(StyleAbstract.shortcut_xml)
 
             shortcut = xml.get(shortcut_att)
-            if shortcut = xml.get(shortcut_att)
+            if shortcut is not None:
                 if shortcut:
                     self.shortcut = shortcut
 
         # Common attributes to tables, celles, characters ------
 
         if self.style_type in ["table", "cell", "character", "paragraph"]:
             fshade_att = self._choose_att(StyleAbstract.fshade_xml)
@@ -563,37 +566,34 @@
             xml.attrib["DefaultStyle"] = xmlc.bool_to_num(self.is_default)
 
         # Specific attributes for table ------------------------
 
         if self.style_type == "table":
             pass
 
-        # Specific attributes for cell -------------------------
-
-        if self.style_type == "cell":
-
-            for case in ["left", "right", "top", "bottom"]:
-                att_name = "{}Padding".format(case.capitalize())
-                xml.attrib[att_name] = self.padding[case]
-
         # Common attributes to paragraphs + characters ---------
 
         if self.style_type in ["paragraph", "character"]:
 
             bshade_att = self._choose_att(StyleAbstract.bg_shade_xml)
             bcolor_att = self._choose_att(StyleAbstract.bg_color_xml)
 
-            xml.attrib[bcolor_att] = self.background["color"]
-            xml.attrib[bshade_att] = self.background["shade"].toxmlstr(True)
+            if self.background["color"] == "None":
+                xml.attrib[bcolor_att] = "None"
+            else:
+                xml.attrib[bcolor_att] = self.background["color"]
+
+            if self.background["shade"].value <= 100:
+                xml.attrib[bshade_att] = self.background["shade"].toxmlstr(True)
 
             if self.font["name"]:
                 xml.attrib["FONT"] = self.font["name"]
 
             if self.style_type == "character":
-                xml.attrib["FONTSIZE"] = str(self.font["size"])
+                xml.attrib["FONTSIZE"] = self.font["size"].toxmlstr(True)
 
             # TODO FIXME Handle font features as a dict instead
             # of a list, like in other styles
             # xml.attrib["FONTFEATURES"] = " ".join(self.font["features"].keys())
 
             if self.font["features"]:
                 xml.attrib["FONTFEATURES"] = ",".join(self.font["features"])
@@ -632,14 +632,17 @@
                 ].toxmlstr(True)
 
             if self.font["underline"]["offset"] is not None:
                 xml.attrib["TXTULP"] = self.font["underline"][
                     "offset"
                 ].toxmlstr(True)
 
+            if self.font["kerning"] is not None:
+                xml.attrib["KERN"] = self.font["kerning"].toxmlstr(True)
+
             if self.features:
                 xml.attrib["FEATURES"] = self.features
 
             if self.lang is not None:
                 xml.attrib["LANGUAGE"] = self.lang
 
             if self.shortcut is not None:
@@ -682,15 +685,15 @@
 
         except AttributeError:
             # NOTE If fromxml was not used
             pass
 
         return xml
 
-    def fromstyle(self, style, override: bool=False):
+    def fromstyle(self, style, override: bool = False):
         """
         Set attributes according to another style.
 
         :type style: ParagraphStyle, CharacterStyle, ...
         :param style: Style to load attributes from.
         :type override: boolean
         :param override: Override attributes that differs from style
@@ -772,27 +775,44 @@
 
     glyph_scale_xml = {
         "max": "MaxGlyphExtend",
         "min": "MinGlyphShrink",
     }
 
     optical_margins_xml = {
-        "both": 14,
-        "left": 4,
-        "right": 8,
-        "none": 0,
-        "undef": None
+        "both": "14",
+        "left": "4",
+        "right": "8",
+        "none": "0",
+        "undef": None,
+    }
+
+    ol_types = {
+        "decimal": "0",
+        "decimal-ar": "1",
+        "lower-roman": "2",
+        "upper-roman": "3",
+        "lower-latin": "4",
+        "upper-latin": "5",
+        "alpha-ar": "6",
+        "abjad-ar": "7",
+        # SEUL CONTRE LES DIEUX CONTRE L'ODIEUX CESAR
+        "asterix": "8",
+        "cjk": "9",
+        "hebrew": "10",
     }
 
     def __init__(self, doc_parent, default=False, **kwargs):
         StyleAbstract.__init__(self, "paragraph", doc_parent, default)
 
         self.indentations = {"left": None, "right": None, "first-line": None}
 
-        self.listing = {"type": None, "char": None}
+        self.listing = {"type": None, "char": None, "subtype": None}
+
+        self.hyphen_following_lines = None
 
         self.glyph_scaling = {
             "min": dimensions.Dim(1.0, unit="pcscale"),
             "max": dimensions.Dim(1.0, unit="pcscale"),
         }
 
         self.initial = {
@@ -814,499 +834,47 @@
 
     def fromxml(self, xml: ET.Element) -> bool:
         is_paragraph = StyleAbstract.fromxml(self, xml, True)
 
         if not is_paragraph:
             return False
 
-        # Text direction ------------------------------------------------
-
-        text_direction = xml.get("DIRECTION")
-        if text_direction is not None:
-
-            if xmlc.num_to_bool(text_direction):
-                self.text_direction = TextDirection.RTL
-            else:
-                self.text_direction = TextDirection.LTR
-
-        # Optical margins -----------------------------------------------
-
-        optic_margin = xml.get("OpticalMargins")
-
-        for human, value in ParagraphStyle.optical_margins_xml.items():
-            if value == optic_margin:
-                self.optical_margins = human
-
-        # Initial capital (aka drop capital) ----------------------------
-
-        initial_used = xml.get("DROP")
-        if initial_used is not None:
-            self.initial["active"] = xmlc.num_to_bool(initial_used)
-
-        initial_lines = xml.get("DROPLIN")
-        if initial_lines is not None:
-            self.initial["lines"] = int(initial_lines)
-
-        initial_indent = xml.get("ParagraphEffectIndent")
-        if initial_indent is not None:
-            self.initial["auto_indent"] = xmlc.num_to_bool(initial_indent)
-
-        for att_name in ["ParagraphEffectOffset", "DROPDIST"]:
-            initial_offset = xml.get(att_name)
-            if initial_offset is not None:
-                self.initial["__offset_att"] = att_name
-                self.initial["offset"].value = float(initial_offset)
-                break
-
-        # Glyph scaling -------------------------------------------------
-
-        mgs = xml.get("MinGlyphShrink")
-        if mgs is not None:
-            self.glyph_scaling["min"].value = float(mgs)
-
-        mge = xml.get("MaxGlyphExtend")
-        if mge is not None:
-            self.glyph_scaling["max"].value = float(mge)
-
-        # Indentation ---------------------------------------------------
-
-        # Left indentation of all paragraph lines
-
-        left = xml.get("INDENT")
-        if left is not None:
-            self.indentations["left"] = dimensions.Dim(float(left))
-
-        # Right indentation of all paragraph lines
-
-        right = xml.get("RMARGIN")
-        if right is not None:
-            self.indentations["right"] = dimensions.Dim(float(right))
-
-        # Indentation of the first line of the paragraph
-
-        first = xml.get("FIRST")
-        if first is not None:
-            self.indentations["first-line"] = dimensions.Dim(
-                float(first), negative=True
-            )
-
-        # Lists ---------------------------------------------------------
-
-        is_ul, is_ol = False, False
-
-        is_bullet = xml.get("Bullet")
-        if is_bullet is not None:
-            if is_bullet == "1":
-                self.listing["type"] = "ul"
-                is_ul = True
-
-        is_numeroted = xml.get("Numeration")
-        if is_numeroted is not None:
-            if is_numeroted == "1":
-                self.listing["type"] = "ol"
-                is_ol = True
-
-        if is_ol and is_ul:
-            raise exceptions.InsaneSLAValue(
-                "Style {} is both bullet and numeroted list.".format(self.name)
-            )
-
-        bullet_char = xml.get("BulletStr")
-        if bullet_char is not None:
-            self.listing["char"] = bullet_char
-
-        # Parent character style ----------------------------------------
-
-        character_parent = xml.get("CPARENT")
-        if character_parent is not None:
-            self.character_parent = character_parent
-
-        # Leading -------------------------------------------------------
-
-        leading = xml.get("LINESPMode")
-        if leading is not None:
-
-            for human, code in ParagraphStyle.leading_xml.items():
-                if leading == code:
-                    self.leading["mode"] = human
-                    break
-
-            if self.leading["mode"] == "fixed":
-                leading_value = xml.get("LINESP")
-
-                if leading_value is not None:
-                    self.leading["value"].value = float(leading_value)
-
-        # Alignment -----------------------------------------------------
-
-        alignment = xml.get("ALIGN")
-        if alignment is not None:
-            for human, code in xmlc.alignment.items():
-                if alignment == code:
-                    self.font["alignment"] = human
-                    break
-
-        # Spaces before and after paragraph -----------------------------
-
-        for case in [["VOR", "before"], ["NACH", "after"]]:
-
-            space_att = xml.get(case[0])
-            if space_att is not None:
-                self.space[case[1]] = dimensions.Dim(float(space_att))
-
-        # Tabs ----------------------------------------------------------
-
-        for child in xml:
-
-            if child.tag == "Tabs":
-                to = StyleTab()
-
-                success = to.fromxml(child)
-                if success:
-                    self.tabs.append(to)
-
-        # End of parsing ------------------------------------------------
-
-        self.undocumented = xmlc.all_undocumented_to_python(xml)
-
-        return True
-
-    def toxml(self) -> ET.Element:
-        xml = StyleAbstract.toxml(self)
-
-        # Text direction ------------------------------------------------
-
-        xml.attrib["DIRECTION"] = str(int(self.text_direction))
-
-        # Optical margins -----------------------------------------------
-
-        if self.optical_margins is not None:
-            xml.attrib["OpticalMargins"] = str(
-                ParagraphStyle.optical_margins_xml[self.optical_margins]
-            )
-
-        # Initial capital (aka drop capital) ----------------------------
-
-        xml.attrib["DROP"] = xmlc.bool_to_num(self.initial["active"])
-        xml.attrib["DROPLIN"] = str(self.initial["lines"])
-
-        xml.attrib[self.initial["__offset_att"]] = self.initial["offset"].toxmlstr()
-
-        if self.initial["auto_indent"]:
-            xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(self.initial["auto_indent"] )
-
-        # Glyph scaling ---------------------------------------------
-
-        for human, att in ParagraphStyle.glyph_scale_xml.items():
-            if self.glyph_scaling[human].value != 1.0:
-                xml.attrib[att] = self.glyph_scaling[human].toxmlstr()
-
-        # -----------------------------------------------------------
-
-        xml.attrib["ALIGN"] = xmlc.alignment[self.font["alignment"]]
-
-        if self.leading["mode"] is not None:
-            xml.attrib["LINESPMode"] = ParagraphStyle.leading_xml[
-                self.leading["mode"]
-            ]
-
-            if self.leading["mode"] == "fixed":
-                xml.attrib["LINESP"] = self.leading["value"].toxmlstr()
-
-        # Indentation -----------------------------------------------
-
-        for case in [
-            ["left", "INDENT"],
-            ["right", "RMARGIN"],
-            ["first-line", "FIRST"],
-        ]:
-
-            if self.indentations[case[0]] is None:
-                xml.attrib[case[1]] = "0"
-            else:
-                xml.attrib[case[1]] = self.indentations[case[0]].toxmlstr()
-
-        # Lists ---------------------------------------------------------
-
-        if self.listing["type"] == "ol":
-            att_seq = [False, True]
-        elif self.listing["type"] == "ul":
-            att_seq = [True, False]
-        else:
-            att_seq = [False, False]
-
-        for case in zip(att_seq, ["Bullet", "Numeration"]):
-            xml.attrib[case[1]] = xmlc.bool_to_num(case[0])
-
-        xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
-
-        # Parent character style ------------------------------------
-
-        # NOTE To not confuse with parent paragraph style which is
-        # in @PARENT, and handled in StyleAbstract
-
-        if self.character_parent:
-            xml.attrib["CPARENT"] = self.character_parent
-
-        for case in [["before", "VOR"], ["after", "NACH"]]:
-            if self.space[case[0]] is not None:
-                xml.attrib[case[1]] = self.space[case[0]].toxmlstr(True)
-
-        # xml.attrib["VOR"] = self.space["before"].toxmlstr()
-        # xml.attrib["NACH"] = self.space["after"].toxmlstr()
-
-        # FONT SIZE -------------------------------------------------
-
-        font_size = str(self.font["size"])
-
-        if self.character_parent and font_size == "0":
-            # If the font size of the paragraph is not defined
-            # because it is defined in a parent character style,
-            # don't write FONTSIZE attribute
-            pass
-        else:
-            if font_size != "0":
-                xml.attrib["FONTSIZE"] = font_size
-
-        # -----------------------------------------------------------
-
-        try:
-            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
-                xml,
-                self.undocumented,
-                True,
-                self.style_type + " style " + self.name,
-                logger=logs.getLogger(),
-            )
-
-        except AttributeError:
-            # NOTE If fromxml was not used
-            pass
-
-        return xml
-
-    def fromdefault(self) -> bool:
-        StyleAbstract.fromdefault(self)
-
-        self.leading = {"mode": None, "value": dimensions.Dim(12)}
-
-        return True
-
-    def _quick_setup(self, settings: dict) -> NoReturn:
-        """
-        Method for defining style settings from class
-        instanciation kwargs.
-
-        :type settings: dict
-        :param settings: Kwargs dictionnary
-        """
-
-        if not settings:
-            return
-
-        StyleAbstract._quick_setup(self, settings)
-
-        for setting_name, setting_value in settings.items():
-
-            if setting_name == "direction":
-                setting_value = setting_value.strip().lower()
-
-                if setting_value in ["ltr", "rtl"]:
-                    if setting_value == "ltr":
-                        self.text_direction = TextDirection.LTR
-                    else:
-                        self.text_direction = TextDirection.RTL
-                else:
-                    raise ValueError(
-                        "Wrong direction setting '{}'. "
-                        "Use either 'ltr' (left to right) 'rtl' "
-                        "(right to left).".format(setting_value)
-                    )
-
-            if setting_name == "spacebefore":
-                self.space["before"] = dimensions.Dim(float(setting_value))
-
-            if setting_name == "spaceafter":
-                self.space["after"] = dimensions.Dim(float(setting_value))
-
-            if setting_name == "cparent":
-                self.character_parent = setting_value
-
-            if setting_name == "leading":
-                if setting_value in ParagraphStyle.leading_xml:
-                    self.leading["mode"] = setting_value
-
-            if setting_name == "leadingValue":
-                self.leading["value"] = dimensions.Dim(
-                    float(setting_value)
-                )
-
-            if setting_name == "alignment":
-
-                if setting_value.lower() in xmlc.alignment.keys():
-                    self.font["alignment"] = setting_value
-                else:
-                    raise ValueError(
-                        "Wrong alignement setting '{}'. "
-                        "Alignement setting must be {}".format(
-                            setting_value, ", ".join(xmlc.alignment.keys())
-                        )
-                    )
-
-    def set_leadingmode(self, leadingmode: LeadingMode) -> bool:
-        """
-        Set leading mode.
-
-        :type leadingmode: string
-        :param leadingmode: "fixed", "automatic", "grid"
-        """
-
-        if leadingmode.lower() in ParagraphStyle.leading_xml:
-            self.leading["mode"] = leadingmode
-            return True
-
-        raise ValueError()
-
-
-class ParagraphStyle(StyleAbstract):
-    """
-    Paragraph style in SLA (STYLE)
-
-    :type default: boolean
-    :param default: Use default settings (False by default)
-    :type kwargs: dict
-    :param kwargs: Quick setting (see kwargs table)
-
-    +--------------+------------------------------------+
-    | Kwargs       | Setting                            |
-    +==============+====================================+
-    | name         | Style name                         |
-    +--------------+------------------------------------+
-    | defaultstyle | Scribus default paragraph style?   |
-    +--------------+------------------------------------+
-    | parent       | Parent style name (paragraph)      |
-    +--------------+------------------------------------+
-    | cparent      | Parent style name (character)      |
-    +--------------+------------------------------------+
-    | alignment    | Text alignment. Must be in         |
-    |              | ``pyscribus.common.xml.alignment`` |
-    |              | keys                               |
-    +--------------+------------------------------------+
-    | direction    | Text direction. Either "ltr"       |
-    |              | (left to right) or "rtl" (right to |
-    |              | left.                              |
-    +--------------+------------------------------------+
-    | font         | Font name                          |
-    +--------------+------------------------------------+
-    | fontsize     | Font size                          |
-    +--------------+------------------------------------+
-    | spacebefore  | Space before paragraph             |
-    +--------------+------------------------------------+
-    | spaceafter   | Space after paragraph              |
-    +--------------+------------------------------------+
-    | leading      | Leading mode. Must be in           |
-    |              | ``ParagraphStyle.leading_xml``.    |
-    |              | If "fixed" mode, you must define   |
-    |              | leadingValue setting.              |
-    +--------------+------------------------------------+
-    | leadingValue | Leading value in pica points if    |
-    |              | leading mode is "fixed".           |
-    +--------------+------------------------------------+
-    | default      | Equivalent to a fromdefault        |
-    |              | call, value being True or the      |
-    |              | default name                       |
-    +--------------+------------------------------------+
-
-    :Example:
-
-    .. code:: python
-
-       title_style = styles.ParagraphStyle(
-           name="Title", fontsize=18, alignment="center",
-           leading="fixed", leadingValue=16
-       )
-
-       normal_style = styles.ParagraphStyle(
-           name="Normal", fontsize=12, alignment="justify",
-           leading="automatic"
-       )
-
-    """
-
-    leading_xml = {
-        "fixed": "0",
-        "automatic": "1",
-        "grid": "2",
-    }
-
-    glyph_scale_xml = {
-        "max": "MaxGlyphExtend",
-        "min": "MinGlyphShrink",
-    }
-
-    optical_margins_xml = {
-        "both": 14,
-        "left": 4,
-        "right": 8,
-        "none": 0,
-        "undef": None
-    }
-
-    def __init__(self, doc_parent, default=False, **kwargs):
-        StyleAbstract.__init__(self, "paragraph", doc_parent, default)
-
-        self.indentations = {"left": None, "right": None, "first-line": None}
-
-        self.listing = {"type": None, "char": None}
-
-        self.glyph_scaling = {
-            "min": dimensions.Dim(1.0, unit="pcscale"),
-            "max": dimensions.Dim(1.0, unit="pcscale"),
-        }
-
-        self.initial = {
-            "active": False,
-            "lines": 2,
-            "offset": dimensions.Dim(0),
-            # NOTE The initial capital offset is documented as @DROPDIST but
-            # implemented as @ParagraphEffectOffset so we store the attribute
-            # used in the file for later.
-            "__offset_att": "paragrapheffectoffset",
-            # NOTE If there no auto_indent set, the value is not saved in SLA file.
-            "auto_indent": False,
-        }
-
-        self.optical_margins = ParagraphStyle.optical_margins_xml["undef"]
-        self.text_direction = TextDirection.LTR
-
-        self._quick_setup(kwargs)
+        # Hyphenation ---------------------------------------------------
 
-    def fromxml(self, xml: ET.Element) -> bool:
-        is_paragraph = StyleAbstract.fromxml(self, xml, True)
+        hyphen_lines = xml.get("HyphenConsecutiveLines")
+        if hyphen_lines is not None:
+            try:
+                hyphen_lines = int(hyphen_lines)
 
-        if not is_paragraph:
-            return False
+                self.hyphen_following_lines = hyphen_lines
+            except ValueError:
+                self.hyphen_following_lines = 2
 
         # Text direction ------------------------------------------------
 
         text_direction = xml.get("DIRECTION")
         if text_direction is not None:
 
             if xmlc.num_to_bool(text_direction):
                 self.text_direction = TextDirection.RTL
             else:
                 self.text_direction = TextDirection.LTR
 
         # Optical margins -----------------------------------------------
 
         optic_margin = xml.get("OpticalMargins")
+        if optic_margin is None:
+            self.optical_margins = "undef"
+        else:
+            for human, value in ParagraphStyle.optical_margins_xml.items():
+                if value is None or value != optic_margin:
+                    continue
 
-        for human, value in ParagraphStyle.optical_margins_xml.items():
-            if value == optic_margin:
                 self.optical_margins = human
+                break
 
         # Initial capital (aka drop capital) ----------------------------
 
         initial_used = xml.get("DROP")
         if initial_used is not None:
             self.initial["active"] = xmlc.num_to_bool(initial_used)
 
@@ -1342,15 +910,15 @@
         left = xml.get("INDENT")
         if left is not None:
             self.indentations["left"] = dimensions.Dim(float(left))
 
         # Right indentation of all paragraph lines
 
         right = xml.get("RMARGIN")
-        if right is not None:
+        if righ is not None:
             self.indentations["right"] = dimensions.Dim(float(right))
 
         # Indentation of the first line of the paragraph
 
         first = xml.get("FIRST")
         if first is not None:
             self.indentations["first-line"] = dimensions.Dim(
@@ -1369,14 +937,22 @@
 
         is_numeroted = xml.get("Numeration")
         if is_numeroted is not None:
             if is_numeroted == "1":
                 self.listing["type"] = "ol"
                 is_ol = True
 
+        num_format = xml.get("NumerationFormat")
+        if num_format is not None:
+            if is_ol:
+                for human, code in ParagraphStyle.ol_types.items():
+                    if code == num_format:
+                        self.listing["subtype"] = human
+                        break
+
         if is_ol and is_ul:
             raise exceptions.InsaneSLAValue(
                 "Style {} is both bullet and numeroted list.".format(self.name)
             )
 
         bullet_char = xml.get("BulletStr")
         if bullet_char is not None:
@@ -1394,19 +970,23 @@
         if leading is not None:
 
             for human, code in ParagraphStyle.leading_xml.items():
                 if leading == code:
                     self.leading["mode"] = human
                     break
 
-            if self.leading["mode"] == "fixed":
-                leading_value = xml.get("LINESP")
+        leading_value = xml.get("LINESP")
+        if leading_value is not None:
+            # NOTE Leading value unit is pica in fixed mode, in points in
+            #      automatic mode.
+            if self.leading["mode"] == "automatic":
+                self.leading["value"].set_unit("pt")
 
-                if leading_value is not None:
-                    self.leading["value"].value = float(leading_value)
+            if self.leading["mode"] in ["fixed", "automatic"]:
+                self.leading["value"].value = float(leading_value)
 
         # Alignment -----------------------------------------------------
 
         alignment = xml.get("ALIGN")
         if alignment is not None:
             for human, code in xmlc.alignment.items():
                 if alignment == code:
@@ -1441,30 +1021,42 @@
     def toxml(self) -> ET.Element:
         xml = StyleAbstract.toxml(self)
 
         # Text direction ------------------------------------------------
 
         xml.attrib["DIRECTION"] = str(int(self.text_direction))
 
+        # Hyphenation ---------------------------------------------------
+
+        if self.hyphen_following_lines is not None:
+            xml.attrib["HyphenConsecutiveLines"] = str(
+                self.hyphen_following_lines
+            )
+
         # Optical margins -----------------------------------------------
 
         if self.optical_margins is not None:
-            xml.attrib["OpticalMargins"] = str(
-                ParagraphStyle.optical_margins_xml[self.optical_margins]
-            )
+            if self.optical_margins != "undef":
+                xml.attrib["OpticalMargins"] = str(
+                    ParagraphStyle.optical_margins_xml[self.optical_margins]
+                )
 
         # Initial capital (aka drop capital) ----------------------------
 
         xml.attrib["DROP"] = xmlc.bool_to_num(self.initial["active"])
         xml.attrib["DROPLIN"] = str(self.initial["lines"])
 
-        xml.attrib[self.initial["__offset_att"]] = self.initial["offset"].toxmlstr()
+        xml.attrib[self.initial["__offset_att"]] = self.initial[
+            "offset"
+        ].toxmlstr(True)
 
         if self.initial["auto_indent"]:
-            xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(self.initial["auto_indent"] )
+            xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(
+                self.initial["auto_indent"]
+            )
 
         # Glyph scaling ---------------------------------------------
 
         for human, att in ParagraphStyle.glyph_scale_xml.items():
             if self.glyph_scaling[human].value != 1.0:
                 xml.attrib[att] = self.glyph_scaling[human].toxmlstr()
 
@@ -1473,43 +1065,50 @@
         xml.attrib["ALIGN"] = xmlc.alignment[self.font["alignment"]]
 
         if self.leading["mode"] is not None:
             xml.attrib["LINESPMode"] = ParagraphStyle.leading_xml[
                 self.leading["mode"]
             ]
 
-            if self.leading["mode"] == "fixed":
-                xml.attrib["LINESP"] = self.leading["value"].toxmlstr()
+        if self.leading["mode"] in ["fixed", "automatic"]:
+            if self.leading["value"].value > 0:
+                xml.attrib["LINESP"] = self.leading["value"].toxmlstr(True)
 
         # Indentation -----------------------------------------------
 
         for case in [
             ["left", "INDENT"],
             ["right", "RMARGIN"],
             ["first-line", "FIRST"],
         ]:
 
             if self.indentations[case[0]] is None:
                 xml.attrib[case[1]] = "0"
             else:
-                xml.attrib[case[1]] = self.indentations[case[0]].toxmlstr()
+                xml.attrib[case[1]] = self.indentations[case[0]].toxmlstr(True)
 
         # Lists ---------------------------------------------------------
 
         if self.listing["type"] == "ol":
             att_seq = [False, True]
         elif self.listing["type"] == "ul":
             att_seq = [True, False]
         else:
             att_seq = [False, False]
 
-        for case in zip(att_seq, ["Bullet", "Numeration"]):
-            xml.attrib[case[1]] = xmlc.bool_to_num(case[0])
+        for list_val, list_att in zip(att_seq, ["Bullet", "Numeration"]):
+            xml.attrib[list_att] = xmlc.bool_to_num(list_val)
 
-        xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
+        if self.listing["type"] == "ol":
+            xml.attrib["NumerationFormat"] = ParagraphStyle.ol_types[
+                self.listing["subtype"]
+            ]
+
+        if self.listing["type"] is not None:
+            xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
 
         # Parent character style ------------------------------------
 
         # NOTE To not confuse with parent paragraph style which is
         # in @PARENT, and handled in StyleAbstract
 
         if self.character_parent:
@@ -1520,24 +1119,26 @@
                 xml.attrib[case[1]] = self.space[case[0]].toxmlstr(True)
 
         # xml.attrib["VOR"] = self.space["before"].toxmlstr()
         # xml.attrib["NACH"] = self.space["after"].toxmlstr()
 
         # FONT SIZE -------------------------------------------------
 
-        font_size = str(self.font["size"])
+        font_size = str(self.font["size"]).strip()
 
-        if self.character_parent and font_size == "0":
-            # If the font size of the paragraph is not defined
-            # because it is defined in a parent character style,
-            # don't write FONTSIZE attribute
-            pass
-        else:
-            if font_size != "0":
-                xml.attrib["FONTSIZE"] = font_size
+        if font_size != "0":
+            xml.attrib["FONTSIZE"] = str(
+                mathc.necessary_float(float(font_size))
+            )
+
+            if self.character_parent:
+                # If the font size of the paragraph is not defined
+                # because it is defined in a parent character style,
+                # don't write FONTSIZE attribute
+                pass
 
         # -----------------------------------------------------------
 
         try:
             xml, undoc_attribs = xmlc.all_undocumented_to_xml(
                 xml,
                 self.undocumented,
@@ -1600,17 +1201,15 @@
                 self.character_parent = setting_value
 
             if setting_name == "leading":
                 if setting_value in ParagraphStyle.leading_xml:
                     self.leading["mode"] = setting_value
 
             if setting_name == "leadingValue":
-                self.leading["value"] = dimensions.Dim(
-                    float(setting_value)
-                )
+                self.leading["value"] = dimensions.Dim(float(setting_value))
 
             if setting_name == "alignment":
 
                 if setting_value.lower() in xmlc.alignment.keys():
                     self.font["alignment"] = setting_value
                 else:
                     raise ValueError(
@@ -1663,23 +1262,22 @@
     |              | the default name.           |          |
     +--------------+-----------------------------+----------+
     """
 
     scale_xml = {
         "SCALEH": "horizontal",
         "SCALEV": "vertical",
-        "BASEO": "baseline_offset"
+        "BASEO": "baseline_offset",
     }
 
     def __init__(self, doc_parent, default=False, **kwargs):
         StyleAbstract.__init__(self, "character", doc_parent, default)
         StyleAbstract._quick_setup(self, kwargs)
 
         self.font["space_width"] = dimensions.Dim(1, unit="pcdecim")
-        self.font["kerning"] = None
 
         self.hyphen_word_min = None
 
         self.scale = {
             "horizontal": 100,
             "vertical": 100,
             "baseline_offset": 0,
@@ -1731,18 +1329,14 @@
 
         wordtrack = xml.get("wordTrack")
         if wordtrack is not None:
             self.font["space_width"] = dimensions.Dim(
                 float(wordtrack), unit="pcdecim"
             )
 
-        kerning = xml.get("KERN")
-        if kerning is not None:
-            self.font["kerning"] = dimensions.Dim(float(kerning), unit="pc")
-
         # Scales --------------------------------------------------------
 
         for att, human in CharacterStyle.scale_xml.items():
             scale_att = xml.get(att)
             if scale_att is not None:
                 self.scale[human] = float(scale_att)
 
@@ -1754,30 +1348,27 @@
 
     def toxml(self) -> ET.Element:
         xml = StyleAbstract.toxml(self)
 
         # Stroke settings -----------------------------------------------
 
         xml.attrib["SCOLOR"] = self.stroke["color"]
-        xml.attrib["SSHADE"] = self.stroke["shade"].toxmlstr()
+        xml.attrib["SSHADE"] = self.stroke["shade"].toxmlstr(True)
 
         # Hyphenation ---------------------------------------------------
 
         if self.hyphen_word_min is not None:
             xml.attrib["HyphenWordMin"] = str(self.hyphen_word_min)
 
         # Font settings -------------------------------------------------
 
         if self.font["space_width"] is not None:
             if self.font["space_width"].value != 1.0:
                 xml.attrib["wordTrack"] = self.font["space_width"].toxmlstr()
 
-        if self.font["kerning"] is not None:
-            xml.attrib["KERN"] = self.font["kerning"].toxmlstr(True)
-
         # Scales --------------------------------------------------------
 
         for att, human in CharacterStyle.scale_xml.items():
             xml.attrib[att] = str(mathc.necessary_float(self.scale[human]))
 
         # ---------------------------------------------------------------
 
@@ -1826,47 +1417,14 @@
         for border in self.borders:
             bx = border.toxml()
             xml.append(bx)
 
         return xml
 
 
-class TabularStyleAbstract(StyleAbstract):
-    """Abstract middle class for Table and Cell styles."""
-
-    def __init__(self, style_type, doc_parent, default=False, **kwargs):
-        StyleAbstract.__init__(self, style_type, doc_parent, default)
-
-    def fromxml(self, xml) -> bool:
-        x = StyleAbstract.fromxml(self, xml)
-
-        if len(x) == 0:
-            return False
-
-        for border in x:
-
-            if border.tag in TableBorder.sides_xml.values():
-                tb = TableBorder()
-
-                success = tb.fromxml(border)
-                if success:
-                    self.borders.append(tb)
-
-        return True
-
-    def toxml(self) -> ET.Element:
-        xml = StyleAbstract.toxml(self)
-
-        for border in self.borders:
-            bx = border.toxml()
-            xml.append(bx)
-
-        return xml
-
-
 class TableBorder(xmlc.PyScribusElement):
     """
     Table border settings in SLA
     (TableBorderLeft, TableBorderRight, TableBorderTop, TableBorderBottom)
 
     :type side: str
     :param side: (Cell) Side of the border
@@ -1875,15 +1433,15 @@
     sides_xml = {
         "left": "TableBorderLeft",
         "right": "TableBorderRight",
         "top": "TableBorderTop",
         "bottom": "TableBorderBottom",
     }
 
-    def __init__(self, side: Optional[str]=False):
+    def __init__(self, side: Optional[str] = False):
         super().__init__()
 
         if side:
             if side.lower() in TableBorder.sides_xml.keys():
                 self.side = side.lower()
             else:
                 self.side = False
@@ -2021,14 +1579,34 @@
     """
     Cell style in SLA (CellStyle)
     """
 
     def __init__(self, doc_parent, default=False, **kwargs):
         TabularStyleAbstract.__init__(self, "cell", doc_parent, default)
 
+    def fromxml(self, xml: ET.Element) -> BoolOrElement:
+        success = TabularStyleAbstract.fromxml(self, xml)
+
+        for case in ["left", "right", "top", "bottom"]:
+            att = xml.get("{}Padding".format(case.capitalize()))
+
+            if att is not None:
+                self.padding[case] = att
+
+        return True
+
+    def toxml(self) -> ET.Element:
+        xml = TabularStyleAbstract.toxml(self)
+
+        for case in ["left", "right", "top", "bottom"]:
+            att_name = "{}Padding".format(case.capitalize())
+            xml.attrib[att_name] = self.padding[case]
+
+        return xml
+
 
 class StyleTab(xmlc.PyScribusElement):
     tab_type_xml = {
         "left": "0",
         "right": "1",
         "period": "2",
         "comma": "3",
@@ -2197,16 +1775,15 @@
 
     def fromdefault(self) -> NoReturn:
         self.end = "flat"
         self.join = "pointy"
         self.opacity = dimensions.Dim(100, unit="pc")
 
     def fromxml(self, xml: ET.Element) -> bool:
-        """
-        """
+        """ """
 
         if xml.tag != "SubLine":
             return False
 
         # --- Shortcut -----------------------------------------------
 
         shortcut = xml.get("Shortcut")
@@ -2258,16 +1835,15 @@
                 if code == line_join:
                     self.join = human
                     break
 
         return True
 
     def toxml(self) -> ET.Element:
-        """
-        """
+        """ """
 
         xml = ET.Element("SubLine")
 
         # --- Color and opacity --------------------------------------
 
         if self.color is not None:
             xml.attrib["Color"] = self.color
@@ -2294,15 +1870,17 @@
 
         return xml
 
 
 # Fonctions =============================================================#
 
 
-def fromSLA(filepath: StringOrPath="", slastring: str="") -> Union[dict, bool]:
+def fromSLA(
+    filepath: StringOrPath = "", slastring: str = ""
+) -> Union[dict, bool]:
     """
     Parse a SLA file / string and returns a dictionary of all styles in it.
 
     :type filepath: string
     :param filepath: SLA filepath
     :type slastring: string
     :param slastring: SLA XML string
```

### Comparing `pyscribus-backported-0.2.4/pyscribus/toc.py` & `pyscribus-backported-0.3/pyscribus/model/toc.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,32 @@
 
 """
 Classes of PyScribus related to table of contents & sections
 """
 
 # Imports ===============================================================#
 
+# To avoid Sphinx complaints from methods annotations referencing same class
+from __future__ import annotations
+
+from typing import Union, NoReturn
+
 import lxml
 import lxml.etree as ET
 
-import pyscribus.common.xml as xmlc
+import pyscribus.model.common.xml as xmlc
+import pyscribus.model.exceptions as exceptions
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 # Classes ===============================================================#
 
+
 class Section(xmlc.PyScribusElement):
     """
     Section in SLA (Section).
     """
 
     def __init__(self):
         super().__init__()
@@ -46,136 +53,121 @@
         self.reversed = False
 
         self.name = ""
         self.number = 1
 
         self.range = {"from": 0, "to": 0}
 
-        self.numerotation = {
-            "type": "decimal",
-            "start": 1
-        }
-
-        self.fill = {
-            "width": 0,
-            "character": chr(0)
-        }
+        self.numerotation = {"type": "decimal", "start": 1}
 
-    def fromdefault(self):
+        self.fill = {"width": 0, "character": chr(0)}
+
+    def fromdefault(self) -> NoReturn:
         """
         Set default attributes for the section.
         """
 
         self.active = True
         self.reversed = False
 
         self.name = "0"
         self.number = 1
 
         self.range = {"from": 0, "to": 0}
 
-        self.numerotation = {
-            "type": "decimal",
-            "start": 1
-        }
-
-        self.fill = {
-            "width": 0,
-            "character": chr(0)
-        }
+        self.numerotation = {"type": "decimal", "start": 1}
+
+        self.fill = {"width": 0, "character": chr(0)}
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         :rtype: boolean
         :returns: True if parsing succeed
         """
 
-        if xml.tag == "Section":
+        if xml.tag != "Section":
+            return False
 
-            nam = xml.get("Name")
+        nam = xml.get("Name")
 
-            if nam is not None:
-                self.name = nam
+        if nam is not None:
+            self.name = nam
 
-            #------------------------------------------------------
+        # -----------------------------------------------------
 
-            rev = xml.get("Reversed")
-            act = xml.get("Active")
+        rev = xml.get("Reversed")
+        act = xml.get("Active")
 
-            if rev is not None:
-                self.reversed = xmlc.num_to_bool(rev)
+        if rev is not None:
+            self.reversed = xmlc.num_to_bool(rev)
 
-            if act is not None:
-                self.active = xmlc.num_to_bool(act)
+        if act is not None:
+            self.active = xmlc.num_to_bool(act)
 
-            #--- Section number -----------------------------------
+        # Section number --------------------------------------
 
-            num = xml.get("Number")
+        num = xml.get("Number")
 
-            if num is not None:
-                self.number = int(num) + 1
+        if num is not None:
+            self.number = int(num) + 1
 
-            #--- Page range ---------------------------------------
+        # Page range ------------------------------------------
 
-            for case in [["From", "from"], ["To", "to"]]:
-                att = xml.get(case[0])
+        for case in [["From", "from"], ["To", "to"]]:
+            att = xml.get(case[0])
 
-                if att is not None:
-                    self.range[case[1]] = int(att) + 1
+            if att is not None:
+                self.range[case[1]] = int(att) + 1
 
-            #--- Numerotation -------------------------------------
+        # Numerotation ----------------------------------------
 
-            num_type = xml.get("Type")
+        num_type = xml.get("Type")
 
-            if num_type is not None:
+        if num_type is not None:
 
-                for human,code in xmlc.num_type_xml.items():
+            for human, code in xmlc.num_type_xml.items():
 
-                    if code == num_type:
+                if code == num_type:
 
-                        self.numerotation["type"] = human
-                        break
+                    self.numerotation["type"] = human
+                    break
 
-            num_start = xml.get("Start")
+        num_start = xml.get("Start")
 
-            if num_start is not None:
-                self.numerotation["start"] = int(num_start)
+        if num_start is not None:
+            self.numerotation["start"] = int(num_start)
 
-            #--- Filling ------------------------------------------
+        # Filling ---------------------------------------------
 
-            fill_char = xml.get("FillChar")
+        fill_char = xml.get("FillChar")
 
-            if fill_char is not None:
+        if fill_char is not None:
 
-                try:
-                    self.fill["character"] = chr(int(fill_char))
+            try:
+                self.fill["character"] = chr(int(fill_char))
 
-                except ValueError:
-                    # NOTE Because python chr() argument must be in
-                    #      [0-1114111] range
+            except ValueError:
+                # NOTE Because python chr() argument must be in
+                #      [0-1114111] range
 
-                    raise exceptions.InsaneSLAValue(
-                        "Fill character in section '{}' "\
-                        "must range from 0 to 1114111.".format(
-                            self.name
-                        )
-                    )
+                raise exceptions.InsaneSLAValue(
+                    "Fill character in section '{}' "
+                    "must range from 0 to 1114111.".format(self.name)
+                )
 
-            field_width = xml.get("FieldWidth")
+        field_width = xml.get("FieldWidth")
 
-            if field_width is not None:
-                self.fill["width"] = int(field_width)
+        if field_width is not None:
+            self.fill["width"] = int(field_width)
 
-            #------------------------------------------------------
+        # -----------------------------------------------------
 
-            return True
-        else:
-            return False
+        return True
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         """
         :rtype: lxml.etree._Element
         :returns: XML representation of section
         """
         xml = ET.Element("Section")
 
         xml.attrib["Number"] = str(self.number - 1)
@@ -211,77 +203,76 @@
         self.name = ""
         self.frame_name = ""
         self.attribute = ""
         self.non_printing = False
         self.style = ""
         self.placement = "end"
 
-    def fromdefault(self):
+    def fromdefault(self) -> NoReturn:
         self.name = "Table of contents"
         self.placement = "end"
         self.non_printing = False
 
-    def toxml(self):
+    def toxml(self) -> ET.Element:
         toc = ET.Element("TableOfContents")
 
         toc.attrib["Name"] = self.name
         toc.attrib["ItemAttributeName"] = xmlc.str_or_nonestr(self.attribute)
         toc.attrib["FrameName"] = self.frame_name
         toc.attrib["ListNonPrinting"] = xmlc.bool_to_num(self.non_printing)
         toc.attrib["Style"] = self.style
         toc.attrib["NumberPlacement"] = TOC.placement_to_xml[self.placement]
 
         return toc
 
-    def fromxml(self, xml):
+    def fromxml(self, xml: ET.Element) -> bool:
         """
         :rtype: boolean
         :returns: True if parsing succeed
         """
 
-        if xml.tag == "TableOfContents":
+        if xml.tag != "TableOfContents":
+            return False
 
-            nam = xml.get("Name")
-            if nam is not None:
-                self.name = nam
+        nam = xml.get("Name")
+        if nam is not None:
+            self.name = nam
 
-            fnam = xml.get("FrameName")
-            if fnam is not None:
-                self.frame_name = fnam
+        fnam = xml.get("FrameName")
+        if fnam is not None:
+            self.frame_name = fnam
 
-            sn = xml.get("Style")
-            if sn is not None:
-                self.style = sn
+        sn = xml.get("Style")
+        if sn is not None:
+            self.style = sn
 
-            np = xml.get("ListNonPrinting")
-            if np is not None:
-                self.non_printing = xmlc.num_to_bool(np)
+        np = xml.get("ListNonPrinting")
+        if np is not None:
+            self.non_printing = xmlc.num_to_bool(np)
 
-            #--------------------------------------------------------
+        # -------------------------------------------------------
 
-            fattribute = xml.get("ItemAttributeName")
-            if fattribute is not None:
+        fattribute = xml.get("ItemAttributeName")
+        if fattribute is not None:
 
-                if fattribute == "None":
-                    self.attribute = ""
-                else:
-                    self.attribute = fattribute
+            if fattribute == "None":
+                self.attribute = ""
+            else:
+                self.attribute = fattribute
 
-            #--------------------------------------------------------
+        # -------------------------------------------------------
 
-            placement = xml.get("NumberPlacement")
-            if placement is not None:
+        placement = xml.get("NumberPlacement")
+        if placement is not None:
 
-                for human, code in TOC.placement_to_xml.items():
+            for human, code in TOC.placement_to_xml.items():
 
-                    if placement == code:
-                        self.placement = human
-                        break
+                if placement == code:
+                    self.placement = human
+                    break
 
-            #--------------------------------------------------------
+        # -------------------------------------------------------
 
-            return True
+        return True
 
-        else:
-            return False
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-backported-0.2.4/pyscribus_backported.egg-info/PKG-INFO` & `pyscribus-backported-0.3/pyscribus_backported.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: pyscribus-backported
-Version: 0.2.4
+Version: 0.3
 Summary: Read, create and update Scribus .sla files. (Python < 3.8 version)
 Author: Étienne Nadji
 Author-email: etnadji@eml.cc
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://etnadji.fr/pyscribus
-Project-URL: Source Code, https://framagit.org/etnadji/pyscribus/-/tree/backported
+Project-URL: Source Code, https://framagit.org/etnadji/pyscribus/-/tree/backported-model
 Project-URL: Issue tracker, https://framagit.org/etnadji/pyscribus/-/issues
 Keywords: scribus,sla
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Intended Audience :: Developers
 Requires-Python: <=3.7.9
 License-File: LICENSE
 
-######################
-PyScribus (backported)
-######################
+.. image:: https://etnadji.fr/pyscribus/_static/logo-300.png
+    :alt: PyScribus logo
+    :align: center
 
-A Python library to read, generate and update Scribus documents (SLA).
+A library aiming to read, generate and update Scribus documents (SLA).
 
-For Python versions newer than 3.7.9, see the main **pyscribus** package.
+----
 
-Prerequisites
-=============
+.. image:: https://nogithub.codeberg.page/badge.svg
+    :alt: Please don't upload to GitHub
+    :target: https://nogithub.codeberg.page
+.. image:: https://img.shields.io/pypi/v/pyscribus.svg?label=latest%20version
+    :alt: PyPi Latest Version
+    :target: https://pypi.python.org/pypi/pyscribus
 
-* `lxml <https://lxml.de/>`_
-* `svg.path <https://pypi.org/project/svg.path/>`_
+----
 
-Optional (for extra features)
------------------------------
+For Python versions newer than 3.8, see the main 
+`pyscribus <https://pypi.org/project/pyscribus>`_ package.
 
-* `Pillow <https://python-pillow.org/>`_ for ``extra.wireframe`` module
+- `Quickstart <https://etnadji.fr/pyscribus/guide/en/quickstart.html>`_
 
-Documentation
-=============
-
-`PyScribus <https://etnadji.fr/pyscribus>`_
```

### Comparing `pyscribus-backported-0.2.4/setup.py` & `pyscribus-backported-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:Utf-8 -*-
 
 import setuptools
 
 with open("../README.pypi.rst", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.2.4"
+VERSION = "0.3"
 DESCRIPTION = "Read, create and update Scribus .sla files. (Python < 3.8 version)"
 
 REQUIRED = ['lxml', 'svg.path']
 
 setuptools.setup(
     name="pyscribus-backported",
     version=VERSION,
@@ -27,15 +27,15 @@
         "Operating System :: OS Independent",
         "Topic :: Multimedia :: Graphics",
         "Topic :: Text Processing :: Markup :: XML",
         "Intended Audience :: Developers"
     ],
     project_urls={
         "Documentation": "https://etnadji.fr/pyscribus",
-        "Source Code": "https://framagit.org/etnadji/pyscribus/-/tree/backported",
+        "Source Code": "https://framagit.org/etnadji/pyscribus/-/tree/backported-model",
         "Issue tracker": "https://framagit.org/etnadji/pyscribus/-/issues",
     },
     python_requires='<=3.7.9',
     install_requires=REQUIRED,
     keywords=["scribus", "sla"],
 )
```

