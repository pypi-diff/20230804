# Comparing `tmp/hivedca-0.0.7.tar.gz` & `tmp/hivedca-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivedca-0.0.7.tar", last modified: Fri Aug  4 00:38:32 2023, max compression
+gzip compressed data, was "hivedca-0.0.8.tar", last modified: Fri Aug  4 00:42:11 2023, max compression
```

## Comparing `hivedca-0.0.7.tar` & `hivedca-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 00:38:32.424238 hivedca-0.0.7/
--rw-rw-rw-   0        0        0      410 2023-08-04 00:38:32.423238 hivedca-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-02 04:45:06.000000 hivedca-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 00:38:32.408293 hivedca-0.0.7/dca/
--rw-rw-rw-   0        0        0      536 2023-08-04 00:38:13.000000 hivedca-0.0.7/dca/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:50.000000 hivedca-0.0.7/dca/backbones.py
--rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:50.000000 hivedca-0.0.7/dca/common.py
--rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:20.000000 hivedca-0.0.7/dca/dataloader.py
--rw-rw-rw-   0        0        0     5614 2023-07-28 06:50:48.000000 hivedca-0.0.7/dca/evaluating.py
--rw-rw-rw-   0        0        0     3535 2023-07-28 08:00:17.000000 hivedca-0.0.7/dca/inferencing.py
--rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:04.000000 hivedca-0.0.7/dca/metrics.py
--rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:36.000000 hivedca-0.0.7/dca/patch_core.py
--rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:06.000000 hivedca-0.0.7/dca/patchcore.py
--rw-rw-rw-   0        0        0     7334 2023-08-04 00:29:54.000000 hivedca-0.0.7/dca/sampler.py
--rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:14.000000 hivedca-0.0.7/dca/training.py
--rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:34.000000 hivedca-0.0.7/dca/training_backup.py
--rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:38.000000 hivedca-0.0.7/dca/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 00:38:32.421781 hivedca-0.0.7/hivedca.egg-info/
--rw-rw-rw-   0        0        0      410 2023-08-04 00:38:32.000000 hivedca-0.0.7/hivedca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-08-04 00:38:32.000000 hivedca-0.0.7/hivedca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 00:38:32.000000 hivedca-0.0.7/hivedca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 00:38:32.000000 hivedca-0.0.7/hivedca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 00:38:32.425240 hivedca-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-08-04 00:38:17.000000 hivedca-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.032305 hivedca-0.0.8/
+-rw-rw-rw-   0        0        0      410 2023-08-04 00:42:11.032305 hivedca-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-02 04:45:06.000000 hivedca-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.019347 hivedca-0.0.8/dca/
+-rw-rw-rw-   0        0        0      536 2023-08-04 00:41:56.000000 hivedca-0.0.8/dca/__init__.py
+-rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:50.000000 hivedca-0.0.8/dca/backbones.py
+-rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:50.000000 hivedca-0.0.8/dca/common.py
+-rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:20.000000 hivedca-0.0.8/dca/dataloader.py
+-rw-rw-rw-   0        0        0     5519 2023-08-04 00:40:44.000000 hivedca-0.0.8/dca/evaluating.py
+-rw-rw-rw-   0        0        0     3429 2023-08-04 00:41:21.000000 hivedca-0.0.8/dca/inferencing.py
+-rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:04.000000 hivedca-0.0.8/dca/metrics.py
+-rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:36.000000 hivedca-0.0.8/dca/patch_core.py
+-rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:06.000000 hivedca-0.0.8/dca/patchcore.py
+-rw-rw-rw-   0        0        0     7334 2023-08-04 00:29:54.000000 hivedca-0.0.8/dca/sampler.py
+-rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:14.000000 hivedca-0.0.8/dca/training.py
+-rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:34.000000 hivedca-0.0.8/dca/training_backup.py
+-rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:38.000000 hivedca-0.0.8/dca/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.030301 hivedca-0.0.8/hivedca.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 00:42:11.033296 hivedca-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-04 00:41:53.000000 hivedca-0.0.8/setup.py
```

### Comparing `hivedca-0.0.7/dca/__init__.py` & `hivedca-0.0.8/dca/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2019 (gnyontu39@gmail.com) and contributors
 #
 
 import inspect
 import os
 import sys
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 real_path = os.path.dirname(os.path.abspath(__file__)).replace("\\","/")
 sys.path.append(real_path)
 
 import backbones
 import common
 import dataloader
