# Comparing `tmp/astro-tiptop-1.1.tar.gz` & `tmp/astro-tiptop-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-tiptop-1.1.tar", last modified: Fri Jul  7 09:12:17 2023, max compression
+gzip compressed data, was "astro-tiptop-1.2.tar", last modified: Fri Aug  4 10:14:26 2023, max compression
```

## Comparing `astro-tiptop-1.1.tar` & `astro-tiptop-1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.147058 astro-tiptop-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 09:11:59.000000 astro-tiptop-1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 09:11:59.000000 astro-tiptop-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 09:11:59.000000 astro-tiptop-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 09:12:17.155058 astro-tiptop-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 09:11:59.000000 astro-tiptop-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-EXAMPLE.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-EXAMPLE.py
--rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-07 09:11:59.000000 astro-tiptop-1.1/TIPTOP-GUI.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/astro_tiptop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 09:12:17.000000 astro-tiptop-1.1/astro_tiptop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.151058 astro-tiptop-1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/parameterFile.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-07 09:11:59.000000 astro-tiptop-1.1/docs/source/wishList.rst
--rw-r--r--   0 runner    (1001) docker     (123)   165545 2023-07-07 09:11:59.000000 astro-tiptop-1.1/main_sphere_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/perfTest/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/ERIS.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/ERIS_LGS.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     7610 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     7496 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniLTAO_3.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     5789 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_1.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_2.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/HarmoniSCAO_3.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/MAVIS.ini
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/SOUL.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest/SPHERE.ini
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 09:11:59.000000 astro-tiptop-1.1/perfTest.sh
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 09:11:59.000000 astro-tiptop-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:12:17.155058 astro-tiptop-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:17.155058 astro-tiptop-1.1/tiptop/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 09:12:16.000000 astro-tiptop-1.1/tiptop/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptopCLT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-07 09:11:59.000000 astro-tiptop-1.1/tiptop/tiptopGUI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.068371 astro-tiptop-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.036371 astro-tiptop-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.044371 astro-tiptop-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 10:14:07.000000 astro-tiptop-1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-04 10:14:07.000000 astro-tiptop-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-04 10:14:07.000000 astro-tiptop-1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 10:14:07.000000 astro-tiptop-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 10:14:07.000000 astro-tiptop-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-04 10:14:26.064371 astro-tiptop-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-04 10:14:07.000000 astro-tiptop-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-04 10:14:07.000000 astro-tiptop-1.2/TIPTOP-EXAMPLE.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-04 10:14:07.000000 astro-tiptop-1.2/TIPTOP-EXAMPLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-08-04 10:14:07.000000 astro-tiptop-1.2/TIPTOP-GUI.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.044371 astro-tiptop-1.2/astro_tiptop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-04 10:14:25.000000 astro-tiptop-1.2/astro_tiptop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-04 10:14:26.000000 astro-tiptop-1.2/astro_tiptop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:14:25.000000 astro-tiptop-1.2/astro_tiptop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 10:14:25.000000 astro-tiptop-1.2/astro_tiptop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 10:14:25.000000 astro-tiptop-1.2/astro_tiptop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.044371 astro-tiptop-1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.048371 astro-tiptop-1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/parameterFile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-08-04 10:14:07.000000 astro-tiptop-1.2/docs/source/wishList.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   165545 2023-08-04 10:14:07.000000 astro-tiptop-1.2/main_sphere_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.056371 astro-tiptop-1.2/perfTest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/ERIS.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/ERIS_LGS.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7610 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniLTAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7496 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniLTAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7520 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniLTAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniSCAO_1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniSCAO_2.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5777 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/HarmoniSCAO_3.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/MAVIS.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/SOUL.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest/SPHERE.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-04 10:14:07.000000 astro-tiptop-1.2/perfTest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-04 10:14:07.000000 astro-tiptop-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:14:26.068371 astro-tiptop-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:14:26.064371 astro-tiptop-1.2/tiptop/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 10:14:07.000000 astro-tiptop-1.2/tiptop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 10:14:25.000000 astro-tiptop-1.2/tiptop/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-08-04 10:14:07.000000 astro-tiptop-1.2/tiptop/tiptop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-08-04 10:14:07.000000 astro-tiptop-1.2/tiptop/tiptopCLT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-04 10:14:07.000000 astro-tiptop-1.2/tiptop/tiptopGUI.py
```

### Comparing `astro-tiptop-1.1/.github/workflows/publish.yml` & `astro-tiptop-1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/.gitignore` & `astro-tiptop-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/LICENSE` & `astro-tiptop-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/PKG-INFO` & `astro-tiptop-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.1
+Version: 1.2
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: gui
 License-File: LICENSE
 
 # TIPTOP
```

### Comparing `astro-tiptop-1.1/README.md` & `astro-tiptop-1.2/README.md`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/TIPTOP-EXAMPLE.ipynb` & `astro-tiptop-1.2/TIPTOP-EXAMPLE.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/TIPTOP-GUI.ipynb` & `astro-tiptop-1.2/TIPTOP-GUI.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/astro_tiptop.egg-info/PKG-INFO` & `astro-tiptop-1.2/astro_tiptop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: astro-tiptop
-Version: 1.1
+Version: 1.2
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/TIPTOP
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: gui
 License-File: LICENSE
 
 # TIPTOP
```

### Comparing `astro-tiptop-1.1/astro_tiptop.egg-info/SOURCES.txt` & `astro-tiptop-1.2/astro_tiptop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/Makefile` & `astro-tiptop-1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/make.bat` & `astro-tiptop-1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/source/conf.py` & `astro-tiptop-1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/source/howto.rst` & `astro-tiptop-1.2/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/source/index.rst` & `astro-tiptop-1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/source/parameterFile.rst` & `astro-tiptop-1.2/docs/source/parameterFile.rst`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
    High Order WFS pixel scale in [mas], unclear what are the units if we chose a pyramid wavefront sensor
    Warning: gives a confusing error message if missing 
 
 .. option:: FieldOfView
 
    **Required**, 
    *type: int*, 
