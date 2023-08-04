# Comparing `tmp/taron-1.0.tar.gz` & `tmp/taron-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taron-1.0.tar", last modified: Fri Aug  4 18:30:36 2023, max compression
+gzip compressed data, was "taron-1.1.tar", last modified: Fri Aug  4 18:35:50 2023, max compression
```

## Comparing `taron-1.0.tar` & `taron-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 18:30:36.684610 taron-1.0/
--rw-rw-rw-   0        0        0      183 2023-08-04 18:30:36.684610 taron-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 18:30:36.684610 taron-1.0/setup.cfg
--rw-rw-rw-   0        0        0      231 2023-08-04 18:29:33.000000 taron-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 18:30:36.678587 taron-1.0/taron/
--rw-rw-rw-   0        0        0      195 2023-08-04 18:29:04.000000 taron-1.0/taron/__init__.py
--rw-rw-rw-   0        0        0       57 2023-08-04 18:07:55.000000 taron-1.0/taron/add_num.py
--rw-rw-rw-   0        0        0      516 2023-07-26 06:42:22.000000 taron-1.0/taron/mydata.py
--rw-rw-rw-   0        0        0     2565 2023-07-26 06:42:23.000000 taron-1.0/taron/network.py
--rw-rw-rw-   0        0        0     2375 2023-07-26 06:42:21.000000 taron-1.0/taron/neurons_better.py
--rw-rw-rw-   0        0        0     6034 2023-07-26 06:42:25.000000 taron-1.0/taron/regressor.py
--rw-rw-rw-   0        0        0      391 2023-07-26 06:42:24.000000 taron-1.0/taron/seeds.py
--rw-rw-rw-   0        0        0     2767 2023-07-23 14:58:56.000000 taron-1.0/taron/synthesis.py
-drwxrwxrwx   0        0        0        0 2023-08-04 18:30:36.683610 taron-1.0/taron.egg-info/
--rw-rw-rw-   0        0        0      183 2023-08-04 18:30:36.000000 taron-1.0/taron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-08-04 18:30:36.000000 taron-1.0/taron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 18:30:36.000000 taron-1.0/taron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 18:30:36.000000 taron-1.0/taron.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 18:35:50.265701 taron-1.1/
+-rw-rw-rw-   0        0        0      183 2023-08-04 18:35:50.265701 taron-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 18:35:50.265701 taron-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-08-04 18:35:27.000000 taron-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:35:50.260210 taron-1.1/taron/
+-rw-rw-rw-   0        0        0      195 2023-08-04 18:29:04.000000 taron-1.1/taron/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-08-04 18:07:55.000000 taron-1.1/taron/add_num.py
+-rw-rw-rw-   0        0        0      516 2023-07-26 06:42:22.000000 taron-1.1/taron/mydata.py
+-rw-rw-rw-   0        0        0     2566 2023-08-04 18:34:46.000000 taron-1.1/taron/network.py
+-rw-rw-rw-   0        0        0     2375 2023-07-26 06:42:21.000000 taron-1.1/taron/neurons_better.py
+-rw-rw-rw-   0        0        0     6034 2023-07-26 06:42:25.000000 taron-1.1/taron/regressor.py
+-rw-rw-rw-   0        0        0      391 2023-07-26 06:42:24.000000 taron-1.1/taron/seeds.py
+-rw-rw-rw-   0        0        0     2767 2023-07-23 14:58:56.000000 taron-1.1/taron/synthesis.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:35:50.264527 taron-1.1/taron.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-08-04 18:35:50.000000 taron-1.1/taron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-08-04 18:35:50.000000 taron-1.1/taron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 18:35:50.000000 taron-1.1/taron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 18:35:50.000000 taron-1.1/taron.egg-info/top_level.txt
```

### Comparing `taron-1.0/taron/mydata.py` & `taron-1.1/taron/mydata.py`

 * *Files identical despite different names*

### Comparing `taron-1.0/taron/network.py` & `taron-1.1/taron/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import torch
 from sklearn.model_selection import train_test_split
 from torch import nn
 from torch.utils.data import Dataset
-from neurons_better import Neurons
+from .neurons_better import Neurons
 from seeds import random_seed
 from mydata import MyData
 import h5py
 
 
 def main(group, sr, seed):
     test_size = 0.2
```

### Comparing `taron-1.0/taron/neurons_better.py` & `taron-1.1/taron/neurons_better.py`

 * *Files identical despite different names*

### Comparing `taron-1.0/taron/regressor.py` & `taron-1.1/taron/regressor.py`

 * *Files identical despite different names*

### Comparing `taron-1.0/taron/synthesis.py` & `taron-1.1/taron/synthesis.py`

 * *Files identical despite different names*

