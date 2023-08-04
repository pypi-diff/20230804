# Comparing `tmp/Jakit-0.2.tar.gz` & `tmp/Jakit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jakit-0.2.tar", last modified: Thu Aug  3 14:15:22 2023, max compression
+gzip compressed data, was "Jakit-0.3.tar", last modified: Thu Aug  3 14:29:07 2023, max compression
```

## Comparing `Jakit-0.2.tar` & `Jakit-0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.757667 Jakit-0.2/
-drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.737671 Jakit-0.2/Jakit/
--rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.2/Jakit/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-08-03 13:26:48.000000 Jakit-0.2/Jakit/jakit_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:15:22.750671 Jakit-0.2/Jakit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      752 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-03 14:15:22.000000 Jakit-0.2/Jakit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.2/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-03 14:15:22.752673 Jakit-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 14:15:22.760667 Jakit-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1951 2023-08-03 14:15:07.000000 Jakit-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.263231 Jakit-0.3/
+drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.220229 Jakit-0.3/Jakit/
+-rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.3/Jakit/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-08-03 13:26:48.000000 Jakit-0.3/Jakit/jakit_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:29:07.259230 Jakit-0.3/Jakit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-08-03 14:29:07.000000 Jakit-0.3/Jakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 14:29:06.000000 Jakit-0.3/Jakit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.3/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-03 14:29:07.262229 Jakit-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:29:07.263231 Jakit-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-08-03 14:28:59.000000 Jakit-0.3/setup.py
```

### Comparing `Jakit-0.2/Jakit/jakit_jobs.py` & `Jakit-0.3/Jakit/jakit_jobs.py`

 * *Files identical despite different names*

### Comparing `Jakit-0.2/Jakit.egg-info/PKG-INFO` & `Jakit-0.3/Jakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.2
+Version: 0.3
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.2/LICENSE` & `Jakit-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Jakit-0.2/PKG-INFO` & `Jakit-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.2
+Version: 0.3
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

