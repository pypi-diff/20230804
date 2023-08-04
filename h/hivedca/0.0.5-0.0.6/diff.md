# Comparing `tmp/hivedca-0.0.5.tar.gz` & `tmp/hivedca-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivedca-0.0.5.tar", last modified: Wed Aug  2 05:13:33 2023, max compression
+gzip compressed data, was "hivedca-0.0.6.tar", last modified: Fri Aug  4 00:34:12 2023, max compression
```

## Comparing `hivedca-0.0.5.tar` & `hivedca-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 05:13:33.467490 hivedca-0.0.5/
--rw-rw-rw-   0        0        0      410 2023-08-02 05:13:33.466427 hivedca-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-02 04:45:04.000000 hivedca-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 05:13:33.439479 hivedca-0.0.5/dca/
--rw-rw-rw-   0        0        0      647 2023-08-02 05:13:30.000000 hivedca-0.0.5/dca/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:49.000000 hivedca-0.0.5/dca/backbones.py
--rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:49.000000 hivedca-0.0.5/dca/common.py
--rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:18.000000 hivedca-0.0.5/dca/dataloader.py
--rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:02.000000 hivedca-0.0.5/dca/metrics.py
--rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:34.000000 hivedca-0.0.5/dca/patch_core.py
--rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:04.000000 hivedca-0.0.5/dca/patchcore.py
--rw-rw-rw-   0        0        0     7326 2023-07-28 00:59:22.000000 hivedca-0.0.5/dca/sampler.py
--rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:12.000000 hivedca-0.0.5/dca/training.py
--rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:32.000000 hivedca-0.0.5/dca/training_backup.py
--rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:37.000000 hivedca-0.0.5/dca/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:13:33.463340 hivedca-0.0.5/hivedca.egg-info/
--rw-rw-rw-   0        0        0      410 2023-08-02 05:13:33.000000 hivedca-0.0.5/hivedca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-08-02 05:13:33.000000 hivedca-0.0.5/hivedca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 05:13:33.000000 hivedca-0.0.5/hivedca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 05:13:33.000000 hivedca-0.0.5/hivedca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 05:13:33.468449 hivedca-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-08-02 05:13:26.000000 hivedca-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:34:12.643135 hivedca-0.0.6/
+-rw-rw-rw-   0        0        0      410 2023-08-04 00:34:12.641133 hivedca-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-02 04:45:06.000000 hivedca-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 00:34:12.619969 hivedca-0.0.6/dca/
+-rw-rw-rw-   0        0        0      499 2023-08-04 00:32:32.000000 hivedca-0.0.6/dca/__init__.py
+-rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:50.000000 hivedca-0.0.6/dca/backbones.py
+-rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:50.000000 hivedca-0.0.6/dca/common.py
+-rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:20.000000 hivedca-0.0.6/dca/dataloader.py
+-rw-rw-rw-   0        0        0     5614 2023-07-28 06:50:48.000000 hivedca-0.0.6/dca/evaluating.py
+-rw-rw-rw-   0        0        0     3535 2023-07-28 08:00:17.000000 hivedca-0.0.6/dca/inferencing.py
+-rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:04.000000 hivedca-0.0.6/dca/metrics.py
+-rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:36.000000 hivedca-0.0.6/dca/patch_core.py
+-rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:06.000000 hivedca-0.0.6/dca/patchcore.py
+-rw-rw-rw-   0        0        0     7334 2023-08-04 00:29:54.000000 hivedca-0.0.6/dca/sampler.py
+-rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:14.000000 hivedca-0.0.6/dca/training.py
+-rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:34.000000 hivedca-0.0.6/dca/training_backup.py
+-rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:38.000000 hivedca-0.0.6/dca/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:34:12.640132 hivedca-0.0.6/hivedca.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-08-04 00:34:12.000000 hivedca-0.0.6/hivedca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-08-04 00:34:12.000000 hivedca-0.0.6/hivedca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 00:34:12.000000 hivedca-0.0.6/hivedca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 00:34:12.000000 hivedca-0.0.6/hivedca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 00:34:12.643135 hivedca-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-04 00:32:28.000000 hivedca-0.0.6/setup.py
```

### Comparing `hivedca-0.0.5/dca/backbones.py` & `hivedca-0.0.6/dca/backbones.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/common.py` & `hivedca-0.0.6/dca/common.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/dataloader.py` & `hivedca-0.0.6/dca/dataloader.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/metrics.py` & `hivedca-0.0.6/dca/metrics.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/patch_core.py` & `hivedca-0.0.6/dca/patch_core.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/patchcore.py` & `hivedca-0.0.6/dca/patchcore.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/sampler.py` & `hivedca-0.0.6/dca/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             approximate_distance_matrix, axis=-1
         ).reshape(-1, 1)
         coreset_indices = []
         num_coreset_samples = int(len(features) * self.percentage)
 
         with torch.no_grad():
             for idx in range(num_coreset_samples):
-                print("Subsampling : " + str(idx) +" / "+str(num_coreset_samples))
+                print("BRAIN - Subsampling : " + str(idx) +" / "+str(num_coreset_samples))
                 select_idx = torch.argmax(approximate_coreset_anchor_distances).item()
                 coreset_indices.append(select_idx)
                 coreset_select_distance = self._compute_batchwise_differences(
                     features, features[select_idx : select_idx + 1]  # noqa: E203
                 )
                 approximate_coreset_anchor_distances = torch.cat(
                     [approximate_coreset_anchor_distances, coreset_select_distance],
```

### Comparing `hivedca-0.0.5/dca/training.py` & `hivedca-0.0.6/dca/training.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/training_backup.py` & `hivedca-0.0.6/dca/training_backup.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/dca/utils.py` & `hivedca-0.0.6/dca/utils.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.5/setup.py` & `hivedca-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hivedca", # Replace with your own username
-    version="0.0.5",
+    version="0.0.6",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

