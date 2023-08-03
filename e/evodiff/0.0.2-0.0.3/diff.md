# Comparing `tmp/evodiff-0.0.2.tar.gz` & `tmp/evodiff-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodiff-0.0.2.tar", last modified: Thu Aug  3 01:39:12 2023, max compression
+gzip compressed data, was "evodiff-0.0.3.tar", last modified: Thu Aug  3 23:34:13 2023, max compression
```

## Comparing `evodiff-0.0.2.tar` & `evodiff-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.627252 evodiff-0.0.2/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.2/LICENSE
--rw-r--r--   0 nityathakkar   (501) staff       (20)       22 2023-08-03 01:37:06.000000 evodiff-0.0.2/MANIFEST.in
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6885 2023-08-03 01:39:12.626569 evodiff-0.0.2/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6433 2023-08-03 01:27:58.000000 evodiff-0.0.2/README.md
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.567304 evodiff-0.0.2/config/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/config38M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/config640M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/configMSA-600M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.2/config/configMSA.json
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.579373 evodiff-0.0.2/evodiff/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/__init__.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/collaters.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/constants.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/data.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/losses.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/metrics.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/model.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.2/evodiff/plot.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    11836 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/pretrained.py
--rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.2/evodiff/utils.py
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 01:39:12.625509 evodiff-0.0.2/evodiff.egg-info/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6885 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/SOURCES.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/dependency_links.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-03 01:39:12.000000 evodiff-0.0.2/evodiff.egg-info/top_level.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-03 01:38:51.000000 evodiff-0.0.2/pyproject.toml
--rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-03 01:39:12.627491 evodiff-0.0.2/setup.cfg
--rw-r--r--   0 nityathakkar   (501) staff       (20)      733 2023-08-03 01:38:22.000000 evodiff-0.0.2/setup.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:34:13.262829 evodiff-0.0.3/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.3/LICENSE
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       27 2023-08-03 23:30:36.000000 evodiff-0.0.3/MANIFEST.in
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6883 2023-08-03 23:34:13.262380 evodiff-0.0.3/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.3/README.md
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:34:13.081614 evodiff-0.0.3/evodiff/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/__init__.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.3/evodiff/collaters.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/constants.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/data.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/losses.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/metrics.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/model.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.3/evodiff/plot.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    11957 2023-08-03 23:23:05.000000 evodiff-0.0.3/evodiff/pretrained.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.3/evodiff/utils.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:34:13.261711 evodiff-0.0.3/evodiff.egg-info/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6883 2023-08-03 23:34:12.000000 evodiff-0.0.3/evodiff.egg-info/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      364 2023-08-03 23:34:12.000000 evodiff-0.0.3/evodiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-03 23:34:12.000000 evodiff-0.0.3/evodiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-03 23:34:12.000000 evodiff-0.0.3/evodiff.egg-info/top_level.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-03 23:23:14.000000 evodiff-0.0.3/pyproject.toml
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-03 23:34:13.262974 evodiff-0.0.3/setup.cfg
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      764 2023-08-03 23:28:57.000000 evodiff-0.0.3/setup.py
```

### Comparing `evodiff-0.0.2/LICENSE` & `evodiff-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/PKG-INFO` & `evodiff-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
@@ -32,17 +32,17 @@
 You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
 
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
-from evodiff.pretrained import OA_AR_640M
+from evodiff.pretrained import OA_AR_38M
 
-model, collater, tokenizer, scheme = OA_AR_640M()
+model, collater, tokenizer, scheme = OA_AR_38M()
 ```
 Available models are:
 * ``` D3PM_BLOSUM_640M() ```
 * ``` D3PM_BLOSUM_38M() ```
 * ``` D3PM_UNIFORM_640M() ```
 * ``` D3PM_UNIFORM_38M() ```
 * ``` OA_AR_640M() ```
```