```

### Comparing `hivedca-0.0.7/dca/backbones.py` & `hivedca-0.0.8/dca/backbones.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/common.py` & `hivedca-0.0.8/dca/common.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/dataloader.py` & `hivedca-0.0.8/dca/dataloader.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/evaluating.py` & `hivedca-0.0.8/dca/evaluating.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,37 @@
 import os
 
 import metrics
 from dataloader import get_dataloaders, get_test_dataloaders
 from utils import fix_seeds, plot_segmentation_images, set_torch_device
 import sys
 
-sys.path.append("./src")
-import patchcore.backbones
-import patchcore.common
-import patchcore.patchcore
+import backbones
+import common
+import patchcore
 
 
 def load_patchcore(patch_core_path):
     device = set_torch_device([0])
     n_patchcores = len(
         [x for x in os.listdir(patch_core_path) if ".faiss" in x]
     )
     if n_patchcores == 1:
-        nn_method = patchcore.common.FaissNN(False, 8)
-        patchcore_instance = patchcore.patchcore.PatchCore(device)
+        nn_method = common.FaissNN(False, 8)
+        patchcore_instance = patchcore.PatchCore(device)
         patchcore_instance.load_from_path(
             load_path=patch_core_path, device=device, nn_method=nn_method
         )
         return patchcore_instance
     else:
         for i in range(n_patchcores):
-            nn_method = patchcore.common.FaissNN(
+            nn_method = common.FaissNN(
                 False, 8
             )
-            patchcore_instance = patchcore.patchcore.PatchCore(device)
+            patchcore_instance = patchcore.PatchCore(device)
             patchcore_instance.load_from_path(
                 load_path=patch_core_path,
                 device=device,
                 nn_method=nn_method,
                 prepend="Ensemble-{}-{}_".format(i + 1, n_patchcores),
             )
             return patchcore_instance
```

### Comparing `hivedca-0.0.7/dca/inferencing.py` & `hivedca-0.0.8/dca/inferencing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import torch
 import numpy as np
 import os
 
 from utils import fix_seeds, set_torch_device
-import sys
 import PIL
 
-sys.path.append("./src")
-import patchcore.backbones
-import patchcore.common
-import patchcore.patchcore
+import backbones
+import common
+import patchcore
 from torchvision import transforms
 
 
 def load_patchcore(patch_core_path):
     device = set_torch_device([0])
     n_patchcores = len(
         [x for x in os.listdir(patch_core_path) if ".faiss" in x]
     )
     if n_patchcores == 1:
-        nn_method = patchcore.common.FaissNN(False, 8)
-        patchcore_instance = patchcore.patchcore.PatchCore(device)
+        nn_method = common.FaissNN(False, 8)
+        patchcore_instance = patchcore.PatchCore(device)
         patchcore_instance.load_from_path(
             load_path=patch_core_path, device=device, nn_method=nn_method
         )
         return patchcore_instance
     else:
         for i in range(n_patchcores):
-            nn_method = patchcore.common.FaissNN(
+            nn_method = common.FaissNN(
                 False, 8
             )
-            patchcore_instance = patchcore.patchcore.PatchCore(device)
+            patchcore_instance = patchcore.PatchCore(device)
             patchcore_instance.load_from_path(
                 load_path=patch_core_path,
                 device=device,
                 nn_method=nn_method,
                 prepend="Ensemble-{}-{}_".format(i + 1, n_patchcores),
             )
             return patchcore_instance
```

### Comparing `hivedca-0.0.7/dca/metrics.py` & `hivedca-0.0.8/dca/metrics.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/patch_core.py` & `hivedca-0.0.8/dca/patch_core.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/patchcore.py` & `hivedca-0.0.8/dca/patchcore.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/sampler.py` & `hivedca-0.0.8/dca/sampler.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/training.py` & `hivedca-0.0.8/dca/training.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/training_backup.py` & `hivedca-0.0.8/dca/training_backup.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/dca/utils.py` & `hivedca-0.0.8/dca/utils.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.7/setup.py` & `hivedca-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hivedca", # Replace with your own username
-    version="0.0.7",
+    version="0.0.8",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