-   Number of pixels on the detector. 
+   Number of pixels per subaperture. 
    TODOI : change this behaviour as it makes no sense. Guido found that this is divided by `NumberLenslet`. Used for the noise. 
    Warning: gives a confusing error message if missing 
 
 .. option:: Binning
    
    **Optional**, 
    *type: int*,
```

### Comparing `astro-tiptop-1.1/docs/source/usage.rst` & `astro-tiptop-1.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/docs/source/wishList.rst` & `astro-tiptop-1.2/docs/source/wishList.rst`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/main_sphere_test.ipynb` & `astro-tiptop-1.2/main_sphere_test.ipynb`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/ERIS.ini` & `astro-tiptop-1.2/perfTest/ERIS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/ERIS_LGS.ini` & `astro-tiptop-1.2/perfTest/ERIS_LGS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/HarmoniLTAO_1.ini` & `astro-tiptop-1.2/perfTest/HarmoniLTAO_1.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/HarmoniLTAO_2.ini` & `astro-tiptop-1.2/perfTest/HarmoniLTAO_2.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/HarmoniLTAO_3.ini` & `astro-tiptop-1.2/perfTest/HarmoniLTAO_3.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/HarmoniSCAO_1.ini` & `astro-tiptop-1.2/perfTest/HarmoniSCAO_2.ini`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 ; wavelength of definition of atmosphere statistics  -  optional - default 500e-9
 Wavelength = 500e-9
 ; seeing at zenith in arcsec- required
 Seeing = 0.65
 ; Outer scale in meter - optional - default: 25.0
 L0 = 25.0
 ; Relative contribution of each layer (sum=1) - optional -  default: [1.0]
-;JQ110Layers
 Cn2Weights = [0.43900001, 0.14700001, 0.1142    , 0.056     , 0.03683   ,   0.0442    , 0.0527    , 0.0794    , 0.01829   , 0.012939  ]
 ; altitude of layers in meters - optional -  default [0.0]
 ;Cn2Heights = [30, 140, 281, 562, 1125, 2250, 4500, 7750, 11000, 14000]
 Cn2Heights = [   83.16413254,   243.29187551,   710.47154255,  2735.63637091,  5583.67373605,  8599.18858474, 11598.92106005, 14221.06437269, 17219.02406272, 21912.89106645]
 ; wind speed values for each layer in m/s - optional -  default [10.0]
 WindSpeed = [6.6, 5.9, 5.1, 4.5, 5.1, 8.3, 16.3, 10.2, 14.3, 17.5]
 ; wind direction for each layer in degrees - optional -  default [0.0]
@@ -41,15 +40,15 @@
 Zenith = [0.0]
 Azimuth = [0.0]
 
 [sources_HO]
 ;Sensing wavelength for HO modes in meters - required
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [0.0]
+Zenith = [15.]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
@@ -64,15 +63,15 @@
 ;HO WFS pixel scale in [mas] - required
 PixelScale = 220      
 ;Number of pixels per subaperture - required
 FieldOfView = 600         
 ;binning factor - optional - default: 1
 Binning = 1
 ;Flux return in [nph/frame/subaperture] - required
-NumberPhotons = [500]    
+NumberPhotons = [150]    
 ;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
 SpotFWHM = [[0.0,0.0,0.0]]      
 ;Spectral bandwidth of the filter (imaging mode) - optional - default: 0.0
 SpectralBandwidth = 0.0
 ;Transmittance at the considered wavelengths for polychromatic mode - optional - default: [1.0]
 Transmittance = [1.0]
 ;Dispersion x/y at the considered wavelength in pixel. Must be the same size than Transmittance - optional - default: [[0.0,0.0]]
@@ -82,15 +81,15 @@
 ; dark current[e-/s/pix] - optional - default: 0.0
 Dark = 0.0
 ;Sky background [e-/s/pix] - optional - default: 0.0           
 SkyBackground = 0.0
 ;Pixel gain - optional - default:1.0
 Gain = 1.0  
 ;excess noise factor - optional - default: 2.0                     
-ExcessNoiseFactor = 1.0
+ExcessNoiseFactor = 1.0 
 ;Number of WFS lenslets - required
 NumberLenslets = [100]    
 ;Size of WFS lenslets in meters- optional
 SizeLenslets = [0.4]                                                     
 ;Noise Variance in rd^2. If not empty, this value overwrites the analytical noise variance calculation - optional
 NoiseVariance = [None]
 ;CoG computation algorithm - optional  -defaut:'wcog'
```

### Comparing `astro-tiptop-1.1/perfTest/HarmoniSCAO_2.ini` & `astro-tiptop-1.2/perfTest/HarmoniSCAO_3.ini`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 [atmosphere]
 r0_Value = 0
 testWindspeed = 0
 ; wavelength of definition of atmosphere statistics  -  optional - default 500e-9
 Wavelength = 500e-9
 ; seeing at zenith in arcsec- required
-Seeing = 0.65
+Seeing = 0.95
 ; Outer scale in meter - optional - default: 25.0
 L0 = 25.0
 ; Relative contribution of each layer (sum=1) - optional -  default: [1.0]
-Cn2Weights = [0.43900001, 0.14700001, 0.1142    , 0.056     , 0.03683   ,   0.0442    , 0.0527    , 0.0794    , 0.01829   , 0.012939  ]
+Cn2Weights =  [0.46510001, 0.18929999, 0.18569999, 0.0698    , 0.02554   , 0.01123   , 0.01545   , 0.02729   , 0.00627   , 0.004438  ]
 ; altitude of layers in meters - optional -  default [0.0]
 ;Cn2Heights = [30, 140, 281, 562, 1125, 2250, 4500, 7750, 11000, 14000]
-Cn2Heights = [   83.16413254,   243.29187551,   710.47154255,  2735.63637091,  5583.67373605,  8599.18858474, 11598.92106005, 14221.06437269, 17219.02406272, 21912.89106645]
+Cn2Heights = [     82.04886699,   252.57894569,   722.807951  ,  2620.66789668, 5167.21882457,  8600.34998944, 11722.58516535, 14220.09282085, 17218.05749335, 21912.70746385]
 ; wind speed values for each layer in m/s - optional -  default [10.0]
 WindSpeed = [6.6, 5.9, 5.1, 4.5, 5.1, 8.3, 16.3, 10.2, 14.3, 17.5]
 ; wind direction for each layer in degrees - optional -  default [0.0]
 WindDirection = [0., 0., 0., 0., 90., -90., -90., 90., 0., 0.]
 
 [sources_science]
 ;list of central wavelengths for each frame - required
