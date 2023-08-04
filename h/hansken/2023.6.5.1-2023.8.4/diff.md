# Comparing `tmp/hansken-2023.6.5.1.tar.gz` & `tmp/hansken-2023.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hansken-2023.6.5.1.tar", last modified: Mon Jun  5 15:00:46 2023, max compression
+gzip compressed data, was "hansken-2023.8.4.tar", last modified: Fri Aug  4 15:03:30 2023, max compression
```

## Comparing `hansken-2023.6.5.1.tar` & `hansken-2023.8.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1528 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.726849 hansken-2023.6.5.1/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       10 2023-06-05 15:00:43.000000 hansken-2023.6.5.1/hansken/VERSION
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2483 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/abstract_trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/admin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32028 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/auth.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/connect.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26374 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/query.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/hansken/recipes/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/export.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/hansken/recipes/report/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.726849 hansken-2023.6.5.1/hansken/recipes/report/templates/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/base.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/default.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/macros.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/print.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/table.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   134436 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/remote.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/hansken/tool/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/_webhdfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_backup.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_extract.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_grant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_mount.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11147 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_quickstart.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_shell.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_stats.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_tasks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_tools.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_upload.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/tool/command_versions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59342 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/hansken/util.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/hansken.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1528 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      299 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-06-05 15:00:46.000000 hansken-2023.6.5.1/hansken.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-05 15:00:46.730850 hansken-2023.6.5.1/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1876 2023-06-05 15:00:39.000000 hansken-2023.6.5.1/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-08-04 15:03:22.000000 hansken-2023.8.4/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-08-04 15:03:22.000000 hansken-2023.8.4/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-04 15:03:30.732478 hansken-2023.8.4/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-08-04 15:03:22.000000 hansken-2023.8.4/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.728478 hansken-2023.8.4/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-04 15:03:27.000000 hansken-2023.8.4/hansken/VERSION
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2483 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/abstract_trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/admin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32028 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/auth.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/connect.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26248 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/query.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/export.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/report/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.728478 hansken-2023.8.4/hansken/recipes/report/templates/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/report/templates/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/base.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/default.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/macros.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/print.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/table.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   135700 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/remote.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/tool/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/_webhdfs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_backup.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_extract.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_grant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_mount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11147 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_quickstart.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_shell.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_stats.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_tasks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_tools.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_upload.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_versions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59819 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/util.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      299 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-08-04 15:03:30.732478 hansken-2023.8.4/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1827 2023-08-04 15:03:22.000000 hansken-2023.8.4/setup.py
```

### Comparing `hansken-2023.6.5.1/LICENSE` & `hansken-2023.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/PKG-INFO` & `hansken-2023.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.6.5.1
+Version: 2023.8.4
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: mount
 Provides-Extra: kerberos
```

### Comparing `hansken-2023.6.5.1/README.md` & `hansken-2023.8.4/README.md`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/__init__.py` & `hansken-2023.8.4/hansken/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/abstract_trace.py` & `hansken-2023.8.4/hansken/abstract_trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/admin.py` & `hansken-2023.8.4/hansken/admin.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/auth.py` & `hansken-2023.8.4/hansken/auth.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/connect.py` & `hansken-2023.8.4/hansken/connect.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/query.py` & `hansken-2023.8.4/hansken/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 log = Logger(__name__)
 
 
 # 'known' default maximum number of clauses in a (boolean) query
 DEFAULT_MAX_CLAUSE_COUNT = 1024
 
 
-# collect the type of a compiled pattern (re.Pattern in 3.7+, a runtime type in Python 3.6)
-_Pattern = type(re.compile('.*'))
-
-
 def _format_value(value):
     """
     Formats a value suitable for Hansken Query Language:
 
     - date, datetime: ISO 8601
     - GeographicLocation: ISO 6709 string
     - tuple of numbers, length 2: assumed to be latlong, formatted as an
@@ -355,15 +351,15 @@
         if pattern is None:
             pattern = field_or_pattern
             # full matches won't work on text (which expands to both meta and data)
             field = 'meta' if full else 'text'
         else:
             field = field_or_pattern
 
-        if isinstance(pattern, _Pattern):
+        if isinstance(pattern, re.Pattern):
             if pattern.flags & ~re.UNICODE:
                 log.warn('regular expression flags in Query objects are ignored ({} used by pattern)',
                          str(re.RegexFlag(pattern.flags)))
             # remote has no use for a Pattern object, use value's original pattern string
             pattern = pattern.pattern
 
         if not isinstance(pattern, str):
```

### Comparing `hansken-2023.6.5.1/hansken/recipes/export.py` & `hansken-2023.8.4/hansken/recipes/export.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/recipes/report/__init__.py` & `hansken-2023.8.4/hansken/recipes/report/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/base.html` & `hansken-2023.8.4/hansken/recipes/report/templates/hansken/base.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/recipes/report/templates/hansken/macros.html` & `hansken-2023.8.4/hansken/recipes/report/templates/hansken/macros.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/remote.py` & `hansken-2023.8.4/hansken/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -874,14 +874,23 @@
         response = self._session.get(self.url(*path))
         return _expect_ok(response).json()
 
     def trace(self, project_id, trace_uid):
         response = self._session.get(self.url(self.path.projects, project_id, '/traces', trace_uid))
         return _expect_ok(response).json()
 
