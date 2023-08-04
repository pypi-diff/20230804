# Comparing `tmp/pykrack-0.0.2.tar.gz` & `tmp/pykrack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrack-0.0.2.tar", last modified: Wed Apr 12 14:09:59 2023, max compression
+gzip compressed data, was "pykrack-0.0.3.tar", last modified: Fri Aug  4 13:43:47 2023, max compression
```

## Comparing `pykrack-0.0.2.tar` & `pykrack-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.191664 pykrack-0.0.2/
--rw-rw-r--   0 ferran    (1000) ferran    (1000)    11337 2023-01-20 02:50:04.000000 pykrack-0.0.2/LICENSE
--rw-rw-r--   0 ferran    (1000) ferran    (1000)      111 2023-01-20 02:50:04.000000 pykrack-0.0.2/MANIFEST.in
--rw-r--r--   0 ferran    (1000) ferran    (1000)     3615 2023-04-12 14:09:59.190664 pykrack-0.0.2/PKG-INFO
--rw-r--r--   0 ferran    (1000) ferran    (1000)     2823 2023-04-12 14:02:23.000000 pykrack-0.0.2/README.md
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.189664 pykrack-0.0.2/pykrack/
--rw-r--r--   0 ferran    (1000) ferran    (1000)       22 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/__init__.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)      524 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/_modidx.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)      800 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/core.py
--rw-r--r--   0 ferran    (1000) ferran    (1000)     2721 2023-04-12 14:09:32.000000 pykrack-0.0.2/pykrack/hierarchy.py
-drwxr-xr-x   0 ferran    (1000) ferran    (1000)        0 2023-04-12 14:09:59.190664 pykrack-0.0.2/pykrack.egg-info/
--rw-r--r--   0 ferran    (1000) ferran    (1000)     3615 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/PKG-INFO
--rw-r--r--   0 ferran    (1000) ferran    (1000)      345 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/SOURCES.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/dependency_links.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)       36 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/entry_points.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        1 2023-04-04 13:10:52.000000 pykrack-0.0.2/pykrack.egg-info/not-zip-safe
--rw-r--r--   0 ferran    (1000) ferran    (1000)       34 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/requires.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)        8 2023-04-12 14:09:59.000000 pykrack-0.0.2/pykrack.egg-info/top_level.txt
--rw-r--r--   0 ferran    (1000) ferran    (1000)      846 2023-04-12 14:06:42.000000 pykrack-0.0.2/settings.ini
--rw-r--r--   0 ferran    (1000) ferran    (1000)       38 2023-04-12 14:09:59.191664 pykrack-0.0.2/setup.cfg
--rw-rw-r--   0 ferran    (1000) ferran    (1000)     2560 2023-01-20 02:50:04.000000 pykrack-0.0.2/setup.py
+drwxr-xr-x   0 ferran     (501) staff       (20)        0 2023-08-04 13:43:47.605898 pykrack-0.0.3/
+-rw-r--r--   0 ferran     (501) staff       (20)    11337 2023-03-28 13:28:58.000000 pykrack-0.0.3/LICENSE
+-rw-r--r--   0 ferran     (501) staff       (20)      111 2023-03-28 13:28:58.000000 pykrack-0.0.3/MANIFEST.in
+-rw-r--r--   0 ferran     (501) staff       (20)     3788 2023-08-04 13:43:47.605593 pykrack-0.0.3/PKG-INFO
+-rw-r--r--   0 ferran     (501) staff       (20)     2996 2023-08-01 14:51:03.000000 pykrack-0.0.3/README.md
+drwxr-xr-x   0 ferran     (501) staff       (20)        0 2023-08-04 13:43:47.602344 pykrack-0.0.3/pykrack/
+-rw-r--r--   0 ferran     (501) staff       (20)       22 2023-08-04 13:37:04.000000 pykrack-0.0.3/pykrack/__init__.py
+-rw-r--r--   0 ferran     (501) staff       (20)      641 2023-08-04 13:37:04.000000 pykrack-0.0.3/pykrack/_modidx.py
+-rw-r--r--   0 ferran     (501) staff       (20)      800 2023-05-26 08:23:05.000000 pykrack-0.0.3/pykrack/core.py
+-rw-r--r--   0 ferran     (501) staff       (20)     2898 2023-08-04 13:37:04.000000 pykrack-0.0.3/pykrack/hierarchy.py
+-rw-r--r--   0 ferran     (501) staff       (20)      800 2023-08-04 13:37:04.000000 pykrack-0.0.3/pykrack/utils.py
+drwxr-xr-x   0 ferran     (501) staff       (20)        0 2023-08-04 13:43:47.605257 pykrack-0.0.3/pykrack.egg-info/
+-rw-r--r--   0 ferran     (501) staff       (20)     3788 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/PKG-INFO
+-rw-r--r--   0 ferran     (501) staff       (20)      362 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/SOURCES.txt
+-rw-r--r--   0 ferran     (501) staff       (20)        1 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/dependency_links.txt
+-rw-r--r--   0 ferran     (501) staff       (20)       36 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/entry_points.txt
+-rw-r--r--   0 ferran     (501) staff       (20)        1 2023-08-01 14:50:58.000000 pykrack-0.0.3/pykrack.egg-info/not-zip-safe
+-rw-r--r--   0 ferran     (501) staff       (20)       34 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/requires.txt
+-rw-r--r--   0 ferran     (501) staff       (20)        8 2023-08-04 13:43:47.000000 pykrack-0.0.3/pykrack.egg-info/top_level.txt
+-rw-r--r--   0 ferran     (501) staff       (20)      846 2023-08-04 13:43:40.000000 pykrack-0.0.3/settings.ini
+-rw-r--r--   0 ferran     (501) staff       (20)       38 2023-08-04 13:43:47.605973 pykrack-0.0.3/setup.cfg
+-rw-r--r--   0 ferran     (501) staff       (20)     2560 2023-03-28 13:28:58.000000 pykrack-0.0.3/setup.py
```

### Comparing `pykrack-0.0.2/LICENSE` & `pykrack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.2/PKG-INFO` & `pykrack-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pykrack
-Version: 0.0.2
-Summary: Computing Krackhardt hierarchy score on netowrkX graphs
+Version: 0.0.3
+Summary: Computing Krackhardt hierarchy score on NetowrkX graphs
 Home-page: https://github.com/FerranC96/pykrack
 Author: FerranC96
 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,18 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+![CI](https://github.com/FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg)
+[![PyPI
+version](https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack)
+
 ## Install
 
 Due to the comparisons with the R package `sna` we recommend using conda
 to manage your environment.
 
 1.  First create the pykrack conda environment from the environment.yml
     file:
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: pykrack Version: 0.0.2 Summary: Computing
-Krackhardt hierarchy score on netowrkX graphs Home-page: https://github.com/
+Metadata-Version: 2.1 Name: pykrack Version: 0.0.3 Summary: Computing
+Krackhardt hierarchy score on NetowrkX graphs Home-page: https://github.com/
 FerranC96/pykrack Author: FerranC96 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE # pyKrack  ## Install Due to the
-comparisons with the R package `sna` we recommend using conda to manage your
-environment. 1. First create the pykrack conda environment from the
-environment.yml file: ``` sh conda (or mamba) env create -f environment.yml ```
-2. Then load the conda environment with: ``` sh conda activate pykrack ``` 3.
-And finally install the package from pip via the following command: ``` sh pip
-install pyKrack ``` Alternatively pyKrack can also be isntalled using pip via
-the following command ``` sh pip install pyKrack ``` Then install the R
-dependencies listed in the conda environmnet.yml manually. ## How to use Please
-see the core and hierarchy notebooks for more detailed explanations.
-**pyKrack** consists of one main function, [`compute_hierarchy`](https://
-FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). ----------------
--------------------------------------------------------- source ###
-compute_hierarchy > compute_hierarchy (G, metric='pykrack') Compute one of the
-possible hierarchy scores | | **Type** | **Default** | **Details** | |---------
-----|-----------|-------------|------------------------------------------------
+Provides-Extra: dev License-File: LICENSE # pyKrack  ![CI](https://github.com/
+FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg) [![PyPI version]
+(https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack) ##
+Install Due to the comparisons with the R package `sna` we recommend using
+conda to manage your environment. 1. First create the pykrack conda environment
+from the environment.yml file: ``` sh conda (or mamba) env create -
+f environment.yml ``` 2. Then load the conda environment with: ``` sh conda
+activate pykrack ``` 3. And finally install the package from pip via the
+following command: ``` sh pip install pyKrack ``` Alternatively pyKrack can
+also be isntalled using pip via the following command ``` sh pip install
+pyKrack ``` Then install the R dependencies listed in the conda environmnet.yml
+manually. ## How to use Please see the core and hierarchy notebooks for more
+detailed explanations. **pyKrack** consists of one main function,
+[`compute_hierarchy`](https://FerranC96.github.io/pykrack/
+hierarchy.html#compute_hierarchy). --------------------------------------------
+---------------------------- source ### compute_hierarchy > compute_hierarchy
+(G, metric='pykrack') Compute one of the possible hierarchy scores | | **Type**
+| **Default** | **Details** | |-------------|-----------|-------------|--------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------| | G | | | Directed
-NetworkX graph | | metric | str | pykrack | Type of hierarchy metric to
-compute. Accepted types are:
+-------------------------------------------------------------------------------
+-------------------| | G | | | Directed NetworkX graph | | metric | str |
+pykrack | Type of hierarchy metric to compute. Accepted types are:
 âpykrackâ for this moduleâs implementation of the Krackhardt score.
 ârsnakrackâ for the sna implementation in R.
 âhierarchy_flowâ for the Luo and Magee 2011 as implemented in the NetworkX
 package. | | **Returns** | **float** | | **One of the possible hierarchy
 scores** |
```

### Comparing `pykrack-0.0.2/README.md` & `pykrack-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+![CI](https://github.com/FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg)
+[![PyPI
+version](https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack)
+
 ## Install
 
 Due to the comparisons with the R package `sna` we recommend using conda
 to manage your environment.
 
 1.  First create the pykrack conda environment from the environment.yml
     file:
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-# pyKrack  ## Install Due to the comparisons with the R package `sna` we
-recommend using conda to manage your environment. 1. First create the pykrack
-conda environment from the environment.yml file: ``` sh conda (or mamba) env
-create -f environment.yml ``` 2. Then load the conda environment with: ``` sh
-conda activate pykrack ``` 3. And finally install the package from pip via the
-following command: ``` sh pip install pyKrack ``` Alternatively pyKrack can
-also be isntalled using pip via the following command ``` sh pip install
-pyKrack ``` Then install the R dependencies listed in the conda environmnet.yml
-manually. ## How to use Please see the core and hierarchy notebooks for more
-detailed explanations. **pyKrack** consists of one main function,
-[`compute_hierarchy`](https://FerranC96.github.io/pykrack/
+# pyKrack  ![CI](https://github.com/FerranC96/pyKrack/actions/workflows/
+test.yaml/badge.svg) [![PyPI version](https://badge.fury.io/py/pykrack.svg)]
+(https://badge.fury.io/py/pykrack) ## Install Due to the comparisons with the R
+package `sna` we recommend using conda to manage your environment. 1. First
+create the pykrack conda environment from the environment.yml file: ``` sh
+conda (or mamba) env create -f environment.yml ``` 2. Then load the conda
+environment with: ``` sh conda activate pykrack ``` 3. And finally install the
+package from pip via the following command: ``` sh pip install pyKrack ```
+Alternatively pyKrack can also be isntalled using pip via the following command
+``` sh pip install pyKrack ``` Then install the R dependencies listed in the
+conda environmnet.yml manually. ## How to use Please see the core and hierarchy
+notebooks for more detailed explanations. **pyKrack** consists of one main
+function, [`compute_hierarchy`](https://FerranC96.github.io/pykrack/
 hierarchy.html#compute_hierarchy). --------------------------------------------
 ---------------------------- source ### compute_hierarchy > compute_hierarchy
 (G, metric='pykrack') Compute one of the possible hierarchy scores | | **Type**
 | **Default** | **Details** | |-------------|-----------|-------------|--------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
```

### Comparing `pykrack-0.0.2/pykrack/_modidx.py` & `pykrack-0.0.3/pykrack/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,8 +2,9 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/pykrack',
                 'doc_host': 'https://FerranC96.github.io',
                 'git_url': 'https://github.com/FerranC96/pykrack',
                 'lib_path': 'pykrack'},
   'syms': { 'pykrack.core': {'pykrack.core.graph_properties': ('core.html#graph_properties', 'pykrack/core.py')},
-            'pykrack.hierarchy': {'pykrack.hierarchy.compute_hierarchy': ('hierarchy.html#compute_hierarchy', 'pykrack/hierarchy.py')}}}
+            'pykrack.hierarchy': {'pykrack.hierarchy.compute_hierarchy': ('hierarchy.html#compute_hierarchy', 'pykrack/hierarchy.py')},
+            'pykrack.utils': {'pykrack.utils.graph_properties': ('core.html#graph_properties', 'pykrack/utils.py')}}}
```

### Comparing `pykrack-0.0.2/pykrack/core.py` & `pykrack-0.0.3/pykrack/core.py`

 * *Files identical despite different names*

### Comparing `pykrack-0.0.2/pykrack/hierarchy.py` & `pykrack-0.0.3/pykrack/hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         'hierarchy_flow' for the Luo and Magee 2011 as implemented in the NetworkX package.
 
     Returns
     -------
     score : float
         One of the possible hierarchy scores
     """
+    
+    import networkx as nx # Be mindful of scoping!
+    from itertools import product
 
     #Ensure Graph is DirectedGraph
     if not G.is_directed():
         raise Exception
     #Ensure Graph is of DiGraph() format
     G = nx.DiGraph(G)
 
@@ -54,14 +57,17 @@
                     symmetric_dyads+=1
         #Raise exception if graph has no edges!
         if non_null_dyads == 0:
             raise Exception
         score = 1 - (symmetric_dyads / non_null_dyads)
     
     elif metric == "rsnakrack": #R implementation from the sna package
+        #Be wary of scoping again!
+        from rpy2.robjects.packages import importr
+
         try:
             base = importr("base")
             sna = importr("sna")
             score = sna.hierarchy(nx.to_numpy_array(G), measure="krackhardt")[0]
         except:
             print("R package sna was not found. Please install manually!")
             print("Computing hierarchy flow instead")
```

### Comparing `pykrack-0.0.2/pykrack.egg-info/PKG-INFO` & `pykrack-0.0.3/pykrack.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pykrack
-Version: 0.0.2
-Summary: Computing Krackhardt hierarchy score on netowrkX graphs
+Version: 0.0.3
+Summary: Computing Krackhardt hierarchy score on NetowrkX graphs
 Home-page: https://github.com/FerranC96/pykrack
 Author: FerranC96
 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,18 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyKrack
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+![CI](https://github.com/FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg)
+[![PyPI
+version](https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack)
+
 ## Install
 
 Due to the comparisons with the R package `sna` we recommend using conda
 to manage your environment.
 
 1.  First create the pykrack conda environment from the environment.yml
     file:
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: pykrack Version: 0.0.2 Summary: Computing
-Krackhardt hierarchy score on netowrkX graphs Home-page: https://github.com/
+Metadata-Version: 2.1 Name: pykrack Version: 0.0.3 Summary: Computing
+Krackhardt hierarchy score on NetowrkX graphs Home-page: https://github.com/
 FerranC96/pykrack Author: FerranC96 Author-email: ferricaro@hotmail.com
 License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE # pyKrack  ## Install Due to the
-comparisons with the R package `sna` we recommend using conda to manage your
-environment. 1. First create the pykrack conda environment from the
-environment.yml file: ``` sh conda (or mamba) env create -f environment.yml ```
-2. Then load the conda environment with: ``` sh conda activate pykrack ``` 3.
-And finally install the package from pip via the following command: ``` sh pip
-install pyKrack ``` Alternatively pyKrack can also be isntalled using pip via
-the following command ``` sh pip install pyKrack ``` Then install the R
-dependencies listed in the conda environmnet.yml manually. ## How to use Please
-see the core and hierarchy notebooks for more detailed explanations.
-**pyKrack** consists of one main function, [`compute_hierarchy`](https://
-FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy). ----------------
--------------------------------------------------------- source ###
-compute_hierarchy > compute_hierarchy (G, metric='pykrack') Compute one of the
-possible hierarchy scores | | **Type** | **Default** | **Details** | |---------
-----|-----------|-------------|------------------------------------------------
+Provides-Extra: dev License-File: LICENSE # pyKrack  ![CI](https://github.com/
+FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg) [![PyPI version]
+(https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack) ##
+Install Due to the comparisons with the R package `sna` we recommend using
+conda to manage your environment. 1. First create the pykrack conda environment
+from the environment.yml file: ``` sh conda (or mamba) env create -
+f environment.yml ``` 2. Then load the conda environment with: ``` sh conda
+activate pykrack ``` 3. And finally install the package from pip via the
+following command: ``` sh pip install pyKrack ``` Alternatively pyKrack can
+also be isntalled using pip via the following command ``` sh pip install
+pyKrack ``` Then install the R dependencies listed in the conda environmnet.yml
+manually. ## How to use Please see the core and hierarchy notebooks for more
+detailed explanations. **pyKrack** consists of one main function,
+[`compute_hierarchy`](https://FerranC96.github.io/pykrack/
+hierarchy.html#compute_hierarchy). --------------------------------------------
+---------------------------- source ### compute_hierarchy > compute_hierarchy
+(G, metric='pykrack') Compute one of the possible hierarchy scores | | **Type**
+| **Default** | **Details** | |-------------|-----------|-------------|--------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------| | G | | | Directed
-NetworkX graph | | metric | str | pykrack | Type of hierarchy metric to
-compute. Accepted types are:
+-------------------------------------------------------------------------------
+-------------------| | G | | | Directed NetworkX graph | | metric | str |
+pykrack | Type of hierarchy metric to compute. Accepted types are:
 âpykrackâ for this moduleâs implementation of the Krackhardt score.
 ârsnakrackâ for the sna implementation in R.
 âhierarchy_flowâ for the Luo and Magee 2011 as implemented in the NetworkX
 package. | | **Returns** | **float** | | **One of the possible hierarchy
 scores** |
```

### Comparing `pykrack-0.0.2/settings.ini` & `pykrack-0.0.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pykrack
 lib_name = pykrack
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pykrack
 nbs_path = nbs
 recursive = True
@@ -17,15 +17,15 @@
 doc_baseurl = /pykrack
 git_url = https://github.com/FerranC96/pykrack
 title = pykrack
 audience = Developers
 author = FerranC96
 author_email = ferricaro@hotmail.com
 copyright = 2023 onwards, FerranC96
-description = Computing Krackhardt hierarchy score on netowrkX graphs
+description = Computing Krackhardt hierarchy score on NetowrkX graphs
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = FerranC96
 requirements = numpy pandas networkx rpy2
 readme_nb = index.ipynb
 allowed_metadata_keys =
```

### Comparing `pykrack-0.0.2/setup.py` & `pykrack-0.0.3/setup.py`

 * *Files identical despite different names*