@@ -40,15 +40,15 @@
 Zenith = [0.0]
 Azimuth = [0.0]
 
 [sources_HO]
 ;Sensing wavelength for HO modes in meters - required
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
-Zenith = [15.]
+Zenith = [0.0]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
```

### Comparing `astro-tiptop-1.1/perfTest/HarmoniSCAO_3.ini` & `astro-tiptop-1.2/perfTest/HarmoniSCAO_1.ini`

 * *Files 22% similar despite different names*

```diff
@@ -4,38 +4,49 @@
 ; telescope zenith angle in degrees - optional - default: 0.0
 ZenithAngle = 30.0
 ; pupil obstruction ratio due to the secondary in relative unites to the telescope diameter - optional - default: 0.0
 ObscurationRatio = 0.28
 ; pupil resolution in pixels - required
 Resolution = 400
 ; path to the pupil model in .fits file - optional (if provided, the pupil model is interpolated) - default: ''
-PathPupil = '/home/frossi/dev/TIPTOP/P3/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits'
+PathPupil = '/aoSystem/data/ELT_CALIBRATION/EELT480pp0.0813spider.fits'
 ; path to a map of static aberrations (nm) in .fits file - optional - default: ''
-PathStaticOn = '/home/frossi/dev/TIPTOP/P3/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits'
+PathStaticOn = '/aoSystem/data/ELT_CALIBRATION/CombinedError_Wavefront_nm.fits'
 ; path to a model of amplitude apodizaton of the electric field in the pupil in .fits file - optional - default: ''
-TechnicalFoV       = 120                                     
+PathApodizer = ''
+; path to a model of a basis of modes to describe addtionnal static aberrations - optional - default: ''
+PathStatModes = '' 
+; pupil angle in degrees - optional - default: 0.0
+PupilAngle = 0.0
+TechnicalFoV = 120
 
 [atmosphere]
-r0_Value = 0
-testWindspeed = 0
 ; wavelength of definition of atmosphere statistics  -  optional - default 500e-9
 Wavelength = 500e-9
 ; seeing at zenith in arcsec- required
-Seeing = 0.95
+Seeing = 0.65
 ; Outer scale in meter - optional - default: 25.0
 L0 = 25.0
 ; Relative contribution of each layer (sum=1) - optional -  default: [1.0]
-Cn2Weights =  [0.46510001, 0.18929999, 0.18569999, 0.0698    , 0.02554   , 0.01123   , 0.01545   , 0.02729   , 0.00627   , 0.004438  ]
+; JQ110Layers
+Cn2Weights = [0.43840001, 0.14700001, 0.1142, 0.056, 0.03683, 0.0442, 0.0527, 0.0794, 0.01829, 0.012939]
+; Cn2Weights = [1.0]
+ 
 ; altitude of layers in meters - optional -  default [0.0]
 ;Cn2Heights = [30, 140, 281, 562, 1125, 2250, 4500, 7750, 11000, 14000]
-Cn2Heights = [     82.04886699,   252.57894569,   722.807951  ,  2620.66789668, 5167.21882457,  8600.34998944, 11722.58516535, 14220.09282085, 17218.05749335, 21912.70746385]
+Cn2Heights = [   83.16413254,   243.29187551,   710.47154255,  2735.63637091,  5583.67373605,  8599.18858474, 11598.92106005, 14221.06437269, 17219.02406272, 21912.89106645]
+; Cn2Heights = [0.0]
+
 ; wind speed values for each layer in m/s - optional -  default [10.0]
 WindSpeed = [6.6, 5.9, 5.1, 4.5, 5.1, 8.3, 16.3, 10.2, 14.3, 17.5]
+; WindSpeed = [8.0]
+
 ; wind direction for each layer in degrees - optional -  default [0.0]
 WindDirection = [0., 0., 0., 0., 90., -90., -90., 90., 0., 0.]
+; WindDirection = [0.]
 
 [sources_science]
 ;list of central wavelengths for each frame - required
 Wavelength = [2200e-9]
 ;list of polar coordinates of the sciences sources; zenith in arcsec and azimuth in degrees - optional -  default: [0.0]
 Zenith = [0.0]
 Azimuth = [0.0]
@@ -45,33 +56,63 @@
 Wavelength = 950e-9
 ;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
 Zenith = [0.0]
 Azimuth = [0.0]
 ;altitude of the guide stars (0 if infinite) - optional - default: 0.0
 Height = 0.0
 
+;[sources_LO]
+;Sensing wavelength for HO modes in meters - required
+;Wavelength = 1650e-9
+;;list of polar coordinates of the guide stars sources; zenith in arcsec and azimuth in degrees - optional - default [0.0]
+;Zenith = [0.0]
+;Azimuth = [0.0]
+
 [sensor_science]
 ;pixel/spaxel scale in mas - required
 PixelScale = 4.0
 ;Field of view in pixel - optional - default: 150
 FieldOfView = 640
+;binning factor - optional - default: 1
+Binning = 1
+;Detected flux in [nph/frame/subaperture] - optional - default: 1500        
+NumberPhotons = [1500]
+;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
+SpotFWHM = [[1.0, 1.0, 0.0]]   
+;Spectral bandwidth of the filter (imaging mode) - optional - default: 0.0
+; wavelength are setup as a linear grid from ScienceWavelength - SpectralBandwidth to ScienceWavelength + SpectralBandwidth with a number of bins defined from the length of the Transmittance field
+SpectralBandwidth = 0.0
+;Transmittance at the considered wavelengths for polychromatic mode - optional - default: [1.0]
+Transmittance = [1.0]
+;Dispersion x/y at the considered wavelength in pixel. Must be the same size than Transmittance - optional - default: [[0.0],[0.0]]
+Dispersion = [[0.0],[0.0]]
+;ron in [e-] - optionnal - default: 0.0
+SigmaRON = [0.0]
+; dark current[e-/s/pix] - optional - default: 0.0
+Dark = 0.0
+;Sky background [e-/s/pix] - optional - default: 0.0           
+SkyBackground = 0.0
+;Pixel gain - optional - default:1.0
+Gain = 1.0
+;excess noise factor - optional - default: 1.0                     
+ExcessNoiseFactor = 1.0 
 
 [sensor_HO]
 ;WFS type - optional - default : Shack-Hartmann
 WfsType = 'Pyramid'
 ;Spot modulation radius in lambda/D units for pyramid WFS - optional - default : None
 Modulation = 3
 ;HO WFS pixel scale in [mas] - required
 PixelScale = 220      
 ;Number of pixels per subaperture - required
 FieldOfView = 600         
 ;binning factor - optional - default: 1
 Binning = 1
 ;Flux return in [nph/frame/subaperture] - required
