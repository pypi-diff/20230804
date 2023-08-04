# Comparing `tmp/atooms-pp-3.3.1.tar.gz` & `tmp/atooms-pp-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms-pp-3.3.1.tar", last modified: Thu Aug  3 17:23:34 2023, max compression
+gzip compressed data, was "atooms-pp-3.3.2.tar", last modified: Thu Aug  3 20:25:06 2023, max compression
```

## Comparing `atooms-pp-3.3.1.tar` & `atooms-pp-3.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.3.1/LICENSE
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.3.1/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.203422 atooms-pp-3.3.1/atooms/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.3.1/atooms/__init__.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      705 2023-08-03 14:31:56.000000 atooms-pp-3.3.1/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.3.1/atooms/postprocessing/_commit.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-08-03 17:23:32.000000 atooms-pp-3.3.1/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15568 2023-08-03 17:17:23.000000 atooms-pp-3.3.1/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.3.1/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.3.1/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.3.1/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.3.1/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.3.1/atooms/postprocessing/fourierspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15946 2023-08-03 17:10:40.000000 atooms-pp-3.3.1/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13996 2023-07-01 09:58:27.000000 atooms-pp-3.3.1/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.3.1/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.3.1/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.3.1/atooms/postprocessing/realspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.3.1/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9945 2023-08-03 15:53:28.000000 atooms-pp-3.3.1/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.3.1/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/atooms_pp.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-08-03 17:23:34.000000 atooms-pp-3.3.1/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.3.1/bin/acf.py
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.3.1/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-08-03 17:23:34.207422 atooms-pp-3.3.1/setup.cfg
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.3.1/setup.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.3.2/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.3.2/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 20:25:06.199592 atooms-pp-3.3.2/atooms/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.3.2/atooms/__init__.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      705 2023-08-03 14:31:56.000000 atooms-pp-3.3.2/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.3.2/atooms/postprocessing/_commit.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-08-03 20:25:05.000000 atooms-pp-3.3.2/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15568 2023-08-03 17:17:23.000000 atooms-pp-3.3.2/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.3.2/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.3.2/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.3.2/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.3.2/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.3.2/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.3.2/atooms/postprocessing/fourierspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15781 2023-08-03 19:56:33.000000 atooms-pp-3.3.2/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13996 2023-07-01 09:58:27.000000 atooms-pp-3.3.2/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.3.2/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.3.2/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.3.2/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.3.2/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.3.2/atooms/postprocessing/realspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.3.2/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9945 2023-08-03 15:53:28.000000 atooms-pp-3.3.2/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.3.2/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/atooms_pp.egg-info/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-08-03 20:25:06.000000 atooms-pp-3.3.2/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-08-03 20:25:06.000000 atooms-pp-3.3.2/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-08-03 20:25:06.000000 atooms-pp-3.3.2/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-08-03 20:25:06.000000 atooms-pp-3.3.2/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-08-03 20:25:06.000000 atooms-pp-3.3.2/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.3.2/bin/acf.py
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.3.2/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-08-03 20:25:06.203592 atooms-pp-3.3.2/setup.cfg
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.3.2/setup.py
```

### Comparing `atooms-pp-3.3.1/LICENSE` & `atooms-pp-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/PKG-INFO` & `atooms-pp-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.3.1
+Version: 3.3.2
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.3.1/README.md` & `atooms-pp-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/__init__.py` & `atooms-pp-3.3.2/atooms/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/alpha2.py` & `atooms-pp-3.3.2/atooms/postprocessing/alpha2.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/api.py` & `atooms-pp-3.3.2/atooms/postprocessing/api.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/ba.py` & `atooms-pp-3.3.2/atooms/postprocessing/ba.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/chi4t.py` & `atooms-pp-3.3.2/atooms/postprocessing/chi4t.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/core.py` & `atooms-pp-3.3.2/atooms/postprocessing/core.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/correlation.py` & `atooms-pp-3.3.2/atooms/postprocessing/correlation.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/filter.py` & `atooms-pp-3.3.2/atooms/postprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/fkt.py` & `atooms-pp-3.3.2/atooms/postprocessing/fkt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/fourierspace.f90` & `atooms-pp-3.3.2/atooms/postprocessing/fourierspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/fourierspace.py` & `atooms-pp-3.3.2/atooms/postprocessing/fourierspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,21 +259,22 @@
         self.k0 = []
         
         # Some internal variables
         # compatible with the boundary conditions
         self._kvectors = []
         self._koffset = 0
 
-    # TODO: by adding setup() when can postpone grid setup. This way we need not compute the grid too early and we can more easily respect the update argument of do().
-    # TODO: we actually need only the cell here! Not the trajectory.
     def setup(self, side):
         # Smallest kvector
-        self.k0 = 2*math.pi / side
+        k0 = 2*math.pi / side
+        if numpy.all(self.k0 == k0):
+            return
         
         # Setup the grid of wave-vectors
+        self.k0 = k0
         if self.kvectors_input is not None:
             self._kvectors, self._koffset = self._setup_from_kvectors(self.kvectors_input, self.k0)
         else:
             # If kgrid of kvectors are not provided, setup a linear grid from kmin,kmax,ksamples data
             # TODO: This shouldnt be allowed with fluctuating cells
             # Or we should fix the smallest k to some average of smallest k per sample
             if self.kgrid is None:
```

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/gr.py` & `atooms-pp-3.3.2/atooms/postprocessing/gr.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/helpers.py` & `atooms-pp-3.3.2/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/ik.py` & `atooms-pp-3.3.2/atooms/postprocessing/ik.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/linkedcells.py` & `atooms-pp-3.3.2/atooms/postprocessing/linkedcells.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/msd.py` & `atooms-pp-3.3.2/atooms/postprocessing/msd.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/partial.py` & `atooms-pp-3.3.2/atooms/postprocessing/partial.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/progress.py` & `atooms-pp-3.3.2/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/qt.py` & `atooms-pp-3.3.2/atooms/postprocessing/qt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/realspace.f90` & `atooms-pp-3.3.2/atooms/postprocessing/realspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/s4kt.py` & `atooms-pp-3.3.2/atooms/postprocessing/s4kt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/sacf.py` & `atooms-pp-3.3.2/atooms/postprocessing/sacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/sk.py` & `atooms-pp-3.3.2/atooms/postprocessing/sk.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/susceptibility.py` & `atooms-pp-3.3.2/atooms/postprocessing/susceptibility.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms/postprocessing/vacf.py` & `atooms-pp-3.3.2/atooms/postprocessing/vacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/atooms_pp.egg-info/PKG-INFO` & `atooms-pp-3.3.2/atooms_pp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.3.1
+Version: 3.3.2
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `atooms-pp-3.3.1/atooms_pp.egg-info/SOURCES.txt` & `atooms-pp-3.3.2/atooms_pp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/bin/acf.py` & `atooms-pp-3.3.2/bin/acf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/bin/pp.py` & `atooms-pp-3.3.2/bin/pp.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.3.1/setup.py` & `atooms-pp-3.3.2/setup.py`

 * *Files identical despite different names*

