# Comparing `tmp/artistlib-0.0.4.tar.gz` & `tmp/artistlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistlib-0.0.4.tar", last modified: Fri Feb  3 13:24:05 2023, max compression
+gzip compressed data, was "artistlib-0.0.5.tar", last modified: Fri Aug  4 11:02:13 2023, max compression
```

## Comparing `artistlib-0.0.4.tar` & `artistlib-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 13:24:05.919372 artistlib-0.0.4/
--rw-rw-rw-   0        0        0     1128 2022-07-27 10:54:06.000000 artistlib-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0      964 2023-02-03 13:24:05.919372 artistlib-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-02-02 18:40:46.000000 artistlib-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 13:24:05.935376 artistlib-0.0.4/artistlib/
--rw-rw-rw-   0        0        0     3261 2023-02-02 17:44:52.000000 artistlib-0.0.4/artistlib/__init__.py
--rw-rw-rw-   0        0        0      518 2023-02-03 13:24:05.935376 artistlib-0.0.4/artistlib/_version.py
-drwxrwxrwx   0        0        0        0 2023-02-03 13:24:05.912372 artistlib-0.0.4/artistlib.egg-info/
--rw-rw-rw-   0        0        0      964 2023-02-03 13:24:05.000000 artistlib-0.0.4/artistlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-02-03 13:24:05.000000 artistlib-0.0.4/artistlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 13:24:05.000000 artistlib-0.0.4/artistlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-03 13:24:03.000000 artistlib-0.0.4/artistlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-02-03 13:24:05.000000 artistlib-0.0.4/artistlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      209 2023-02-03 13:24:05.927374 artistlib-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      933 2022-09-28 11:15:37.000000 artistlib-0.0.4/setup.py
--rw-rw-rw-   0        0        0    83021 2022-09-28 12:26:33.000000 artistlib-0.0.4/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:02:13.421900 artistlib-0.0.5/
+-rw-rw-rw-   0        0        0     1128 2022-07-27 10:54:06.000000 artistlib-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0      964 2023-08-04 11:02:13.421900 artistlib-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-02-02 18:40:46.000000 artistlib-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:02:13.438902 artistlib-0.0.5/artistlib/
+-rw-rw-rw-   0        0        0     4701 2023-08-04 09:52:37.000000 artistlib-0.0.5/artistlib/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-08-04 11:02:13.439900 artistlib-0.0.5/artistlib/_version.py
+-rw-rw-rw-   0        0        0      195 2023-08-04 09:52:37.000000 artistlib-0.0.5/artistlib/console.py
+-rw-rw-rw-   0        0        0     1528 2023-08-04 09:52:37.000000 artistlib-0.0.5/artistlib/remote_access.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:02:13.413899 artistlib-0.0.5/artistlib.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-08-04 11:02:13.000000 artistlib-0.0.5/artistlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-08-04 11:02:13.000000 artistlib-0.0.5/artistlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:02:13.000000 artistlib-0.0.5/artistlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 11:02:10.000000 artistlib-0.0.5/artistlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-04 11:02:13.000000 artistlib-0.0.5/artistlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      209 2023-08-04 11:02:13.431902 artistlib-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      933 2022-09-28 11:15:37.000000 artistlib-0.0.5/setup.py
+-rw-rw-rw-   0        0        0    83021 2022-09-28 12:26:33.000000 artistlib-0.0.5/versioneer.py
```

### Comparing `artistlib-0.0.4/LICENSE.md` & `artistlib-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `artistlib-0.0.4/PKG-INFO` & `artistlib-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistlib
-Version: 0.0.4
+Version: 0.0.5
 Summary: aRTist Python library
 Home-page: https://github.com/BAMresearch/aRTist-PythonLib
 Author: Carsten Bellon
 Author-email: Carsten.Bellon@bam.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `artistlib-0.0.4/artistlib.egg-info/PKG-INFO` & `artistlib-0.0.5/artistlib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistlib
-Version: 0.0.4
+Version: 0.0.5
 Summary: aRTist Python library
 Home-page: https://github.com/BAMresearch/aRTist-PythonLib
 Author: Carsten Bellon
 Author-email: Carsten.Bellon@bam.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `artistlib-0.0.4/setup.py` & `artistlib-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `artistlib-0.0.4/versioneer.py` & `artistlib-0.0.5/versioneer.py`

 * *Files identical despite different names*