-NumberPhotons = [150]    
+NumberPhotons = [500]    
 ;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
 SpotFWHM = [[0.0,0.0,0.0]]      
 ;Spectral bandwidth of the filter (imaging mode) - optional - default: 0.0
 SpectralBandwidth = 0.0
 ;Transmittance at the considered wavelengths for polychromatic mode - optional - default: [1.0]
 Transmittance = [1.0]
 ;Dispersion x/y at the considered wavelength in pixel. Must be the same size than Transmittance - optional - default: [[0.0,0.0]]
@@ -96,14 +137,46 @@
 Algorithm = 'wcog' 
 ;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
 WindowRadiusWCoG = 6
 ;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
 ThresholdWCoG = 0.0
 ;New value for pixels lower than threshold - optional - default: 0.0        
 NewValueThrPix = 0.0
+ 
+;[sensor_LO]
+;;LO WFS pixel scale in [mas] - required
+;PixelScale = 40.0
+;;Number of pixels per subaperture - required 
+;FieldOfView = 200 
+;;binning factor - optional - default: 1
+;Binning = 1   
+;;detected flux in [nph/frame/subaperture] - required           
+;NumberPhotons = [200] 
+;;HO spot scale in [mas] - optional - defaut: [[0.0, 0.0, 0.0]]
+;SpotFWHM = [[0.0,0.0,0.0]]   
+;;ron in [e-] - optional - default: 0.0        
+;SigmaRON = 0.0   
+;;dark current[e-/s/pix] - optional - default: 0.0        
+;Dark = 0.0
+;;sky background [e-/s/pix] - optional - default: 0.0          
+;SkyBackground = 0.0
+;;Pixel gain - optional - default:1.0
+;Gain = 1.0  
+;;excess noise factor - optional - default: 2.0                     
+;ExcessNoiseFactor = 2.0 
+;;number of WFS lenslets - required
+;NumberLenslets = [4]
+;;CoG computation algorithm - optional  - default:'wcog'
+;Algorithm = 'wcog' 
+;;Number of pixels for windiwing the low order WFS pixels - optional - default: 2      
+;WindowRadiusWCoG = 2
+;;Threshold Number of pixels for windowing the low order WFS pixels - optional - default: 0.0        
+;ThresholdWCoG = 0.0
+;;New value for pixels lower than threshold - optional - default: 0.0        
+;NewValueThrPix = 0.0
 
 [DM]
 ;DM actuators pitch in meters - required
 NumberActuators = [80]
 ;DM actuators pitch in meters - required
 DmPitchs = [0.38]
 ;DM influence function model - optional - default: 'gaussian'
@@ -123,12 +196,18 @@
 ; Number of reconstructed layers for tomographic systems - optional - default: 10
 NumberReconstructedLayers= 10
 ;Shape of the AO-corrected area - optional - default: 'circle'
 AoArea = 'circle'
 
 [RTC]
 ;HO Loop gain - required
-LoopGain_HO = 0.8                                
+LoopGain_HO = 0.5                             
 ;HO loop frequency in [Hz] - required
 SensorFrameRate_HO = 500.0
 ;HO loop frame delay - required
