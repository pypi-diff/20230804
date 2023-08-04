# Comparing `tmp/meow-sim-0.7.1.tar.gz` & `tmp/meow-sim-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.7.1.tar", last modified: Sun Jul  9 20:23:05 2023, max compression
+gzip compressed data, was "meow-sim-0.7.2.tar", last modified: Fri Aug  4 02:41:27 2023, max compression
```

## Comparing `meow-sim-0.7.1.tar` & `meow-sim-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-07-09 20:23:00.000000 meow-sim-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-07-09 20:23:05.004513 meow-sim-0.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-09 20:23:00.000000 meow-sim-0.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/
--rw-r--r--   0 root         (0) root         (0)     3747 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     8828 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/propagate.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    12464 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12796 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17433 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8092 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-09 20:23:00.000000 meow-sim-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 20:23:05.004513 meow-sim-0.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/tests/
--rw-r--r--   0 root         (0) root         (0)      359 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.118081 meow-sim-0.7.2/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-08-04 02:41:22.000000 meow-sim-0.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 02:41:27.118081 meow-sim-0.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-08-04 02:41:22.000000 meow-sim-0.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.106081 meow-sim-0.7.2/meow/
+-rw-r--r--   0 root         (0) root         (0)     3747 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.106081 meow-sim-0.7.2/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8828 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.110081 meow-sim-0.7.2/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.110081 meow-sim-0.7.2/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17433 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-08-04 02:41:22.000000 meow-sim-0.7.2/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.114081 meow-sim-0.7.2/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 02:41:27.000000 meow-sim-0.7.2/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-08-04 02:41:27.000000 meow-sim-0.7.2/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 02:41:27.000000 meow-sim-0.7.2/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      446 2023-08-04 02:41:27.000000 meow-sim-0.7.2/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 02:41:27.000000 meow-sim-0.7.2/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-08-04 02:41:22.000000 meow-sim-0.7.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 02:41:27.118081 meow-sim-0.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 02:41:27.114081 meow-sim-0.7.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-08-04 02:41:22.000000 meow-sim-0.7.2/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-08-04 02:41:22.000000 meow-sim-0.7.2/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-08-04 02:41:22.000000 meow-sim-0.7.2/tests/test_nbs.py
```

### Comparing `meow-sim-0.7.1/LICENSE` & `meow-sim-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/PKG-INFO` & `meow-sim-0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.7.1
+Version: 0.7.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.7.1/README.md` & `meow-sim-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/__init__.py` & `meow-sim-0.7.2/meow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.7.1/meow/assets/silicon.csv` & `meow-sim-0.7.2/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/assets/silicon_oxide.csv` & `meow-sim-0.7.2/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/base_model.py` & `meow-sim-0.7.2/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/cache.py` & `meow-sim-0.7.2/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/cell.py` & `meow-sim-0.7.2/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/cross_section.py` & `meow-sim-0.7.2/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/eme/__init__.py` & `meow-sim-0.7.2/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/eme/common.py` & `meow-sim-0.7.2/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/eme/propagate.py` & `meow-sim-0.7.2/meow/eme/propagate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/eme/sax.py` & `meow-sim-0.7.2/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/environment.py` & `meow-sim-0.7.2/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/fde/lumerical.py` & `meow-sim-0.7.2/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/fde/tidy3d.py` & `meow-sim-0.7.2/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/gds_structures.py` & `meow-sim-0.7.2/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/geometries.py` & `meow-sim-0.7.2/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/integrate.py` & `meow-sim-0.7.2/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/materials.py` & `meow-sim-0.7.2/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/mesh.py` & `meow-sim-0.7.2/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/mode.py` & `meow-sim-0.7.2/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/structures.py` & `meow-sim-0.7.2/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow/visualize.py` & `meow-sim-0.7.2/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.7.2/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.7.1
+Version: 0.7.2
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.7.1/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.7.2/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/pyproject.toml` & `meow-sim-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
@@ -32,15 +32,15 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
   "matplotlib",
   "numpy>=1.24",
-  "pydantic",
+  "pydantic<2",
   "sax>=0.8.4",
   "scipy",
   "shapely",
   "tidy3d>=2.1",
   "trimesh[easy]",
   "packaging",
 ]
```

### Comparing `meow-sim-0.7.1/tests/test_mode_operators.py` & `meow-sim-0.7.2/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.1/tests/test_nbs.py` & `meow-sim-0.7.2/tests/test_nbs.py`

 * *Files identical despite different names*