### Comparing `evodiff-0.0.2/README.md` & `evodiff-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
 
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
-from evodiff.pretrained import OA_AR_640M
+from evodiff.pretrained import OA_AR_38M
 
-model, collater, tokenizer, scheme = OA_AR_640M()
+model, collater, tokenizer, scheme = OA_AR_38M()
 ```
 Available models are:
 * ``` D3PM_BLOSUM_640M() ```
 * ``` D3PM_BLOSUM_38M() ```
 * ``` D3PM_UNIFORM_640M() ```
 * ``` D3PM_UNIFORM_38M() ```
 * ``` OA_AR_640M() ```
```

### Comparing `evodiff-0.0.2/evodiff/collaters.py` & `evodiff-0.0.3/evodiff/collaters.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/data.py` & `evodiff-0.0.3/evodiff/data.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/losses.py` & `evodiff-0.0.3/evodiff/losses.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/metrics.py` & `evodiff-0.0.3/evodiff/metrics.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/model.py` & `evodiff-0.0.3/evodiff/model.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/plot.py` & `evodiff-0.0.3/evodiff/plot.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff/pretrained.py` & `evodiff-0.0.3/evodiff/pretrained.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,116 +70,116 @@
     return model, tokenizer
 
 def D3PM_BLOSUM_640M(return_all=False):
     dt=500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
     Q_prod, Q_t = tokenizer.q_blosum_schedule(timesteps=dt)
     collater = D3PMCollater(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-640M", "config/config640M.json",
+    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-640M", "evodiff/config/config640M.json",
                                                       diffusion_timesteps=dt,
                                                       tokenizer=tokenizer)
     scheme = 'd3pm'
     if return_all:
         return model, collater, tokenizer, scheme, dt, Q_prod, Q_t
     else:
         return model, collater, tokenizer, scheme
 
 def D3PM_BLOSUM_38M(return_all=False):
     dt=500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
     Q_prod, Q_t = tokenizer.q_blosum_schedule(timesteps=dt)
     collater = D3PMCollater(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-38M", "config/config38M.json",
+    model, tokenizer = load_sequence_checkpoint("d3pm-blosum-38M", "evodiff/config/config38M.json",
                                                       diffusion_timesteps=dt,
                                                       tokenizer=tokenizer)
     scheme = 'd3pm'
     if return_all:
         return model, collater, tokenizer, scheme, dt, Q_prod, Q_t
     else:
         return model, collater, tokenizer, scheme
 
 def D3PM_UNIFORM_640M(return_all=False):
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollater(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_sequence_checkpoint("d3pm-uniform-640M", "config/config640M.json", diffusion_timesteps=dt,
+    model, tokenizer = load_sequence_checkpoint("d3pm-uniform-640M", "evodiff/config640M.json", diffusion_timesteps=dt,
                                             tokenizer=tokenizer)
     scheme = 'd3pm'
     if return_all:
         return model, collater, tokenizer, scheme, dt, Q_prod, Q_t
     else:
         return model, collater, tokenizer, scheme
 
 
 def D3PM_UNIFORM_38M(return_all=False):
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=True)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollater(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_sequence_checkpoint("d3pm-uniform-38M", "config/config38M.json", diffusion_timesteps=dt,
+    model, tokenizer = load_sequence_checkpoint("d3pm-uniform-38M", "evodiff/config/config38M.json", diffusion_timesteps=dt,
                                             tokenizer=tokenizer)
     scheme = 'd3pm'
     if return_all:
         return model, collater, tokenizer, scheme, dt, Q_prod, Q_t
     else:
         return model, collater, tokenizer, scheme
 
 
 def OA_AR_640M():
     tokenizer = Tokenizer()
     collater = OAMaskCollater(tokenizer=tokenizer)
-    model, tokenizer = load_sequence_checkpoint("oaar-640M", "config/config640M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("oaar-640M", "evodiff/config/config640M.json", diffusion_timesteps=None, \
                          tokenizer=tokenizer)
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 
 def OA_AR_38M():
     tokenizer = Tokenizer()
     collater = OAMaskCollater(tokenizer=tokenizer)
-    model, tokenizer = load_sequence_checkpoint("oaar-38M", "config/config38M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("oaar-38M", "evodiff/config/config38M.json", diffusion_timesteps=None, \
                          tokenizer=tokenizer)
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 
 def LR_AR_640M():
     n_tokens = len(PROTEIN_ALPHABET)
     tokenizer = Tokenizer(protein_alphabet=PROTEIN_ALPHABET, all_aas=ALL_AAS, pad=PAD)
     collater = LMCollater(PROTEIN_ALPHABET)
-    model, tokenizer = load_sequence_checkpoint("lrar-640M", "config/config640M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("lrar-640M", "evodiff/config/config640M.json", diffusion_timesteps=None, \
                                 tokenizer=tokenizer, causal=True, n_tokens=n_tokens)
     scheme='causal-mask'
     return model, collater, tokenizer, scheme
 
 
 def LR_AR_38M():
     n_tokens = len(PROTEIN_ALPHABET)
     tokenizer = Tokenizer(protein_alphabet=PROTEIN_ALPHABET, all_aas=ALL_AAS, pad=PAD)
     collater = LMCollater(PROTEIN_ALPHABET)
-    model, tokenizer = load_sequence_checkpoint("lrar-38M", "config/config38M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("lrar-38M", "evodiff/config/config38M.json", diffusion_timesteps=None, \
                                 tokenizer=tokenizer, causal=True, n_tokens=n_tokens)
     scheme='causal-mask'
     return model, collater, tokenizer, scheme
 
 def CARP_38M():
     n_tokens = len(PROTEIN_ALPHABET)
     tokenizer = Tokenizer(protein_alphabet=PROTEIN_ALPHABET, all_aas=ALL_AAS, pad=PAD)
     collater = OAMaskCollater(tokenizer=tokenizer)
-    model, tokenizer = load_sequence_checkpoint("carp-38M", "config/config38M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("carp-38M", "evodiff/config/config38M.json", diffusion_timesteps=None, \
                                 tokenizer=tokenizer, causal=False, n_tokens=n_tokens)
     scheme='mask'
     return model, collater, tokenizer, scheme
 
 def CARP_640M():
     n_tokens = len(PROTEIN_ALPHABET)
     tokenizer = Tokenizer(protein_alphabet=PROTEIN_ALPHABET, all_aas=ALL_AAS, pad=PAD)
     collater = OAMaskCollater(tokenizer=tokenizer)
-    model, tokenizer = load_sequence_checkpoint("carp-640M", "config/config640M.json", diffusion_timesteps=None, \
+    model, tokenizer = load_sequence_checkpoint("carp-640M", "evodiff/config/config640M.json", diffusion_timesteps=None, \
                                 tokenizer=tokenizer, causal=False, n_tokens=n_tokens)
     scheme='mask'
     return model, collater, tokenizer, scheme
 
 def ESM1b_650M():
     "Wrapper for ESM model"
     model, alphabet = esm.pretrained.esm1b_t33_650M_UR50S()
@@ -188,67 +188,67 @@
     return model, collater, alphabet, scheme
 
 def MSA_D3PM_BLOSUM_RANDSUB():
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=False)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollaterMSA(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_msa_checkpoint("msa-d3pm-blosum-randsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-d3pm-blosum-randsub", "evodiff/config/configMSA.json",
                                                 diffusion_timesteps=dt,
                                                 tokenizer=tokenizer)
     scheme = 'd3pm'
     return model, collater, tokenizer, scheme
 
 def MSA_D3PM_BLOSUM_MAXSUB():
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=False)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollaterMSA(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_msa_checkpoint("msa-d3pm-blosum-maxsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-d3pm-blosum-maxsub", "evodiff/config/configMSA.json",
                                                 diffusion_timesteps=dt,
                                                 tokenizer=tokenizer)
     scheme = 'd3pm'
     return model, collater, tokenizer, scheme
 
 def MSA_D3PM_UNIFORM_RANDSUB():
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=False)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollaterMSA(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_msa_checkpoint("msa-d3pm-uniform-randsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-d3pm-uniform-randsub", "evodiff/config/configMSA.json",
                                                 diffusion_timesteps=dt,
                                                 tokenizer=tokenizer)
     scheme = 'd3pm'
     return model, collater, tokenizer, scheme
 
 def MSA_D3PM_UNIFORM_MAXSUB():
     dt = 500
     tokenizer = Tokenizer(path_to_blosum="data/blosum62-special-MSA.mat", sequences=False)
     Q_prod, Q_t = tokenizer.q_random_schedule(timesteps=dt)
     collater = D3PMCollaterMSA(tokenizer=tokenizer, num_timesteps=dt, Q=Q_t, Q_bar=Q_prod)
-    model, tokenizer = load_msa_checkpoint("msa-d3pm-uniform-maxsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-d3pm-uniform-maxsub", "evodiff/config/configMSA.json",
                                                 diffusion_timesteps=dt,
                                                 tokenizer=tokenizer)
     scheme = 'd3pm'
     return model, collater, tokenizer, scheme
 
 
 def MSA_OA_AR_RANDSUB():
     tokenizer = Tokenizer()
     collater = MSAAbsorbingCollater(alphabet=MSA_ALPHABET)
-    model, tokenizer = load_msa_checkpoint("msa-oaar-randsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-oaar-randsub", "evodiff/config/configMSA.json",
                                            diffusion_timesteps=None,
                                            tokenizer=tokenizer)
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 def MSA_OA_AR_MAXSUB():
     tokenizer = Tokenizer()
     collater = MSAAbsorbingCollater(alphabet=MSA_ALPHABET)
-    model, tokenizer = load_msa_checkpoint("msa-oaar-maxsub", "config/configMSA.json",
+    model, tokenizer = load_msa_checkpoint("msa-oaar-maxsub", "evodiff/config/configMSA.json",
                                            diffusion_timesteps=None,
                                            tokenizer=tokenizer)
     scheme = 'mask'
     return model, collater, tokenizer, scheme
 
 def ESM_MSA_1b():
     "Wrapper for ESM model"
```

### Comparing `evodiff-0.0.2/evodiff/utils.py` & `evodiff-0.0.3/evodiff/utils.py`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.2/evodiff.egg-info/PKG-INFO` & `evodiff-0.0.3/evodiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
 Home-page: https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
@@ -32,17 +32,17 @@
 You will also need to install PyTorch. We tested our models on ` v2.0.1 `.
 
 We obtain sequences from the [Uniref50 dataset](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4375400/), which contains approximately 45 million protein sequences. The Multiple Sequence Alignments (MSAs) are from the [OpenFold dataset](https://www.biorxiv.org/content/10.1101/2022.11.20.517210v2), containing MSAs for 132,000 unique Protein Data Bank (PDB) chains.
 
 ### Loading pretrained models
 To load a model:
 ```
-from evodiff.pretrained import OA_AR_640M
+from evodiff.pretrained import OA_AR_38M
 
-model, collater, tokenizer, scheme = OA_AR_640M()
+model, collater, tokenizer, scheme = OA_AR_38M()
 ```
 Available models are:
 * ``` D3PM_BLOSUM_640M() ```
 * ``` D3PM_BLOSUM_38M() ```
 * ``` D3PM_UNIFORM_640M() ```
 * ``` D3PM_UNIFORM_38M() ```
 * ``` OA_AR_640M() ```
```

### Comparing `evodiff-0.0.2/setup.py` & `evodiff-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="evodiff", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     description="Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8.5',
-    package_data={'evodiff': ['config/*']},
+    # include_package_data=True,
+    package_data={'evodiff': ['*.json']},
 )
```