-LoopDelaySteps_HO = 1
+LoopDelaySteps_HO = 1   
+; LO loop gain - optional - default: Nome
+LoopGain_LO = 0.5
+;Loop frequency in Hz  - optional - default: None
+SensorFrameRate_LO = 500.0
+;Corresponding delays (in frames)  - optional - default: None
+LoopDelaySteps_LO = 1
```

### Comparing `astro-tiptop-1.1/perfTest/MAVIS.ini` & `astro-tiptop-1.2/perfTest/MAVIS.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/SOUL.ini` & `astro-tiptop-1.2/perfTest/SOUL.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/perfTest/SPHERE.ini` & `astro-tiptop-1.2/perfTest/SPHERE.ini`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/tiptop/tiptop.py` & `astro-tiptop-1.2/tiptop/tiptop.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,74 @@
 from matplotlib import rc
 from p3.aoSystem.fourierModel import *
 from p3.aoSystem.FourierUtils import *
 from configparser import ConfigParser
 import yaml
 
 from mastsel import *
+from mastsel import gpuEnabled as gpuMastsel
+from p3.aoSystem import gpuEnabled as gpuP3
 
 from datetime import datetime
 
 rc("text", usetex=False)
 
+def arrayP3toMastsel(v):
+    if (gpuP3 and gpuMastsel) or (not gpuP3 and not gpuMastsel):
+        return v
+    elif not gpuP3 and gpuMastsel:
+        return cp.asarray(v)
+    elif gpuP3 and not gpuMastsel: 
+        return v.get()
+    
+def cpuArray(v):
+    if isinstance(v,np.ndarray):
+        return v
+    else:
+        return v.get()
+
+def psdSetToPsfSet(N, freq_range, dk, mask, inputPSDs,wavelength,pixelscale,npixel,scaleFactor=1,verbose=False):
+    NGS_SR = []
+    psdArray = []
+    psfLongExpArr = []
+    NGS_FWHM_mas = []
+    for computedPSD in inputPSDs:
+        # Get the PSD at the NGSs positions at the sensing wavelength
+        # computed PSD from fao are given in nm^2, i.e they are multiplied by dk**2 already
+        psd            = Field(wavelength, N, freq_range, 'rad')
+        psd.sampling   = computedPSD / dk**2 # the PSD must be provided in m^2.m^2
+        psdArray.append(psd)
+        # Get the PSF
+        psfLE          = longExposurePsf(mask, psd )
+        # It cuts the PSF if the PSF is larger than the requested dimension
+        if psfLE.sampling.shape[0] > npixel:
+            psfLE.sampling = psfLE.sampling[int(psfLE.sampling.shape[0]/2-npixel/2):int(psfLE.sampling.shape[0]/2+npixel/2),
+                                            int(psfLE.sampling.shape[1]/2-npixel/2):int(psfLE.sampling.shape[1]/2+npixel/2)]
+        psfLongExpArr.append(psfLE)
+        # Get SR and FWHM in mas at the NGSs positions at the sensing wavelength
+        s1=cpuArray(computedPSD).sum()
+        
+        SR             = np.exp(-s1*scaleFactor) # Strehl-ratio at the sensing wavelength
+        
+        NGS_SR.append(SR)
+        FWHMx,FWHMy    = getFWHM( psfLE.sampling, pixelscale, method='contour', nargout=2)
+        FWHM           = np.sqrt(FWHMx*FWHMy) #max(FWHMx, FWHMy) #0.5*(FWHMx+FWHMy) #average over major and minor axes
+        # note : the uncertainities on the FWHM seems to create a bug in mavisLO
+
+
+        NGS_FWHM_mas.append(FWHM)
+        if verbose:
+            print('SR(@',int(wavelength*1e9),'nm)  :', SR)
+            print('FWHM(@',int(wavelength*1e9),'nm):', FWHM)
+
+    return NGS_SR, psdArray, psfLongExpArr, NGS_FWHM_mas
+
 def overallSimulation(path, parametersFile, outputDir, outputFile, doConvolve=False,
                       doPlot=False, returnRes=False, addSrAndFwhm=False,
-                      verbose=False, getHoErrorBreakDown=False):
+                      verbose=False, getHoErrorBreakDown=False, savePSDs=False):
     """
     function to run the entire tiptop simulation based on the imput file
 
     :param path2param: required, path to the parameter file
     :type path2param: str
     :param paramFileName: required, name of the parameter file to be used without the extention
     :type paramFileName: str
@@ -37,197 +89,167 @@
     :param getHoErrorBreakDown: optional default: False, If you want HO error breakdosn set this to True
     :type getHoErrorBreakDown: bool
 
     :return: TBD
     :rtype: TBD
 
     """
-
+    
+    if returnRes and doPlot:
+        print('WARNING: returnRes and doPlot cannot both be True, setting doPlot to False.')
+        doPlot = False
+        
     # initiate the parser
     fullPathFilename_ini = os.path.join(path, parametersFile + '.ini')
     fullPathFilename_yml = os.path.join(path, parametersFile + '.yml')
-
+    
     # initialize jitter_FWHM variable with a default value
     jitter_FWHM = None
 
     if os.path.exists(fullPathFilename_yml):
+        fullPathFilename = fullPathFilename_yml
         with open(fullPathFilename_yml) as f:
-            my_yaml_dict = yaml.safe_load(f)
-        # read main parameters
-        tel_radius = my_yaml_dict['telescope']['TelescopeDiameter']/2  # mas
-        wvl_temp = my_yaml_dict['sources_science']['Wavelength']
-        if isinstance(wvl_temp, list):
-            wvl = wvl_temp[0]  # lambda
-        else:
-            wvl = wvl_temp     # lambda
-        zenithSrc  = my_yaml_dict['sources_science']['Zenith']
-        azimuthSrc = my_yaml_dict['sources_science']['Azimuth']
-
-        # it checks if LO parameters are set and then it acts accordingly
-        if 'sensor_LO' in my_yaml_dict.keys():
-            LOisOn = True
-            if verbose: print('LO part is present')
-        else:
-            LOisOn = False
-            nNaturalGS = 0
-            if verbose: print('LO part is not present')
-
-        if LOisOn:
-            LO_wvl_temp = my_yaml_dict['sources_LO']['Wavelength']
-            if isinstance(LO_wvl_temp, list):
-                LO_wvl = LO_wvl_temp[0]  # lambda
-            else:
-                LO_wvl = LO_wvl_temp     # lambda
-            LO_zen     = my_yaml_dict['sources_LO']['Zenith']
-            LO_az      = my_yaml_dict['sources_LO']['Azimuth']
-            LO_fluxes  = my_yaml_dict['sensor_LO']['NumberPhotons']
-            fr         = my_yaml_dict['RTC']['SensorFrameRate_LO']
-
-        if 'jitter_FWHM' in my_yaml_dict['telescope'].keys():
-            jitter_FWHM = my_yaml_dict['telescope']['jitter_FWHM']
-
-        fao = fourierModel( fullPathFilename_yml, calcPSF=False, verbose=verbose
-                           , display=False, getPSDatNGSpositions=True
-                           , computeFocalAnisoCov=False, TiltFilter=LOisOn
-                           , getErrorBreakDown=getHoErrorBreakDown)
-
+            my_yaml_dict = yaml.safe_load(f)        
+        my_data_map = my_yaml_dict
     elif os.path.exists(fullPathFilename_ini):
-        parser           = ConfigParser()
-        parser.read(fullPathFilename_ini);
-        # read main parameters
-        tel_radius = eval(parser.get('telescope', 'TelescopeDiameter'))/2  # mas
-        wvl_temp = eval(parser.get('sources_science', 'Wavelength'))
-        if isinstance(wvl_temp, list):
-            wvl = wvl_temp[0]  # lambda
-        else:
-            wvl = wvl_temp     # lambda
-        zenithSrc  = eval(parser.get('sources_science', 'Zenith'))
-        azimuthSrc = eval(parser.get('sources_science', 'Azimuth'))
-        # it checks if LO parameters are set and then it acts accordingly
-        if parser.has_section('sensor_LO'):
-            LOisOn = True
-            if verbose: print('LO part is present')
-        else:
-            LOisOn = False
-            nNaturalGS = 0
-            if verbose: print('LO part is not present')
-
-        if LOisOn:
-            LO_wvl_temp = eval(parser.get('sources_LO', 'Wavelength'))
-            if isinstance(LO_wvl_temp, list):
-                LO_wvl = LO_wvl_temp[0]  # lambda
-            else:
-                LO_wvl = LO_wvl_temp     # lambda
-            LO_zen     = eval(parser.get('sources_LO', 'Zenith'))
-            LO_az      = eval(parser.get('sources_LO', 'Azimuth'))
-            LO_fluxes  = eval(parser.get('sensor_LO', 'NumberPhotons'))
-            fr         = eval(parser.get('RTC', 'SensorFrameRate_LO'))
-        if parser.has_option('telescope', 'jitter_FWHM'):
-            jitter_FWHM = eval(parser.get('telescope', 'jitter_FWHM'))
-
-        fao = fourierModel( fullPathFilename_ini, calcPSF=False, verbose=verbose
-                           , display=False, getPSDatNGSpositions=True
-                           , computeFocalAnisoCov=False, TiltFilter=LOisOn
-                           , getErrorBreakDown=getHoErrorBreakDown)
-        
+        fullPathFilename = fullPathFilename_ini
+        config = ConfigParser()
+        config.optionxform = str
+        config.read(fullPathFilename_ini)
+        my_data_map = {} 
+        for section in config.sections():
+            my_data_map[section] = {}
+            for name,value in config.items(section):
+                my_data_map[section].update({name:eval(value)})
     else:
         raise FileNotFoundError('No .yml or .ini can be found in '+ path)
+                  
+    # read main parameters
+    tel_radius = my_data_map['telescope']['TelescopeDiameter']/2  # mas
+    wvl_temp = my_data_map['sources_science']['Wavelength']
+    if isinstance(wvl_temp, list):
+        wvl = wvl_temp[0]  # lambda
+    else:
+        wvl = wvl_temp     # lambda
+    zenithSrc  = my_data_map['sources_science']['Zenith']
+    azimuthSrc = my_data_map['sources_science']['Azimuth']
+
+    # it checks if LO parameters are set and then it acts accordingly
+    if 'sensor_LO' in my_data_map.keys():
+        LOisOn = True
+        if verbose: print('LO part is present')
+    else:
+        LOisOn = False
+        nNaturalGS = 0
+        if verbose: print('LO part is not present')
+
+    if LOisOn:
+        LO_wvl_temp = my_data_map['sources_LO']['Wavelength']
+        if isinstance(LO_wvl_temp, list):
+            LO_wvl = LO_wvl_temp[0]  # lambda
+        else:
+            LO_wvl = LO_wvl_temp     # lambda
+        LO_zen     = my_data_map['sources_LO']['Zenith']
+        LO_az      = my_data_map['sources_LO']['Azimuth']
+        LO_fluxes  = my_data_map['sensor_LO']['NumberPhotons']
+        fr         = my_data_map['RTC']['SensorFrameRate_LO']
+
+    if 'jitter_FWHM' in my_data_map['telescope'].keys():
+        jitter_FWHM = my_data_map['telescope']['jitter_FWHM']
+
+    fao = fourierModel( fullPathFilename, calcPSF=False, verbose=verbose
+                       , display=False, getPSDatNGSpositions=True
+                       , computeFocalAnisoCov=False, TiltFilter=LOisOn
+                       , getErrorBreakDown=getHoErrorBreakDown)
 
     if LOisOn:
         # NGSs positions
         NGS_flux = []
         polarNGSCoordsList = []
         for aFlux, aZen, aAz in zip(LO_fluxes, LO_zen, LO_az):
             polarNGSCoordsList.append([aZen, aAz])
-            NGS_flux.append(LO_fluxes[0]*fr)
+            NGS_flux.append(aFlux*fr)
             polarNGSCoords     = np.asarray(polarNGSCoordsList)
             nNaturalGS         = polarNGSCoords.shape[0]
 
     pp                 = polarToCartesian(np.array( [zenithSrc, azimuthSrc]))
     xxPointigs         = pp[0,:]
     yyPointigs         = pp[1,:]
 
     # High-order PSD caculations at the science directions and NGSs directions
     PSD                = fao.PSD # in nm^2
+        
     nPointings         = pp.shape[1]
     if verbose:
         print('******** HO PSD science and NGSs directions')
 
     PSD           = PSD.transpose()
     N             = PSD[0].shape[0]
+    nPixPSF       = int(fao.freq.nOtf /fao.freq.kRef_)
     freq_range    = fao.ao.cam.fovInPix*fao.freq.PSDstep
     pitch         = 1/freq_range
     grid_diameter = pitch*N
     sx            = int(2*np.round(tel_radius/pitch))
     dk            = 1e9*fao.freq.kcMax_/fao.freq.resAO
 
     # Define the pupil shape
     mask = Field(wvl, N, grid_diameter)
-    mask.sampling = cp.asarray(congrid(fao.ao.tel.pupil, [sx, sx]))
+
+    psInMas = cpuArray(fao.freq.psInMas)
+
+    mask.sampling = congrid(arrayP3toMastsel(fao.ao.tel.pupil), [sx, sx])
+        
     mask.sampling = zeroPad(mask.sampling, (N-sx)//2)
+    
     if verbose:
         print('fao.samp:', fao.freq.samp)
-        print('fao.freq.psInMas:', fao.freq.psInMas)
-
-    def psdSetToPsfSet(inputPSDs,wavelength,pixelscale,scaleFactor=1,verbose=False):
-        NGS_SR = []
-        psdArray = []
-        psfLongExpArr = []
-        NGS_FWHM_mas = []
-        for computedPSD in inputPSDs:
-            # Get the PSD at the NGSs positions at the sensing wavelength
-            # computed PSD from fao are given in nm^2, i.e they are multiplied by dk**2 already
-            psd            = Field(wavelength, N, freq_range, 'rad')
-            psd.sampling   = cp.asarray( computedPSD / dk**2) # the PSD must be provided in m^2.m^2
-            psdArray.append(psd)
-            # Get the PSF
-            psfLE          = longExposurePsf(mask, psd )
-            psfLongExpArr.append(psfLE)
-            # Get SR and FWHM in mas at the NGSs positions at the sensing wavelength
-            SR             = np.exp(-computedPSD.sum()* scaleFactor) # Strehl-ratio at the sensing wavelength
-            NGS_SR.append(SR)
-            FWHMx,FWHMy    = getFWHM( psfLE.sampling, pixelscale, method='contour', nargout=2)
-            FWHM           = np.sqrt(FWHMx*FWHMy) #max(FWHMx, FWHMy) #0.5*(FWHMx+FWHMy) #average over major and minor axes
-            # note : the uncertainities on the FWHM seems to create a bug in mavisLO
-            NGS_FWHM_mas.append(FWHM)
-            if verbose:
-                print('SR(@',int(wavelength*1e9),'nm)  :', SR)
-                print('FWHM(@',int(wavelength*1e9),'nm):', FWHM)
-
-        return NGS_SR, psdArray, psfLongExpArr, NGS_FWHM_mas
+        print('fao.PSD.shape:', fao.PSD.shape)
+        print('fao.freq.psInMas:', psInMas)
 
     # HO PSF
     if verbose:
         print('******** HO PSF')
-    pointings_SR, psdPointingsArray, psfLongExpPointingsArr, pointings_FWHM_mas = psdSetToPsfSet(PSD[0:nPointings],
+    
+    pointings_SR, psdPointingsArray, psfLongExpPointingsArr, pointings_FWHM_mas = psdSetToPsfSet(N, 
+                                                                                                 freq_range, 
+                                                                                                 dk,
+                                                                                                 mask, 
+                                                                                                 arrayP3toMastsel(PSD[0:nPointings]),
                                                                                                  wvl,
-                                                                                                 fao.freq.psInMas[0],
+                                                                                                 psInMas[0],
+                                                                                                 nPixPSF,
                                                                                                  scaleFactor=(2*np.pi*1e-9/wvl)**2,
                                                                                                  verbose=verbose)
 
     if LOisOn == False or (doConvolve == False and returnRes == False):
         results = []
         for psfLongExp in psfLongExpPointingsArr:
             if jitter_FWHM is not None:
                 ellp = [0, sigma_from_FWHM(jitter_FWHM), sigma_from_FWHM(jitter_FWHM)]
                 results.append(convolve(psfLongExp,
-                               residualToSpectrum(ellp, wvl, N, 1/(fao.ao.cam.fovInPix * fao.freq.psInMas[0]))))
+                               residualToSpectrum(ellp, wvl, N, 1/(fao.ao.cam.fovInPix * psInMas[0]))))
             else:
                 results.append(psfLongExp)
 
     else:
         # LOW ORDER PART
         if verbose:
             print('******** LO PART')
-        psInMas_NGS        = fao.freq.psInMas[0] * (LO_wvl/wvl) #airy pattern PSF FWHM
+        psInMas_NGS        = psInMas[0] * (LO_wvl/wvl) #airy pattern PSF FWHM
 
         if verbose:
             print('******** HO PSF - NGS directions')
-        NGS_SR, psdArray, psfLE_NGS, NGS_FWHM_mas = psdSetToPsfSet(PSD[-nNaturalGS:],
-                                                                   LO_wvl, psInMas_NGS,
+        NGS_SR, psdArray, psfLE_NGS, NGS_FWHM_mas = psdSetToPsfSet(N, 
+                                                                   freq_range, 
+                                                                   dk, 
+                                                                   mask, 
+                                                                   arrayP3toMastsel(PSD[-nNaturalGS:]), 
+                                                                   LO_wvl, 
+                                                                   psInMas_NGS, 
+                                                                   nPixPSF,
                                                                    scaleFactor=(2*np.pi*1e-9/LO_wvl)**2,
                                                                    verbose=verbose)
 
         cartPointingCoords = np.dstack( (xxPointigs, yyPointigs) ).reshape(-1, 2)
         cartNGSCoordsList = []
         for i in range(nNaturalGS):
             cartNGSCoordsList.append(polarToCartesian(polarNGSCoords[i,:]))
@@ -243,17 +265,16 @@
                 for n in range(cov_ellipses.shape[0]):
                     print('cov_ellipses #',n,': ',cov_ellipses[n,:], ' (unit: rad, mas, mas)')
             # FINAl CONVOLUTION
             if verbose:
                 print('******** FINAL CONVOLUTION')
             results = []
             for ellp, psfLongExp in zip(cov_ellipses, psfLongExpPointingsArr):
-                results.append(convolve(psfLongExp, residualToSpectrum(ellp, wvl
-                                                                       , N, 1/(fao.ao.cam.fovInPix
-                                                                               * fao.freq.psInMas[0]))))
+                resSpec = residualToSpectrum(ellp, wvl, N, 1/(fao.ao.cam.fovInPix * psInMas[0]))
+                results.append(convolve(psfLongExp, resSpec))
 
     if doPlot:
         if LOisOn and doConvolve and returnRes == False:
             tiledDisplay(results)
             plotEllipses(cartPointingCoords, cov_ellipses, 0.4)
         else:
             results[0].standardPlot(True)
@@ -275,25 +296,35 @@
             return HO_res
     else:
         # OPEN-LOOP PSD
         k   = np.sqrt(fao.freq.k2_)
         pf  = FourierUtils.pistonFilter(fao.ao.tel.D,k)
         psdOL = Field(wvl, N, freq_range, 'rad')
         temp = fao.ao.atm.spectrum(k) * pf
-        psdOL.sampling = cp.asarray(fao.ao.atm.spectrum(k) * pf * (fao.freq.wvlRef/np.pi)**2) # the PSD must be provided in m^2.m^2
+        psdOL.sampling = arrayP3toMastsel(fao.ao.atm.spectrum(k) * pf * (fao.freq.wvlRef/np.pi)**2) # the PSD must be provided in m^2.m^2
         # Get the OPEN-LOOP PSF
         psfOL = longExposurePsf(mask, psdOL)
+        # It cuts the PSF if the PSF is larger than the requested dimension (N>nPixPSF)
+#        if psfOL.sampling.shape[0] > nPixPSF:
+#            psfOL.sampling = psfOL.sampling[int(psfOL.sampling.shape[0]/2-nPixPSF/2):int(psfOL.sampling.shape[0]/2+nPixPSF/2),
+#                                            int(psfOL.sampling.shape[1]/2-nPixPSF/2):int(psfOL.sampling.shape[1]/2+nPixPSF/2)]
+#        psfOL.sampling = cpuArray(psdOL.sampling)
+
         if doPlot:
             fig, ax1 = plt.subplots(1,1)
             im = ax1.imshow(np.log(np.abs(psfOL.sampling) + 1e-20), cmap='hot')
             ax1.set_title('open loop PSF', color='black')
             
         # DIFFRACTION LIMITED PSD
         psdDL = Field(wvl, N, freq_range, 'rad')
         psfDL = longExposurePsf(mask, psdDL)
+        # It cuts the PSF if the PSF is larger than the requested dimension (N>nPixPSF)
+        if psfDL.sampling.shape[0] > nPixPSF:
+            psfDL.sampling = psfDL.sampling[int(psfDL.sampling.shape[0]/2-nPixPSF/2):int(psfDL.sampling.shape[0]/2+nPixPSF/2),
+                                            int(psfDL.sampling.shape[1]/2-nPixPSF/2):int(psfDL.sampling.shape[1]/2+nPixPSF/2)]
         if doPlot:
             fig, ax2 = plt.subplots(1,1)
             im = ax2.imshow(np.log(np.abs(psfDL.sampling) + 1e-20), cmap='hot')
             ax2.set_title('diffraction limited PSF', color='black')
 
         # save PSF cube in fits
         hdul1 = fits.HDUList()
@@ -302,58 +333,75 @@
         for img in results:
             cube.append(img.sampling)
 
         cube = np.array(cube)
         hdul1.append(fits.ImageHDU(data=cube))
         hdul1.append(fits.ImageHDU(data=psfOL.sampling)) # append open-loop PSF
         hdul1.append(fits.ImageHDU(data=psfDL.sampling)) # append diffraction limited PSF
+        if savePSDs:
+            hdul1.append(fits.ImageHDU(data=cpuArray(PSD))) # append high order PSD
+
 
         #############################
         # header
         hdr0 = hdul1[0].header
         now = datetime.now()
         hdr0['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         # parameters in the header
-        if os.path.exists(fullPathFilename_yml):
-            for key_primary in my_yaml_dict:
-                for key_secondary in my_yaml_dict[key_primary]:
-                    temp = my_yaml_dict[key_primary][key_secondary]
-                    if isinstance(temp, list):
-                        iii = 0
-                        for elem in temp:
+        for key_primary in my_data_map:
+            for key_secondary in my_data_map[key_primary]:
+                temp = my_data_map[key_primary][key_secondary]
+                if isinstance(temp, list):
+                    iii = 0
+                    for elem in temp:
+                        if isinstance(elem, list):
+                            jjj = 0
+                            for elem2 in elem:
+                                hdr0['HIERARCH '+key_primary+' '+key_secondary +' '+str(iii)+' '+str(jjj)] = elem2
+                                jjj += 1
+                        else:                        
                             hdr0['HIERARCH '+key_primary+' '+key_secondary +' '+str(iii)] = elem
-                            iii += 1
-                    else:
-                        hdr0['HIERARCH '+key_primary+' '+key_secondary] = temp
+                    iii += 1
+                else:
+                    hdr0['HIERARCH '+key_primary+' '+key_secondary] = temp
+                    
         # header of the PSFs
         hdr1 = hdul1[1].header
         hdr1['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         hdr1['CONTENT'] = "PSF CUBE"
         hdr1['SIZE'] = str(cube.shape)
         hdr1['WL_NM'] = str(int(wvl*1e9))
-        hdr1['PIX_MAS'] = str(fao.freq.psInMas[0])
+        hdr1['PIX_MAS'] = str(psInMas[0])
         hdr1['CC'] = "CARTESIAN COORD. IN ASEC OF THE "+str(pp.shape[1])+" SOURCES"
         for i in range(pp.shape[1]):
             hdr1['CCX'+str(i).zfill(4)] = pp[0,i]
             hdr1['CCY'+str(i).zfill(4)] = pp[1,i]
         if addSrAndFwhm:
             for i in range(cube.shape[0]):
                 hdr1['SR'+str(i).zfill(4)]   = getStrehl(cube[i,:,:], fao.ao.tel.pupil, fao.freq.sampRef)
             for i in range(cube.shape[0]):
-                hdr1['FWHM'+str(i).zfill(4)] = getFWHM(cube[i,:,:], fao.freq.psInMas[0], method='contour', nargout=1)
+                hdr1['FWHM'+str(i).zfill(4)] = getFWHM(cube[i,:,:], psInMas[0], method='contour', nargout=1)
 
         # header of the OPEN-LOOP PSF
         hdr2 = hdul1[2].header
         hdr2['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         hdr2['CONTENT'] = "OPEN-LOOP PSF"
         hdr2['SIZE'] = str(psfOL.sampling.shape)
         
         # header of the DIFFRACTION LIMITED PSF
         hdr3 = hdul1[3].header
         hdr3['TIME'] = now.strftime("%Y%m%d_%H%M%S")
         hdr3['CONTENT'] = "DIFFRACTION LIMITED PSF"
         hdr3['SIZE'] = str(psfDL.sampling.shape)
+
+        if savePSDs:
+            # header of the PSD
+            hdr4 = hdul1[4].header
+            hdr4['TIME'] = now.strftime("%Y%m%d_%H%M%S")
+            hdr4['CONTENT'] = "High Order PSD"
+            hdr4['SIZE'] = str(PSD.shape)
+
         #############################
 
         hdul1.writeto( os.path.join(outputDir, outputFile + '.fits'), overwrite=True)
         if verbose:
             print("Output cube shape:", cube.shape)
```

### Comparing `astro-tiptop-1.1/tiptop/tiptopCLT.py` & `astro-tiptop-1.2/tiptop/tiptopCLT.py`

 * *Files identical despite different names*

### Comparing `astro-tiptop-1.1/tiptop/tiptopGUI.py` & `astro-tiptop-1.2/tiptop/tiptopGUI.py`

 * *Files identical despite different names*