+    def descriptor(self, project_id, trace_uid, stream='raw', key=fetch):
+        key = self._maybe_fetch_key(image_id=image_from_uid(trace_uid), key=key)
+        response = self._session.get(
+            self.url(self.path.projects, project_id, '/traces', trace_uid, '/data', '/descriptor'),
+            params=omit_empty({'dataType': stream}),
+            headers=omit_empty({'Hansken-Image-Key': b64encode(key) if key else None})
+        )
+        return _expect_ok(response, codes.ok).json()
+
     def data(self, project_id, trace_uid, stream='raw', offset=0, size=None, key=fetch, bufsize=8 << 10):
         """
         Opens a streaming read request that provides the requested data stream
         of a particular trace. Note that this provides a stream that should be
         closed by the user after use.
 
         :param project_id: the project to associate the request with
@@ -2423,14 +2432,28 @@
 
     @_auto_open
     def trace(self, trace_uid):
         source = self.connection.trace(self.project_id, trace_uid)
         return self.trace_class(source)
 
     @_auto_open
+    def descriptor(self, trace_uid, stream='raw', key=fetch):
+        """
+        Retrieve the data descriptor for a named stream (default ``raw``) for a
+        particular trace.
+
+        :param trace_uid: the trace to retrieve the data descriptor for
+        :param stream: stream to get the descriptor for
+        :param key: key for the image of this trace (default is to fetch the
+            key automatically, if it's available)
+        :return: the stream's data descriptor (as-is)
+        """
+        return self.connection.descriptor(self.project_id, trace_uid, stream, key)
+
+    @_auto_open
     def data(self, trace_uid, stream='raw', offset=0, size=None, key=fetch):
         if key is fetch:
             # ProjectContext caches keys, prefer cached over fetched from remote
             key = self.key(image_from_uid(trace_uid))
 
         return self.connection.data(self.project_id, trace_uid, stream, offset, size, key)
 
@@ -2914,14 +2937,17 @@
 
     def roots(self):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
     def trace(self, trace_uid):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
+    def descriptor(self, trace_uid, stream='raw', key=fetch):
+        raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
+
     def data(self, trace_uid, stream='raw', offset=0, size=None, key=fetch):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
     def children(self, trace_uid, query=None, start=0, count=None, sort=None, facets=None, snippets=None, timeout=None):
         raise TypeError('method not supported in multi-project search, use a regular ProjectContext')
 
     def note(self, trace_uid, note, refresh=None):
```

### Comparing `hansken-2023.6.5.1/hansken/tool/__init__.py` & `hansken-2023.8.4/hansken/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/_webhdfs.py` & `hansken-2023.8.4/hansken/tool/_webhdfs.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_backup.py` & `hansken-2023.8.4/hansken/tool/command_backup.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_extract.py` & `hansken-2023.8.4/hansken/tool/command_extract.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_grant.py` & `hansken-2023.8.4/hansken/tool/command_grant.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_mount.py` & `hansken-2023.8.4/hansken/tool/command_mount.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_quickstart.py` & `hansken-2023.8.4/hansken/tool/command_quickstart.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_shell.py` & `hansken-2023.8.4/hansken/tool/command_shell.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_stats.py` & `hansken-2023.8.4/hansken/tool/command_stats.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_tasks.py` & `hansken-2023.8.4/hansken/tool/command_tasks.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_tools.py` & `hansken-2023.8.4/hansken/tool/command_tools.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_upload.py` & `hansken-2023.8.4/hansken/tool/command_upload.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/tool/command_versions.py` & `hansken-2023.8.4/hansken/tool/command_versions.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken/trace.py` & `hansken-2023.8.4/hansken/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,14 +431,26 @@
         :param key: key for the image of this trace (default is to fetch the
             key automatically, if it's available)
         :return: a file-like object to read bytes from the named stream
         :rtype: `io.BufferedReader`
         """
         return self.context.data(self.uid, stream, offset, size, key)
 
+    def descriptor(self, stream='raw', key=fetch):
+        """
+        Retrieve the data descriptor for a named stream (default ``raw``) for
+        this `.Trace`.
+
+        :param stream: stream to get the descriptor for
+        :param key: key for the image of this trace (default is to fetch the
+            key automatically, if it's available)
+        :return: the stream's data descriptor (as-is)
+        """
+        return self.context.descriptor(self.uid, stream, key)
+
     @property
     def preview_types(self):
         """
         A set of preview type names (mime types) available for this `.Trace`.
         These names can be used with calls to `preview <.Trace.preview>`.
 
         :return: preview type names available for this `.Trace` (possibly
```

### Comparing `hansken-2023.6.5.1/hansken/util.py` & `hansken-2023.8.4/hansken/util.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/hansken.egg-info/PKG-INFO` & `hansken-2023.8.4/hansken.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.6.5.1
+Version: 2023.8.4
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: mount
 Provides-Extra: kerberos
```

### Comparing `hansken-2023.6.5.1/hansken.egg-info/SOURCES.txt` & `hansken-2023.8.4/hansken.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hansken-2023.6.5.1/setup.py` & `hansken-2023.8.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     url='https://hansken.org/',
     description='Python API to the Hansken REST endpoint',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 
     packages=find_packages(),
```

