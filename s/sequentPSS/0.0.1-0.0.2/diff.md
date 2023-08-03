# Comparing `tmp/sequentPSS-0.0.1.tar.gz` & `tmp/sequentPSS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentPSS-0.0.1.tar", last modified: Thu Aug  3 03:20:35 2023, max compression
+gzip compressed data, was "sequentPSS-0.0.2.tar", last modified: Thu Aug  3 03:30:26 2023, max compression
```

## Comparing `sequentPSS-0.0.1.tar` & `sequentPSS-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 03:20:35.293643 sequentPSS-0.0.1/
--rw-rw-rw-   0        0        0       48 2023-08-03 03:00:45.000000 sequentPSS-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-08-03 03:20:35.292645 sequentPSS-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 03:20:35.244773 sequentPSS-0.0.1/sequentPSS/
--rw-rw-rw-   0        0        0       27 2023-08-03 03:17:13.000000 sequentPSS-0.0.1/sequentPSS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:20:35.286661 sequentPSS-0.0.1/sequentPSS/sampleData/
--rw-rw-rw-   0        0        0   936536 2023-08-02 23:11:54.000000 sequentPSS-0.0.1/sequentPSS/sampleData/concatenated_df.csv
--rw-rw-rw-   0        0        0     1872 2023-08-03 02:58:33.000000 sequentPSS-0.0.1/sequentPSS/sequentPSS.py
-drwxrwxrwx   0        0        0        0 2023-08-03 03:20:35.282672 sequentPSS-0.0.1/sequentPSS.egg-info/
--rw-rw-rw-   0        0        0      274 2023-08-03 03:20:34.000000 sequentPSS-0.0.1/sequentPSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-08-03 03:20:35.000000 sequentPSS-0.0.1/sequentPSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 03:20:34.000000 sequentPSS-0.0.1/sequentPSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 03:20:34.000000 sequentPSS-0.0.1/sequentPSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 03:20:34.000000 sequentPSS-0.0.1/sequentPSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 03:20:35.294640 sequentPSS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1254 2023-08-03 03:18:25.000000 sequentPSS-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:30:26.380896 sequentPSS-0.0.2/
+-rw-rw-rw-   0        0        0       48 2023-08-03 03:00:45.000000 sequentPSS-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-08-03 03:30:26.379898 sequentPSS-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:30:26.345988 sequentPSS-0.0.2/sequentPSS/
+-rw-rw-rw-   0        0        0       27 2023-08-03 03:17:13.000000 sequentPSS-0.0.2/sequentPSS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:30:26.372915 sequentPSS-0.0.2/sequentPSS/sampleData/
+-rw-rw-rw-   0        0        0   936536 2023-08-02 23:11:54.000000 sequentPSS-0.0.2/sequentPSS/sampleData/concatenated_df.csv
+-rw-rw-rw-   0        0        0     2133 2023-08-03 03:29:38.000000 sequentPSS-0.0.2/sequentPSS/sequentPSS.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:30:26.370920 sequentPSS-0.0.2/sequentPSS.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-08-03 03:30:25.000000 sequentPSS-0.0.2/sequentPSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-08-03 03:30:26.000000 sequentPSS-0.0.2/sequentPSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:30:25.000000 sequentPSS-0.0.2/sequentPSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 03:30:25.000000 sequentPSS-0.0.2/sequentPSS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 03:30:26.000000 sequentPSS-0.0.2/sequentPSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:30:26.381891 sequentPSS-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2023-08-03 03:30:06.000000 sequentPSS-0.0.2/setup.py
```

### Comparing `sequentPSS-0.0.1/sequentPSS/sampleData/concatenated_df.csv` & `sequentPSS-0.0.2/sequentPSS/sampleData/concatenated_df.csv`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.1/sequentPSS/sequentPSS.py` & `sequentPSS-0.0.2/sequentPSS/sequentPSS.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
+# In[7]:
 
 
 import numpy as np
 import pandas as pd
 import random2
+import os #os의 경우 기본적으로 주어지기 때문에 setup.py에 하지 않는다.
 
 
 # ## data
 
-# In[6]:
+# In[8]:
 
 
+# change path to relative path - only for publishing
+current_directory = os.path.dirname(os.path.abspath(__file__))
+os.chdir(current_directory)
+
 path = "./sampleData/concatenated_df.csv"
 simul_data = pd.read_csv(path)
 
 
 # ## simulation code
 
 # In[3]:
@@ -49,14 +54,15 @@
    
     # select data
     condition = (simul_data['p1'] == p1) & (simul_data['p2'] == p2) & (simul_data['p3'] == p3)
     filtered_df = simul_data[condition]
     
     dfs = []
     for i in range(n): # now, extracts by #n
+        
         uniq_num = random2.choice(pd.unique(filtered_df['uniq_num']))
         chosen_df = filtered_df[filtered_df['uniq_num'] == uniq_num] #filter only uniq_num
     
         # now make new simulation data
         new_data = {
             'p1': [chosen_df['p1'].iloc[0]],
             'p2': [chosen_df['p2'].iloc[0]],
@@ -73,19 +79,25 @@
     result_df = pd.concat(dfs, axis=0, ignore_index=True) 
     
     return result_df
 
 
 # ## 1) preprocessing (1)
 
-# In[1]:
+# In[4]:
 
 
 def criterion(asd):
     print(asd + "asdasdasdccqc")
 
 
 # In[ ]:
 
 
 
 
+
+# In[ ]:
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sequentPSS-0.0.1/setup.py` & `sequentPSS-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sequentPSS',
-    version = '0.0.1',
+    version = '0.0.2',
     description = "algorithm for sequential parameter searching with GSA",
     url = 'https://github.com/MG-Choi/sequentPSS',
     author = 'MoongiChoi',
     author_email = 'u1316663@utah.edu',
     packages = find_packages(),
     package_data = {'sequentPSS': ['sampleData/concatenated_df.csv']},
     include_package_data = True,
```

