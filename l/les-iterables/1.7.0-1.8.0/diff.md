# Comparing `tmp/les_iterables-1.7.0.tar.gz` & `tmp/les_iterables-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "les_iterables-1.7.0.tar", last modified: Tue Feb 28 14:09:57 2023, max compression
+gzip compressed data, was "les_iterables-1.8.0.tar", last modified: Fri Aug  4 09:40:24 2023, max compression
```

## Comparing `les_iterables-1.7.0.tar` & `les_iterables-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:09:57.375584 les_iterables-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-28 14:09:44.000000 les_iterables-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-28 14:09:57.375584 les_iterables-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-28 14:09:44.000000 les_iterables-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-28 14:09:44.000000 les_iterables-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-28 14:09:57.375584 les_iterables-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:09:57.371583 les_iterables-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:09:57.375584 les_iterables-1.7.0/src/les_iterables/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/augmenting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/combining.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/searching.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/selecting.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-28 14:09:44.000000 les_iterables-1.7.0/src/les_iterables/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:09:57.375584 les_iterables-1.7.0/src/les_iterables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:09:57.000000 les_iterables-1.7.0/src/les_iterables.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:40:24.287663 les_iterables-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 09:40:09.000000 les_iterables-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-04 09:40:24.287663 les_iterables-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-04 09:40:09.000000 les_iterables-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 09:40:09.000000 les_iterables-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 09:40:24.287663 les_iterables-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:40:24.283663 les_iterables-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:40:24.287663 les_iterables-1.8.0/src/les_iterables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/augmenting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/combining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/searching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/selecting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 09:40:09.000000 les_iterables-1.8.0/src/les_iterables/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:40:24.287663 les_iterables-1.8.0/src/les_iterables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:40:24.000000 les_iterables-1.8.0/src/les_iterables.egg-info/zip-safe
```

### Comparing `les_iterables-1.7.0/LICENSE.txt` & `les_iterables-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/PKG-INFO` & `les_iterables-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: les_iterables
-Version: 1.7.0
+Version: 1.8.0
 Summary: Iterable processing functions
 Home-page: https://github.com/sixty-north/les_iterables
 Author: Sixty North AS
 Author-email: systems+les_iterables@sixty-north.com
 License: MIT License
 Keywords: iterators iterables
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `les_iterables-1.7.0/README.md` & `les_iterables-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/setup.cfg` & `les_iterables-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/__init__.py` & `les_iterables-1.8.0/src/les_iterables/__init__.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/augmenting.py` & `les_iterables-1.8.0/src/les_iterables/augmenting.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/combining.py` & `les_iterables-1.8.0/src/les_iterables/combining.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/functions.py` & `les_iterables-1.8.0/src/les_iterables/functions.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/generating.py` & `les_iterables-1.8.0/src/les_iterables/generating.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/grouping.py` & `les_iterables-1.8.0/src/les_iterables/grouping.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/parsing.py` & `les_iterables-1.8.0/src/les_iterables/parsing.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables/selecting.py` & `les_iterables-1.8.0/src/les_iterables/selecting.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
         if not predicate(item):
             yield item
             break
     yield from iterator
 
 
 def transform_if(iterable, predicate, transform):
-    """Apply a transformation to items which match a preducate.
+    """Apply a transformation to items which match a predicate.
 
     Non-matching items will not be transformed.
 
     Args:
         iterable: An iterable of items.
         predicate: predicate: A predicate function with which to select items to be transformed.
         transform: A unary function which accepts an item to be transformed and returns the
```

### Comparing `les_iterables-1.7.0/src/les_iterables/sequences.py` & `les_iterables-1.8.0/src/les_iterables/sequences.py`

 * *Files identical despite different names*

### Comparing `les_iterables-1.7.0/src/les_iterables.egg-info/PKG-INFO` & `les_iterables-1.8.0/src/les_iterables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: les-iterables
-Version: 1.7.0
+Version: 1.8.0
 Summary: Iterable processing functions
 Home-page: https://github.com/sixty-north/les_iterables
 Author: Sixty North AS
 Author-email: systems+les_iterables@sixty-north.com
 License: MIT License
 Keywords: iterators iterables
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `les_iterables-1.7.0/src/les_iterables.egg-info/SOURCES.txt` & `les_iterables-1.8.0/src/les_iterables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

