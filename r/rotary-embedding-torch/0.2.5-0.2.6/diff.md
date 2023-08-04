# Comparing `tmp/rotary-embedding-torch-0.2.5.tar.gz` & `tmp/rotary-embedding-torch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary-embedding-torch-0.2.5.tar", last modified: Wed Jun 28 19:00:30 2023, max compression
+gzip compressed data, was "rotary-embedding-torch-0.2.6.tar", last modified: Fri Aug  4 17:16:25 2023, max compression
```

## Comparing `rotary-embedding-torch-0.2.5.tar` & `rotary-embedding-torch-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:00:30.133528 rotary-embedding-torch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-28 19:00:16.000000 rotary-embedding-torch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-28 19:00:30.133528 rotary-embedding-torch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-28 19:00:16.000000 rotary-embedding-torch-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:00:30.133528 rotary-embedding-torch-0.2.5/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-28 19:00:16.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-06-28 19:00:16.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 19:00:30.133528 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-28 19:00:30.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-28 19:00:30.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 19:00:30.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 19:00:30.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 19:00:30.000000 rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 19:00:30.133528 rotary-embedding-torch-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-28 19:00:16.000000 rotary-embedding-torch-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/setup.py
```

### Comparing `rotary-embedding-torch-0.2.5/LICENSE` & `rotary-embedding-torch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.5/PKG-INFO` & `rotary-embedding-torch-0.2.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.5/README.md` & `rotary-embedding-torch-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -100,15 +100,17 @@
 q, k = rotary_emb.rotate_queries_and_keys(q, k)
 ```
 
 ## Interpolating Sequence Positions
 
 This MetaAI <a href="https://arxiv.org/abs//2306.15595">paper</a> proposes simply fine-tuning on interpolations of the sequence positions for extending to longer context length for pretrained models. They show this performs much better than simply fine-tuning on the same sequence positions but extended further.
 
-You can use this by simply setting the `interpolation_factor` on initialization to a value greater than `1.` (ex. if pretrained model was trained on 2048, setting `interpolation_factor = 2.` would allow fine-tuning to `2048 x 2. = 4096`)
+You can use this by setting the `interpolate_factor` on initialization to a value greater than `1.` (ex. if pretrained model was trained on 2048, setting `interpolate_factor = 2.` would allow fine-tuning to `2048 x 2. = 4096`)
+
+Update: someone in the community has reported that it does not work well. please email me if you see either a positive or negative result
 
 ```python
 import torch
 from rotary_embedding_torch import RotaryEmbedding
 
 rotary_emb = RotaryEmbedding(
     dim = 32,
@@ -140,7 +142,15 @@
 ```bibtex
 @inproceedings{Chen2023ExtendingCW,
     title   = {Extending Context Window of Large Language Models via Positional Interpolation},
     author  = {Shouyuan Chen and Sherman Wong and Liangjian Chen and Yuandong Tian},
     year    = {2023}
 }
 ```
+
+```bibtex
+@misc{bloc97-2023
+    title   = {NTK-Aware Scaled RoPE allows LLaMA models to have extended (8k+) context size without any fine-tuning and minimal perplexity degradation.}
+    author  = {/u/bloc97},
+    url     = {https://www.reddit.com/r/LocalLLaMA/comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/}
+}
+```
```

#### html2text {}

```diff
@@ -45,24 +45,30 @@
 heads have been split out, but prior to the dot product and subsequent softmax
 (attention) # instead of using `rotate_queries_or_keys`, you will use
 `rotate_queries_and_keys`, the rest is taken care of q, k =
 rotary_emb.rotate_queries_and_keys(q, k) ``` ## Interpolating Sequence
 Positions This MetaAI paper proposes simply fine-tuning on interpolations of
 the sequence positions for extending to longer context length for pretrained
 models. They show this performs much better than simply fine-tuning on the same
-sequence positions but extended further. You can use this by simply setting the
-`interpolation_factor` on initialization to a value greater than `1.` (ex. if
-pretrained model was trained on 2048, setting `interpolation_factor = 2.` would
-allow fine-tuning to `2048 x 2. = 4096`) ```python import torch from
-rotary_embedding_torch import RotaryEmbedding rotary_emb = RotaryEmbedding( dim
-= 32, interpolate_factor = 2. # add this line of code to pretrained model and
-fine-tune for ~1000 steps, as shown in paper ) ``` ## Citations ```bibtex @misc
+sequence positions but extended further. You can use this by setting the
+`interpolate_factor` on initialization to a value greater than `1.` (ex. if
+pretrained model was trained on 2048, setting `interpolate_factor = 2.` would
+allow fine-tuning to `2048 x 2. = 4096`) Update: someone in the community has
+reported that it does not work well. please email me if you see either a
+positive or negative result ```python import torch from rotary_embedding_torch
+import RotaryEmbedding rotary_emb = RotaryEmbedding( dim = 32,
+interpolate_factor = 2. # add this line of code to pretrained model and fine-
+tune for ~1000 steps, as shown in paper ) ``` ## Citations ```bibtex @misc
 {su2021roformer, title = {RoFormer: Enhanced Transformer with Rotary Position
 Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and
 Yunfeng Liu}, year = {2021}, eprint = {2104.09864}, archivePrefix = {arXiv},
 primaryClass = {cs.CL} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
 Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
 Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
 and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex @inproceedings
 {Chen2023ExtendingCW, title = {Extending Context Window of Large Language
 Models via Positional Interpolation}, author = {Shouyuan Chen and Sherman Wong
-and Liangjian Chen and Yuandong Tian}, year = {2023} } ```
+and Liangjian Chen and Yuandong Tian}, year = {2023} } ``` ```bibtex @misc
+{bloc97-2023 title = {NTK-Aware Scaled RoPE allows LLaMA models to have
+extended (8k+) context size without any fine-tuning and minimal perplexity
+degradation.} author = {/u/bloc97}, url = {https://www.reddit.com/r/LocalLLaMA/
+comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/} } ```
```

### Comparing `rotary-embedding-torch-0.2.5/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary-embedding-torch-0.2.6/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,23 @@
         freqs_for = 'lang',
         theta = 10000,
         max_freq = 10,
         num_freqs = 1,
         learned_freq = False,
         use_xpos = False,
         xpos_scale_base = 512,
-        interpolate_factor = 1.
+        interpolate_factor = 1.,
+        theta_rescale_factor = 1.
     ):
         super().__init__()
+        # proposed by reddit user bloc97, to rescale rotary embeddings to longer sequence length without fine-tuning
+        # has some connection to NTK literature
+        # https://www.reddit.com/r/LocalLLaMA/comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/
+        theta *= theta_rescale_factor ** (dim / (dim - 2))
+
         if exists(custom_freqs):
             freqs = custom_freqs
         elif freqs_for == 'lang':
             freqs = 1. / (theta ** (torch.arange(0, dim, 2)[:(dim // 2)].float() / dim))
         elif freqs_for == 'pixel':
             freqs = torch.linspace(1., max_freq / 2, dim // 2) * pi
         elif freqs_for == 'constant':
```

### Comparing `rotary-embedding-torch-0.2.5/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.5/setup.py` & `rotary-embedding-torch-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.2.5',
+  version = '0.2.6',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

