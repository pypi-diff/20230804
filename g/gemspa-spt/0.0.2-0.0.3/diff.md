# Comparing `tmp/gemspa-spt-0.0.2.tar.gz` & `tmp/gemspa-spt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemspa-spt-0.0.2.tar", last modified: Mon May 29 18:00:32 2023, max compression
+gzip compressed data, was "gemspa-spt-0.0.3.tar", last modified: Fri Aug  4 17:17:03 2023, max compression
```

## Comparing `gemspa-spt-0.0.2.tar` & `gemspa-spt-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 18:00:32.854575 gemspa-spt-0.0.2/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1511 2023-04-13 14:56:39.000000 gemspa-spt-0.0.2/LICENSE
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2630 2023-05-29 18:00:32.854416 gemspa-spt-0.0.2/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      329 2023-05-27 19:14:13.000000 gemspa-spt-0.0.2/README.md
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      735 2023-05-29 17:58:03.000000 gemspa-spt-0.0.2/pyproject.toml
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       38 2023-05-29 18:00:32.854621 gemspa-spt-0.0.2/setup.cfg
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 18:00:32.851144 gemspa-spt-0.0.2/src/
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 18:00:32.852181 gemspa-spt-0.0.2/src/gemspa_spt/
--rw-------   0 sarahkeegan   (501) staff       (20)      103 2023-04-13 15:17:17.000000 gemspa-spt-0.0.2/src/gemspa_spt/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    28402 2023-05-29 17:25:20.000000 gemspa-spt-0.0.2/src/gemspa_spt/particle_tracks.py
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 18:00:32.853504 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2630 2023-05-29 18:00:32.000000 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      326 2023-05-29 18:00:32.000000 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/SOURCES.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-05-29 18:00:32.000000 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/dependency_links.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       26 2023-05-29 18:00:32.000000 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/requires.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       11 2023-05-29 18:00:32.000000 gemspa-spt-0.0.2/src/gemspa_spt.egg-info/top_level.txt
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 18:00:32.854024 gemspa-spt-0.0.2/tests/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1516 2023-05-29 17:55:25.000000 gemspa-spt-0.0.2/tests/test_functions.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1938 2023-05-29 17:55:25.000000 gemspa-spt-0.0.2/tests/test_input.py
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:17:03.890541 gemspa-spt-0.0.3/
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1511 2023-04-18 13:13:22.000000 gemspa-spt-0.0.3/LICENSE
+-rw-r--r--   0 snk218   (1170528910) 1222563772     2630 2023-08-04 17:17:03.890282 gemspa-spt-0.0.3/PKG-INFO
+-rw-r--r--   0 snk218   (1170528910) 1222563772      329 2023-05-30 13:18:00.000000 gemspa-spt-0.0.3/README.md
+-rw-r--r--   0 snk218   (1170528910) 1222563772      728 2023-08-04 17:14:39.000000 gemspa-spt-0.0.3/pyproject.toml
+-rw-r--r--   0 snk218   (1170528910) 1222563772       38 2023-08-04 17:17:03.890626 gemspa-spt-0.0.3/setup.cfg
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:17:03.883232 gemspa-spt-0.0.3/src/
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:17:03.885851 gemspa-spt-0.0.3/src/gemspa_spt/
+-rw-r--r--   0 snk218   (1170528910) 1222563772      103 2023-04-18 13:13:22.000000 gemspa-spt-0.0.3/src/gemspa_spt/__init__.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772    28402 2023-05-30 13:18:00.000000 gemspa-spt-0.0.3/src/gemspa_spt/particle_tracks.py
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:17:03.888523 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/
+-rw-r--r--   0 snk218   (1170528910) 1222563772     2630 2023-08-04 17:17:03.000000 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/PKG-INFO
+-rw-r--r--   0 snk218   (1170528910) 1222563772      326 2023-08-04 17:17:03.000000 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/SOURCES.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772        1 2023-08-04 17:17:03.000000 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/dependency_links.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772       19 2023-08-04 17:17:03.000000 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/requires.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772       11 2023-08-04 17:17:03.000000 gemspa-spt-0.0.3/src/gemspa_spt.egg-info/top_level.txt
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:17:03.889632 gemspa-spt-0.0.3/tests/
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1516 2023-05-30 13:18:00.000000 gemspa-spt-0.0.3/tests/test_functions.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1938 2023-05-30 13:18:00.000000 gemspa-spt-0.0.3/tests/test_input.py
```

### Comparing `gemspa-spt-0.0.2/LICENSE` & `gemspa-spt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gemspa-spt-0.0.2/PKG-INFO` & `gemspa-spt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemspa-spt
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for analysis of single particle tracking experiments
 Author-email: Sarah Keegan <sarah.keegan@nyulangone.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sarah Keegan
         All rights reserved.
```

### Comparing `gemspa-spt-0.0.2/pyproject.toml` & `gemspa-spt-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemspa-spt"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sarah Keegan", email="sarah.keegan@nyulangone.org" },
 ]
 description = "A package for analysis of single particle tracking experiments"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
@@ -17,13 +17,13 @@
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "numpy",
     "pandas",
-    "scikit-image"
+    "scipy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/liamholtlab/gemspa-spt"
 "Bug Tracker" = "https://github.com/liamholtlab/gemspa-spt/issues"
```

### Comparing `gemspa-spt-0.0.2/src/gemspa_spt/particle_tracks.py` & `gemspa-spt-0.0.3/src/gemspa_spt/particle_tracks.py`

 * *Files identical despite different names*

### Comparing `gemspa-spt-0.0.2/src/gemspa_spt.egg-info/PKG-INFO` & `gemspa-spt-0.0.3/src/gemspa_spt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemspa-spt
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for analysis of single particle tracking experiments
 Author-email: Sarah Keegan <sarah.keegan@nyulangone.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Sarah Keegan
         All rights reserved.
```

### Comparing `gemspa-spt-0.0.2/tests/test_functions.py` & `gemspa-spt-0.0.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `gemspa-spt-0.0.2/tests/test_input.py` & `gemspa-spt-0.0.3/tests/test_input.py`

 * *Files identical despite different names*

