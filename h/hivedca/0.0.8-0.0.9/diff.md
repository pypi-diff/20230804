# Comparing `tmp/hivedca-0.0.8.tar.gz` & `tmp/hivedca-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivedca-0.0.8.tar", last modified: Fri Aug  4 00:42:11 2023, max compression
+gzip compressed data, was "hivedca-0.0.9.tar", last modified: Fri Aug  4 01:02:43 2023, max compression
```

## Comparing `hivedca-0.0.8.tar` & `hivedca-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.032305 hivedca-0.0.8/
--rw-rw-rw-   0        0        0      410 2023-08-04 00:42:11.032305 hivedca-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-02 04:45:06.000000 hivedca-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.019347 hivedca-0.0.8/dca/
--rw-rw-rw-   0        0        0      536 2023-08-04 00:41:56.000000 hivedca-0.0.8/dca/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:50.000000 hivedca-0.0.8/dca/backbones.py
--rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:50.000000 hivedca-0.0.8/dca/common.py
--rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:20.000000 hivedca-0.0.8/dca/dataloader.py
--rw-rw-rw-   0        0        0     5519 2023-08-04 00:40:44.000000 hivedca-0.0.8/dca/evaluating.py
--rw-rw-rw-   0        0        0     3429 2023-08-04 00:41:21.000000 hivedca-0.0.8/dca/inferencing.py
--rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:04.000000 hivedca-0.0.8/dca/metrics.py
--rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:36.000000 hivedca-0.0.8/dca/patch_core.py
--rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:06.000000 hivedca-0.0.8/dca/patchcore.py
--rw-rw-rw-   0        0        0     7334 2023-08-04 00:29:54.000000 hivedca-0.0.8/dca/sampler.py
--rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:14.000000 hivedca-0.0.8/dca/training.py
--rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:34.000000 hivedca-0.0.8/dca/training_backup.py
--rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:38.000000 hivedca-0.0.8/dca/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 00:42:11.030301 hivedca-0.0.8/hivedca.egg-info/
--rw-rw-rw-   0        0        0      410 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 00:42:10.000000 hivedca-0.0.8/hivedca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 00:42:11.033296 hivedca-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-08-04 00:41:53.000000 hivedca-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:02:43.749187 hivedca-0.0.9/
+-rw-rw-rw-   0        0        0      410 2023-08-04 01:02:43.748199 hivedca-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-02 04:45:06.000000 hivedca-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 01:02:43.726250 hivedca-0.0.9/dca/
+-rw-rw-rw-   0        0        0      536 2023-08-04 01:02:36.000000 hivedca-0.0.9/dca/__init__.py
+-rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:50.000000 hivedca-0.0.9/dca/backbones.py
+-rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:50.000000 hivedca-0.0.9/dca/common.py
+-rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:20.000000 hivedca-0.0.9/dca/dataloader.py
+-rw-rw-rw-   0        0        0     5519 2023-08-04 01:00:50.000000 hivedca-0.0.9/dca/evaluating.py
+-rw-rw-rw-   0        0        0     3429 2023-08-04 00:41:21.000000 hivedca-0.0.9/dca/inferencing.py
+-rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:04.000000 hivedca-0.0.9/dca/metrics.py
+-rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:36.000000 hivedca-0.0.9/dca/patch_core.py
+-rw-rw-rw-   0        0        0    11767 2023-08-04 00:57:04.000000 hivedca-0.0.9/dca/patchcore.py
+-rw-rw-rw-   0        0        0     7334 2023-08-04 00:29:54.000000 hivedca-0.0.9/dca/sampler.py
+-rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:14.000000 hivedca-0.0.9/dca/training.py
+-rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:34.000000 hivedca-0.0.9/dca/training_backup.py
+-rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:38.000000 hivedca-0.0.9/dca/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:02:43.746194 hivedca-0.0.9/hivedca.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-08-04 01:02:43.000000 hivedca-0.0.9/hivedca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-08-04 01:02:43.000000 hivedca-0.0.9/hivedca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:02:43.000000 hivedca-0.0.9/hivedca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 01:02:43.000000 hivedca-0.0.9/hivedca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:02:43.749187 hivedca-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-04 01:02:33.000000 hivedca-0.0.9/setup.py
```

### Comparing `hivedca-0.0.8/dca/__init__.py` & `hivedca-0.0.9/dca/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2019 (gnyontu39@gmail.com) and contributors
 #
 
 import inspect
 import os
 import sys
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 real_path = os.path.dirname(os.path.abspath(__file__)).replace("\\","/")
 sys.path.append(real_path)
 
 import backbones
 import common
 import dataloader
