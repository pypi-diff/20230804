# Comparing `tmp/evodiff-0.0.5.tar.gz` & `tmp/evodiff-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodiff-0.0.5.tar", last modified: Fri Aug  4 17:20:10 2023, max compression
+gzip compressed data, was "evodiff-0.0.6.tar", last modified: Fri Aug  4 17:25:11 2023, max compression
```

## Comparing `evodiff-0.0.5.tar` & `evodiff-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.232364 evodiff-0.0.5/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.5/LICENSE
--rw-r--r--   0 nityathakkar   (501) staff       (20)       16 2023-08-04 17:18:36.000000 evodiff-0.0.5/MANIFEST.in
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:20:10.231554 evodiff-0.0.5/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.5/README.md
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.158344 evodiff-0.0.5/config/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/config38M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/config640M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/configMSA-600M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/configMSA.json
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.165626 evodiff-0.0.5/evodiff/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/__init__.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.5/evodiff/collaters.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/constants.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/data.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/losses.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/metrics.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/model.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/plot.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    11829 2023-08-04 17:19:48.000000 evodiff-0.0.5/evodiff/pretrained.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.5/evodiff/utils.py
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.231102 evodiff-0.0.5/evodiff.egg-info/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-04 17:20:10.000000 evodiff-0.0.5/evodiff.egg-info/SOURCES.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/dependency_links.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/top_level.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-04 17:18:33.000000 evodiff-0.0.5/pyproject.toml
--rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-04 17:20:10.232517 evodiff-0.0.5/setup.cfg
--rw-r--r--   0 nityathakkar   (501) staff       (20)      799 2023-08-04 17:18:38.000000 evodiff-0.0.5/setup.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:25:11.828262 evodiff-0.0.6/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.6/LICENSE
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       16 2023-08-04 17:18:36.000000 evodiff-0.0.6/MANIFEST.in
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:25:11.827970 evodiff-0.0.6/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.6/README.md
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:25:11.795805 evodiff-0.0.6/config/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.6/config/config38M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.6/config/config640M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.6/config/configMSA-600M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.6/config/configMSA.json
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:25:11.802405 evodiff-0.0.6/evodiff/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/__init__.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.6/evodiff/collaters.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/constants.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/data.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/losses.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/metrics.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/model.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.6/evodiff/plot.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    11990 2023-08-04 17:24:45.000000 evodiff-0.0.6/evodiff/pretrained.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.6/evodiff/utils.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:25:11.827404 evodiff-0.0.6/evodiff.egg-info/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:25:11.000000 evodiff-0.0.6/evodiff.egg-info/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-04 17:25:11.000000 evodiff-0.0.6/evodiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-04 17:25:11.000000 evodiff-0.0.6/evodiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-04 17:25:11.000000 evodiff-0.0.6/evodiff.egg-info/top_level.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-04 17:24:40.000000 evodiff-0.0.6/pyproject.toml
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-04 17:25:11.828347 evodiff-0.0.6/setup.cfg
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      794 2023-08-04 17:24:43.000000 evodiff-0.0.6/setup.py
```

### Comparing `evodiff-0.0.5/LICENSE` & `evodiff-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/PKG-INFO` & `evodiff-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
```

### Comparing `evodiff-0.0.5/README.md` & `evodiff-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/collaters.py` & `evodiff-0.0.6/evodiff/collaters.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/data.py` & `evodiff-0.0.6/evodiff/data.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/losses.py` & `evodiff-0.0.6/evodiff/losses.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/metrics.py` & `evodiff-0.0.6/evodiff/metrics.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/model.py` & `evodiff-0.0.6/evodiff/model.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/plot.py` & `evodiff-0.0.6/evodiff/plot.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff/pretrained.py` & `evodiff-0.0.6/evodiff/pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+import pkg_resources
 import json
 from evodiff.model import ByteNetLMTime, MSATransformerTime
 from sequence_models.esm import MSATransformer
 from sequence_models.constants import MSA_ALPHABET, PROTEIN_ALPHABET, ALL_AAS, PAD, MSA_PAD, MASK
 from sequence_models.collaters import LMCollater
 from evodiff.utils import Tokenizer, download_model
 from evodiff.collaters import D3PMCollater, OAMaskCollater, ESMOAMaskCollater, D3PMCollaterMSA, ESMOAMaskCollaterMSA
@@ -84,15 +85,16 @@
         return model, collater, tokenizer, scheme
 
 def D3PM_BLOSUM_38M(return_all=False):
     dt=500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
     Q_prod, Q_t = tokenizer.q_blosum_schedule(timesteps=dt)
     collater = D3PMCollater(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-38M", "config/config38M.json",
+    file_path = pkg_resources.resource_filename('evodiff', 'config/config38M.json')
+    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-38M", file_path,
                                                       diffusion_timesteps=dt,
                                                       tokenizer=tokenizer)
     scheme = 'd3pm'
     if return_all:
         return model, collater, tokenizer, scheme, dt, Q_prod, Q_t
     else:
         return model, collater, tokenizer, scheme
@@ -133,15 +135,16 @@
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 
 def OA_AR_38M():
     tokenizer = Tokenizer()
     collater = OAMaskCollater(tokenizer=tokenizer)
-    model, tokenizer = load_sequence_checkpoint("oaar-38M", "config/config38M.json", diffusion_timesteps=None, \
+    file_path = pkg_resources.resource_filename('evodiff', 'config/config38M.json')
+    model, tokenizer = load_sequence_checkpoint("oaar-38M", file_path, diffusion_timesteps=None, \
                          tokenizer=tokenizer)
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 
 def LR_AR_640M():
     n_tokens = len(PROTEIN_ALPHABET)
```

### Comparing `evodiff-0.0.5/evodiff/utils.py` & `evodiff-0.0.6/evodiff/utils.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.5/evodiff.egg-info/PKG-INFO` & `evodiff-0.0.6/evodiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
```

### Comparing `evodiff-0.0.5/setup.py` & `evodiff-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="evodiff", # Replace with your own username
-    version="0.0.5",
+    version="0.0.6",
     description="Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/evodiff",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8.5',
     # include_package_data=True,
     # package_dir = {"": "config"},
     packages=setuptools.find_packages(),
-    package_data={'': ['config/*.json']},
+    package_data={'': ['config/*']},
 )
```