```

### Comparing `hivedca-0.0.8/dca/backbones.py` & `hivedca-0.0.9/dca/backbones.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/common.py` & `hivedca-0.0.9/dca/common.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/dataloader.py` & `hivedca-0.0.9/dca/dataloader.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/evaluating.py` & `hivedca-0.0.9/dca/evaluating.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,8 +158,8 @@
             if np.sum(masks_gt[i]) > 0:
                 sel_idxs.append(i)
         pixel_scores = metrics.compute_pixelwise_retrieval_metrics(
             [segmentations[i] for i in sel_idxs],
             [masks_gt[i] for i in sel_idxs],
         )
         anomaly_pixel_auroc = pixel_scores["auroc"]
-        print(auroc,full_pixel_auroc,anomaly_pixel_auroc)
+        return auroc,full_pixel_auroc,anomaly_pixel_auroc
```

### Comparing `hivedca-0.0.8/dca/inferencing.py` & `hivedca-0.0.9/dca/inferencing.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/metrics.py` & `hivedca-0.0.9/dca/metrics.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/patch_core.py` & `hivedca-0.0.9/dca/patch_core.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/patchcore.py` & `hivedca-0.0.9/dca/patchcore.py`

 * *Files 6% similar despite different names*

```diff
@@ -182,24 +182,24 @@
         """This function provides anomaly scores/maps for full dataloaders."""
         _ = self.forward_modules.eval()
 
         scores = []
         masks = []
         labels_gt = []
         masks_gt = []
-        with tqdm.tqdm(dataloader, desc="Inferring...", leave=False) as data_iterator:
-            for image in data_iterator:
-                if isinstance(image, dict):
-                    labels_gt.extend(image["is_anomaly"].numpy().tolist())
-                    masks_gt.extend(image["mask"].numpy().tolist())
-                    image = image["image"]
-                _scores, _masks = self._predict(image)
-                for score, mask in zip(_scores, _masks):
-                    scores.append(score)
-                    masks.append(mask)
+        for dataloader_idx,image in enumerate(dataloader):
+            print("BRAIN - Infer : " + str(dataloader_idx) + " / " + str(len(dataloader)))
+            if isinstance(image, dict):
+                labels_gt.extend(image["is_anomaly"].numpy().tolist())
+                masks_gt.extend(image["mask"].numpy().tolist())
+                image = image["image"]
+            _scores, _masks = self._predict(image)
+            for score, mask in zip(_scores, _masks):
+                scores.append(score)
+                masks.append(mask)
         return scores, masks, labels_gt, masks_gt
 
     def _predict(self, images):
         """Infer score and mask for a batch of images."""
         images = images.to(torch.float).to(self.device)
         _ = self.forward_modules.eval()
```

### Comparing `hivedca-0.0.8/dca/sampler.py` & `hivedca-0.0.9/dca/sampler.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/training.py` & `hivedca-0.0.9/dca/training.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/training_backup.py` & `hivedca-0.0.9/dca/training_backup.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/dca/utils.py` & `hivedca-0.0.9/dca/utils.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.8/setup.py` & `hivedca-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hivedca", # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

