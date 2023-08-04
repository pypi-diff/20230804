# Comparing `tmp/linktransformer-0.1.0.tar.gz` & `tmp/linktransformer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktransformer-0.1.0.tar", last modified: Tue Aug  1 03:15:37 2023, max compression
+gzip compressed data, was "linktransformer-0.1.1.tar", last modified: Fri Aug  4 09:12:20 2023, max compression
```

## Comparing `linktransformer-0.1.0.tar` & `linktransformer-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.0/LICENSE.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.0/MANIFEST.in
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6612 2023-08-01 03:15:37.376510 linktransformer-0.1.0/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4822 2023-08-01 02:24:24.000000 linktransformer-0.1.0/README.md
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-01 02:47:57.000000 linktransformer-0.1.0/pyproject.toml
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-01 03:15:37.376510 linktransformer-0.1.0/setup.cfg
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.372510 linktransformer-0.1.0/src/
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/src/linktransformer/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      196 2023-07-31 22:07:54.000000 linktransformer-0.1.0/src/linktransformer/__init__.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/src/linktransformer/configs/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.0/src/linktransformer/configs/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      385 2023-07-31 15:19:15.000000 linktransformer-0.1.0/src/linktransformer/configs/linkage.json
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/src/linktransformer/data/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.0/src/linktransformer/data/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.0/src/linktransformer/data/coarse.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.0/src/linktransformer/data/es_mexican_products.xlsx
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.0/src/linktransformer/data/fine.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.0/src/linktransformer/data/toy_comp_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.0/src/linktransformer/data/toy_comp_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.0/src/linktransformer/data/toy_multi_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.0/src/linktransformer/data/toy_multi_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.0/src/linktransformer/data/translation_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.0/src/linktransformer/data/translation_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13310 2023-08-01 02:59:59.000000 linktransformer-0.1.0/src/linktransformer/infer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4059 2023-08-01 02:30:53.000000 linktransformer-0.1.0/src/linktransformer/model_card_templates.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/src/linktransformer/modified_sbert/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    11761 2023-08-01 02:25:49.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/LinkTransformer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3382 2023-08-01 01:32:03.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/cluster_fns.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/data_loaders.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    16108 2023-07-30 18:14:20.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/evaluation.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/losses.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4361 2023-08-01 02:54:25.000000 linktransformer-0.1.0/src/linktransformer/modified_sbert/train.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9140 2023-08-01 02:48:11.000000 linktransformer-0.1.0/src/linktransformer/preprocess.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6571 2023-08-01 02:59:39.000000 linktransformer-0.1.0/src/linktransformer/train_model.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     2429 2023-08-01 02:59:57.000000 linktransformer-0.1.0/src/linktransformer/utils.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-01 03:15:37.376510 linktransformer-0.1.0/src/linktransformer.egg-info/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6612 2023-08-01 03:15:37.000000 linktransformer-0.1.0/src/linktransformer.egg-info/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1291 2023-08-01 03:15:37.000000 linktransformer-0.1.0/src/linktransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-01 03:15:37.000000 linktransformer-0.1.0/src/linktransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-01 03:15:37.000000 linktransformer-0.1.0/src/linktransformer.egg-info/requires.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-01 03:15:37.000000 linktransformer-0.1.0/src/linktransformer.egg-info/top_level.txt
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.778906 linktransformer-0.1.1/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1078 2023-07-31 06:29:08.000000 linktransformer-0.1.1/LICENSE.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.1/MANIFEST.in
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 09:12:20.778906 linktransformer-0.1.1/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6506 2023-08-04 08:35:37.000000 linktransformer-0.1.1/README.md
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1159 2023-08-01 15:57:37.000000 linktransformer-0.1.1/pyproject.toml
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-08-04 09:12:20.778906 linktransformer-0.1.1/setup.cfg
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.770906 linktransformer-0.1.1/src/
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      228 2023-08-04 07:11:40.000000 linktransformer-0.1.1/src/linktransformer/__init__.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/configs/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      155 2023-07-30 23:26:02.000000 linktransformer-0.1.1/src/linktransformer/configs/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      489 2023-08-03 18:53:19.000000 linktransformer-0.1.1/src/linktransformer/configs/linkage.json
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer/data/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.1/src/linktransformer/data/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/coarse.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/es_mexican_products.xlsx
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/fine.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/toy_comp_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.1/src/linktransformer/data/toy_comp_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.1/src/linktransformer/data/toy_multi_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.1/src/linktransformer/data/toy_multi_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.1/src/linktransformer/data/toy_pairs.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.1/src/linktransformer/data/translation_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.1/src/linktransformer/data/translation_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    17215 2023-08-04 06:03:40.000000 linktransformer-0.1.1/src/linktransformer/infer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     5675 2023-08-04 08:58:00.000000 linktransformer-0.1.1/src/linktransformer/model_card_templates.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.778906 linktransformer-0.1.1/src/linktransformer/modified_sbert/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    12778 2023-08-04 08:39:49.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/LinkTransformer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-07-31 04:10:46.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3382 2023-08-01 01:32:03.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/cluster_fns.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/data_loaders.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-02 20:50:51.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/evaluation.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/losses.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6296 2023-08-04 06:19:29.000000 linktransformer-0.1.1/src/linktransformer/modified_sbert/train.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    25645 2023-08-03 02:50:02.000000 linktransformer-0.1.1/src/linktransformer/preprocess.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8408 2023-08-04 08:53:23.000000 linktransformer-0.1.1/src/linktransformer/train_model.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4148 2023-08-04 06:26:48.000000 linktransformer-0.1.1/src/linktransformer/utils.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-08-04 09:12:20.774906 linktransformer-0.1.1/src/linktransformer.egg-info/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     8297 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1330 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      116 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/requires.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-08-04 09:12:20.000000 linktransformer-0.1.1/src/linktransformer.egg-info/top_level.txt
```

### Comparing `linktransformer-0.1.0/LICENSE.txt` & `linktransformer-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/PKG-INFO` & `linktransformer-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,32 +55,32 @@
 pip install linktransformer
 ```
 
 ## Getting Started
 
 ```python
 
-from linktransformer import lm_merge_df, dedup
-
+import linktransformer as lt
 # Example usage of lm_merge_df
-merged_df = lm_merge_df(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model')
+merged_df = lt.merge(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model-from-huggingface')
 
 # Example usage of dedup
-deduplicated_df = dedup(df, model='your-pretrained-model', on='text_column', threshold=0.8)
+deduplicated_df = lt.dedup_rows(df, model='your-pretrained-model', on='text_column', threshold=0.8)
 ```
 
+All transformer based models from [HuggingFace](https://huggingface.co/) are supported. We recommend [sentence-transformers](https://www.sbert.net/docs/pretrained_models.html) for these tasks as they are trained for semantic similarity tasks. 
 
 ## Usage 
 
 ### Merging Pandas Dataframes
 
-The lm_merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
+The merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
 
 ```python
-def lm_merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
+def merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
                  use_gpu=False, batch_size=128, pooling_type='mean', openai_key=None):
     """
     Merge two dataframes using language model embeddings
     :param df1: first dataframe (left) 
     :param df2: second dataframe (right)
     :param merge_type: type of merge to perform 1:m or m:1 or 1:1
     :param model: language model to use
@@ -90,30 +90,66 @@
     :param suffixes: suffixes to use for overlapping columns
     :return: merged dataframe
     """
 
 
 ```
 
-A special case of merging is aggregation - when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, lm_merge_blocking can be used to merge within blocking keys. 
+A special case of merging is aggregation (use function: aggregate_rows)- when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, merge_blocking can be used to merge within blocking keys. 
 
 
-### Deduplicating Data
+### Clustering or Deduplicating Data
 ```python
-def dedup(df, model, on, threshold=0.5, openai_key=None):
+def dedup_rows(df, model, on, threshold=0.5, openai_key=None):
+    """
+    A function to deduplicate a dataframe based on a similarity threshold
+    :param df: dataframe to deduplicate
+    :param model: language model to use
+    :param on: column to deduplicate on
+    :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
+    :return: deduplicated dataframe
+    """
+
+def cluster_rows(df, model, on, threshold=0.5, openai_key=None):
     """
     A function to deduplicate a dataframe based on a similarity threshold
     :param df: dataframe to deduplicate
     :param model: language model to use
     :param on: column to deduplicate on
     :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
     :return: deduplicated dataframe
     """
+
+```
+
+We allow a simple clustering function to cluster rows based on a key. Deduplication is just keeping only one row per cluster.
+
+
+### Get similarity score between 2 sets of columns
+
+```python
+
+def evaluate_pairs(df,model,left_on,right_on,openai_key=None):
+    """
+    This function evaluates paired columns in a dataframe and gives a match score (cosine similarity). 
+    Typically, this can be though of as a way to evaluate already merged in dataframes.
+
+    :param df (DataFrame): Dataframe to evaluate.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to evaluate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to evaluate on in df.
+    :return: DataFrame: The evaluated dataframe.
+    """
+
+
 ```
 
+
 ### Training your own LinkTransformer model
 
 ```python
 
 
 def train_model(
     model_path: str='your-pretrained-model',
@@ -125,38 +161,40 @@
     config_path: str = LINKAGE_CONFIG_PATH,
     training_args: dict = {"num_epochs":10},
     log_wandb: bool = False,
 ) -> str:
     """
     Train the LinkTransformer model.
 
-    Args:
-        model_path (str): The name of the model to use.
-        dataset_path (str): Path to the dataset in Excel format.
-        left_col_names (List[str]): List of column names to use as left side data.
-        right_col_names (List[str]): List of column names to use as right side data.
-        left_id_name (List[str]): List of column names to use as identifiers for the left data.
-        right_id_name (List[str]): List of column names to use as identifiers for the right data.
-        config_path (str): Path to the JSON configuration file.
-        training_args (dict): Dictionary of training arguments to override the config.
-        log_wandb (bool): Whether to log the training run on wandb.
-
-    Returns:
-        str: The path to the saved best model.
+    :param model_path (str): The name of the model to use.
+    :param dataset_path (str): Path to the dataset in Excel format.
+    :param left_col_names (List[str]): List of column names to use as left side data.
+    :param right_col_names (List[str]): List of column names to use as right side data.
+    :param left_id_name (List[str]): List of column names to use as identifiers for the left data.
+    :param right_id_name (List[str]): List of column names to use as identifiers for the right data.
+    :param config_path (str): Path to the JSON configuration file.
+    :param training_args (dict): Dictionary of training arguments to override the config.
+    :param log_wandb (bool): Whether to log the training run on wandb.
+    :returns: str: The path to the saved best model.
     """
 
 
 ```
 
 
+
+
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvement, please create a new issue or submit a pull request.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
 The sentence-transformers library and HugginFace for providing pre-trained NLP models
 The faiss library for efficient similarity search
 The sklearn and networkx libraries for clustering and graph operations
 OpenAI for providing language model embeddings
 
+
+## Roadmap 
+We will continue to come up with more feature rich updates and introduce more modalities like images using support for vision and multimodal models.
```

### Comparing `linktransformer-0.1.0/README.md` & `linktransformer-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 pip install linktransformer
 ```
 
 ## Getting Started
 
 ```python
 
-from linktransformer import lm_merge_df, dedup
-
+import linktransformer as lt
 # Example usage of lm_merge_df
-merged_df = lm_merge_df(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model')
+merged_df = lt.merge(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model-from-huggingface')
 
 # Example usage of dedup
-deduplicated_df = dedup(df, model='your-pretrained-model', on='text_column', threshold=0.8)
+deduplicated_df = lt.dedup_rows(df, model='your-pretrained-model', on='text_column', threshold=0.8)
 ```
 
+All transformer based models from [HuggingFace](https://huggingface.co/) are supported. We recommend [sentence-transformers](https://www.sbert.net/docs/pretrained_models.html) for these tasks as they are trained for semantic similarity tasks. 
 
 ## Usage 
 
 ### Merging Pandas Dataframes
 
-The lm_merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
+The merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
 
 ```python
-def lm_merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
+def merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
                  use_gpu=False, batch_size=128, pooling_type='mean', openai_key=None):
     """
     Merge two dataframes using language model embeddings
     :param df1: first dataframe (left) 
     :param df2: second dataframe (right)
     :param merge_type: type of merge to perform 1:m or m:1 or 1:1
     :param model: language model to use
@@ -55,30 +55,66 @@
     :param suffixes: suffixes to use for overlapping columns
     :return: merged dataframe
     """
 
 
 ```
 
-A special case of merging is aggregation - when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, lm_merge_blocking can be used to merge within blocking keys. 
+A special case of merging is aggregation (use function: aggregate_rows)- when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, merge_blocking can be used to merge within blocking keys. 
 
 
-### Deduplicating Data
+### Clustering or Deduplicating Data
 ```python
-def dedup(df, model, on, threshold=0.5, openai_key=None):
+def dedup_rows(df, model, on, threshold=0.5, openai_key=None):
+    """
+    A function to deduplicate a dataframe based on a similarity threshold
+    :param df: dataframe to deduplicate
+    :param model: language model to use
+    :param on: column to deduplicate on
+    :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
+    :return: deduplicated dataframe
+    """
+
+def cluster_rows(df, model, on, threshold=0.5, openai_key=None):
     """
     A function to deduplicate a dataframe based on a similarity threshold
     :param df: dataframe to deduplicate
     :param model: language model to use
     :param on: column to deduplicate on
     :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
     :return: deduplicated dataframe
     """
+
+```
+
+We allow a simple clustering function to cluster rows based on a key. Deduplication is just keeping only one row per cluster.
+
+
+### Get similarity score between 2 sets of columns
+
+```python
+
+def evaluate_pairs(df,model,left_on,right_on,openai_key=None):
+    """
+    This function evaluates paired columns in a dataframe and gives a match score (cosine similarity). 
+    Typically, this can be though of as a way to evaluate already merged in dataframes.
+
+    :param df (DataFrame): Dataframe to evaluate.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to evaluate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to evaluate on in df.
+    :return: DataFrame: The evaluated dataframe.
+    """
+
+
 ```
 
+
 ### Training your own LinkTransformer model
 
 ```python
 
 
 def train_model(
     model_path: str='your-pretrained-model',
@@ -90,38 +126,40 @@
     config_path: str = LINKAGE_CONFIG_PATH,
     training_args: dict = {"num_epochs":10},
     log_wandb: bool = False,
 ) -> str:
     """
     Train the LinkTransformer model.
 
-    Args:
-        model_path (str): The name of the model to use.
-        dataset_path (str): Path to the dataset in Excel format.
-        left_col_names (List[str]): List of column names to use as left side data.
-        right_col_names (List[str]): List of column names to use as right side data.
-        left_id_name (List[str]): List of column names to use as identifiers for the left data.
-        right_id_name (List[str]): List of column names to use as identifiers for the right data.
-        config_path (str): Path to the JSON configuration file.
-        training_args (dict): Dictionary of training arguments to override the config.
-        log_wandb (bool): Whether to log the training run on wandb.
-
-    Returns:
-        str: The path to the saved best model.
+    :param model_path (str): The name of the model to use.
+    :param dataset_path (str): Path to the dataset in Excel format.
+    :param left_col_names (List[str]): List of column names to use as left side data.
+    :param right_col_names (List[str]): List of column names to use as right side data.
+    :param left_id_name (List[str]): List of column names to use as identifiers for the left data.
+    :param right_id_name (List[str]): List of column names to use as identifiers for the right data.
+    :param config_path (str): Path to the JSON configuration file.
+    :param training_args (dict): Dictionary of training arguments to override the config.
+    :param log_wandb (bool): Whether to log the training run on wandb.
+    :returns: str: The path to the saved best model.
     """
 
 
 ```
 
 
+
+
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvement, please create a new issue or submit a pull request.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
 The sentence-transformers library and HugginFace for providing pre-trained NLP models
 The faiss library for efficient similarity search
 The sklearn and networkx libraries for clustering and graph operations
 OpenAI for providing language model embeddings
 
+
+## Roadmap 
+We will continue to come up with more feature rich updates and introduce more modalities like images using support for vision and multimodal models.
```

### Comparing `linktransformer-0.1.0/pyproject.toml` & `linktransformer-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linktransformer"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
        "scikit-learn",
         "faiss-cpu",
         "hdbscan",
         "networkx",
         "torch",
         "sentence_transformers",
```

### Comparing `linktransformer-0.1.0/src/linktransformer/data/es_mexican_products.xlsx` & `linktransformer-0.1.1/src/linktransformer/data/es_mexican_products.xlsx`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/data/toy_multi_2.csv` & `linktransformer-0.1.1/src/linktransformer/data/toy_multi_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/data/translation_1.csv` & `linktransformer-0.1.1/src/linktransformer/data/translation_1.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/data/translation_2.csv` & `linktransformer-0.1.1/src/linktransformer/data/translation_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/infer.py` & `linktransformer-0.1.1/src/linktransformer/infer.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import numpy as np
 import pandas as pd
 import faiss
 from typing import Union, List, Optional, Tuple,Dict, Any
 from pandas import DataFrame
 
 from linktransformer.modified_sbert.cluster_fns import cluster
-from linktransformer.utils import serialize_columns, infer_embeddings, load_model
+from linktransformer.utils import serialize_columns, infer_embeddings, load_model, cosine_similarity
 
 
 
 
 
 
 
-def lm_merge(
+def merge(
     df1: DataFrame,
     df2: DataFrame,
     merge_type: str = '1:1',
     on: Optional[Union[str, List[str]]] = None,
     model: str = "all-MiniLM-L6-v2",
     left_on: Optional[Union[str, List[str]]] = None,
     right_on: Optional[Union[str, List[str]]] = None,
@@ -59,39 +59,44 @@
     ### If how is 1:m, then we want to merge df1 to df2
     ### Check if how is valid
     if merge_type not in ["1:m", "m:1", "1:1"]:
         raise ValueError(f"Invalid merge type: {merge_type}")
 
     if merge_type == "1:m":
         if df1[left_on].duplicated().any():
-            raise ValueError(f"Keys in df1 are not unique")
+           print("Warning: Keys in df1 are not unique")
 
     if merge_type == "m:1":
         ## Check if keys in df2 are unique
         if df2[right_on].duplicated().any():
-            raise ValueError(f"Keys in df2 are not unique")
-
+            print("Warning: Keys in df2 are not unique")
     if merge_type == "1:1":
         ## Check if keys in df1 are unique
         if df1[left_on].duplicated().any():
-            raise ValueError(f"Keys in df1 are not unique")
+           print("Warning: Keys in df1 are not unique")
         ## Check if keys in df2 are unique
         if df2[right_on].duplicated().any():
-            raise ValueError(f"Keys in df2 are not unique")
+           print("Warning: Keys in df1 are not unique")
 
     df1 = df1.copy()
     df2 = df2.copy()
     ## give ids to each df
-    df1.loc[:, "id"] = np.arange(len(df1))
-    df2.loc[:, "id"] = np.arange(len(df2))
+    ##Ensure that there is no id_lt column in df1 or df2
+    if "id_lt" in df1.columns:
+        raise ValueError(f"Column id_lt already exists in df1, please rename it to proceed")
+    if "id_lt" in df2.columns:
+        raise ValueError(f"Column id_lt already exists in df2,please rename it to proceed")
+
+    df1.loc[:, "id_lt"] = np.arange(len(df1))
+    df2.loc[:, "id_lt"] = np.arange(len(df2))
 
     if isinstance(right_on, list):
-        strings_right = serialize_columns(df2, right_on, sep_token=model)
+        strings_right = serialize_columns(df2, right_on, model=model)
     if isinstance(left_on, list):
-        strings_left = serialize_columns(df1, left_on, sep_token=model)
+        strings_left = serialize_columns(df1, left_on, model=model)
     else:
         strings_left = df1[left_on].tolist()
         strings_right = df2[right_on].tolist()
 
     ## Load the model
     model = load_model(model)
 
@@ -142,15 +147,15 @@
 
     print(f"LM matched on key columns - left: {left_on}{suffixes[0]}, right: {right_on}{suffixes[1]}")
     return df_lm_matched
 
     
 
 
-def lm_merge_blocking(
+def merge_blocking(
     df1: DataFrame,
     df2: DataFrame,
     merge_type: str = '1:1',
     on: Optional[Union[str, List[str]]] = None,
     model: str = "all-MiniLM-L6-v2",
     left_on: Optional[Union[str, List[str]]] = None,
     right_on: Optional[Union[str, List[str]]] = None,
@@ -159,36 +164,33 @@
     use_gpu: bool = False,
     batch_size: int = 128,
     openai_key: Optional[str] = None
 ) -> DataFrame:
     """
     Merge two dataframes using language model embeddings with optional blocking.
 
-    Args:
-        df1 (DataFrame): First dataframe (left).
-        df2 (DataFrame): Second dataframe (right).
-        merge_type (str): Type of merge to perform (1:m or m:1 or 1:1).
-        model (str): Language model to use.
-        on (Union[str, List[str]], optional): Column(s) to join on in df1. Defaults to None.
-        left_on (Union[str, List[str]], optional): Column(s) to join on in df1. Defaults to None.
-        right_on (Union[str, List[str]], optional): Column(s) to join on in df2. Defaults to None.
-        blocking_vars (List[str], optional): Columns to use for blocking. Defaults to None.
-        suffixes (Tuple[str, str]): Suffixes to use for overlapping columns. Defaults to ('_x', '_y').
-        use_gpu (bool): Whether to use GPU. Not supported yet. Defaults to False.
-        batch_size (int): Batch size for inferencing embeddings. Defaults to 128.
-        openai_key (str, optional): OpenAI API key for InferKit API. Defaults to None.
-
-    Returns:
-        DataFrame: The merged dataframe.
+    :param df1 (DataFrame): First dataframe (left).
+    :param df2 (DataFrame): Second dataframe (right).
+    :param merge_type (str): Type of merge to perform (1:m or m:1 or 1:1).
+    :param model (str): Language model to use.
+    :param on (Union[str, List[str]], optional): Column(s) to join on in df1. Defaults to None.
+    :param left_on (Union[str, List[str]], optional): Column(s) to join on in df1. Defaults to None.
+    :param right_on (Union[str, List[str]], optional): Column(s) to join on in df2. Defaults to None.
+    :param blocking_vars (List[str], optional): Columns to use for blocking. Defaults to None.
+    :param suffixes (Tuple[str, str]): Suffixes to use for overlapping columns. Defaults to ('_x', '_y').
+    :param use_gpu (bool): Whether to use GPU. Not supported yet. Defaults to False.
+    :param batch_size (int): Batch size for inferencing embeddings. Defaults to 128.
+    :param openai_key (str, optional): OpenAI API key for InferKit API. Defaults to None.
+    :return: DataFrame: The merged dataframe.
     """
     ### For blocking, we need to chunk the dfs into blocks
     ### First, we need to check if blocking vars are specified
     if blocking_vars is None:
         print("No blocking vars specified, matching between all rows")
-        df_lm_matched = lm_merge(df1, df2, merge_type=merge_type, on=on, model=model, left_on=left_on,
+        df_lm_matched = merge(df1, df2, merge_type=merge_type, on=on, model=model, left_on=left_on,
                                     right_on=right_on, suffixes=suffixes, use_gpu=use_gpu, batch_size=batch_size,
                                      openai_key=openai_key)
         return df_lm_matched
     else:
         ## Partition the dfs into blocks
         ## First, check if blocking vars are in df1 and df2 - both should exist
         if not set(blocking_vars).issubset(set(df1.columns)):
@@ -222,15 +224,15 @@
         common_keys = set(df1_block_list).intersection(set(df2_block_list))
 
         for block_1 in common_keys:
             print(f"Merging block {block_1}")
             df1_block = df1_blocks.get_group(block_1)
             df2_block = df2_blocks.get_group(block_1)
             ## Merge the blocks
-            df_block_matched = lm_merge(df1_block, df2_block, merge_type=merge_type, on=on, model=model,
+            df_block_matched = merge(df1_block, df2_block, merge_type=merge_type, on=on, model=model,
                                            left_on=left_on, right_on=right_on, suffixes=suffixes, use_gpu=use_gpu,
                                            batch_size=batch_size, openai_key=openai_key)
             ## Add to merged dfs
             merged_dfs.append(df_block_matched)
 
         ## Add df corresponding to skipped keys
         for block_1 in skipped_keys_1:
@@ -242,105 +244,191 @@
             merged_dfs.append(df2_block)
 
         ## Concatenate the merged dfs
         df_lm_matched = pd.concat(merged_dfs, axis=0).reset_index(drop=True)
         return df_lm_matched
 
 
-def dedup(
+
+
+def aggregate_rows(
+    df: DataFrame,
+    ref_df: DataFrame,
+    model: str,
+    left_on: Union[str, List[str]],
+    right_on: Union[str, List[str]],
+    openai_key: str = None
+) -> DataFrame:
+    """
+    Aggregate the dataframe based on a reference dataframe using a language model.
+
+    :param df (DataFrame): Dataframe to aggregate.
+    :param ref_df (DataFrame): Reference dataframe to aggregate on.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to aggregate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to aggregate on in ref_df.
+    :return: DataFrame: The aggregated dataframe.
+    """
+
+    df = df.copy()
+    ref_df = ref_df.copy()
+
+    ## Just use the merge function with merge type 1:m
+    df_lm_matched = merge(df, ref_df, merge_type="1:1", on=None, model=model, left_on=left_on,
+                                right_on=right_on, suffixes=("_x", "_y"), use_gpu=False, batch_size=128,
+                                 openai_key=openai_key)
+
+    return df_lm_matched
+
+
+
+def evaluate_pairs(df,model,left_on,right_on,openai_key=None):
+    """
+    This function evaluates paired columns in a dataframe and gives a match score (cosine similarity). 
+    Typically, this can be though of as a way to evaluate already merged in dataframes.
+
+    :param df (DataFrame): Dataframe to evaluate.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to evaluate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to evaluate on in df.
+    :return: DataFrame: The evaluated dataframe.
+    """
+
+    df = df.copy()
+
+    ###We will serialize the columns if they are lists
+    if isinstance(left_on, list):
+        strings_left = serialize_columns(df, left_on, model=model)
+    else:
+        strings_left = df[left_on].tolist()
+    
+    if isinstance(right_on, list):
+        strings_right = serialize_columns(df, right_on, model=model)
+    else:
+        strings_right = df[right_on].tolist()
+
+    ## Load the model
+    model = load_model(model)
+
+    ## Infer embeddings for df1
+    embeddings1 = infer_embeddings(strings_left, model, batch_size=128, openai_key=openai_key)
+    ## Infer embeddings for df2
+    embeddings2 = infer_embeddings(strings_right, model, batch_size=128, openai_key=openai_key)
+
+    ### Expand dim if embeddings are 1d (numpy)
+    if len(embeddings1.shape) == 1:
+        embeddings1 = np.expand_dims(embeddings1, axis=0)
+    if len(embeddings2.shape) == 1:
+        embeddings2 = np.expand_dims(embeddings2, axis=0)
+    ## Normalize embedding tensors using numpy
+
+    embeddings1 = embeddings1 / np.linalg.norm(embeddings1, axis=1, keepdims=True)
+    embeddings2 = embeddings2 / np.linalg.norm(embeddings2, axis=1, keepdims=True)
+
+    ## Compute cosine similarity between CORRESPONDING pair of embeddings
+    cosine_similarity_12 = cosine_similarity(embeddings1,embeddings2)
+    print(cosine_similarity_12.shape)
+
+    ## Add cosine similarity to df
+    df["score"] = cosine_similarity_12.flatten()
+
+    return df
+
+def cluster_rows(
     df: DataFrame,
     model: str,
     on: Union[str, List[str]],
     cluster_type: str = "SLINK",
     cluster_params: Dict[str, Any] = {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"},
     openai_key: str = None
 ) -> DataFrame:
     """
-    Deduplicate a dataframe based on a similarity threshold.
+    Deduplicate a dataframe based on a similarity threshold. Various clustering options are supported.         
+    "agglomerative": {
+            "threshold": 0.5,
+            "clustering linkage": "ward",  # You can choose a default linkage method
+            "metric": "euclidean",  # You can choose a default metric
+        },
+        "HDBScan": {
+            "min cluster size": 5,
+            "min samples": 1,
+        },
+        "SLINK": {
+            "min cluster size": 2,
+            "threshold": 0.1,
+        },
+    }
 
-    Args:
-        df (DataFrame): Dataframe to deduplicate.
-        model (str): Language model to use.
-        on (Union[str, List[str]]): Column(s) to deduplicate on.
-        cluster_type (str): Clustering method to use. Defaults to "SLINK".
-        cluster_params (Dict[str, Any]): Parameters for clustering method. Defaults to {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"}.
-        openai_key (str): OpenAI API key for InferKit API. Defaults to None.
-
-    Returns:
-        DataFrame: The deduplicated dataframe.
+    :param df (DataFrame): Dataframe to deduplicate.
+    :param model (str): Language model to use.
+    :param on (Union[str, List[str]]): Column(s) to deduplicate on.
+    :param cluster_type (str): Clustering method to use. Defaults to "SLINK".
+    :param cluster_params (Dict[str, Any]): Parameters for clustering method. Defaults to {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"}.
+    :param openai_key (str): OpenAI API key
+    :return: DataFrame: The deduplicated dataframe.
     """
     print(f"Deduplicating dataframe with originally {len(df)} rows")
 
     df = df.copy()
 
     ### First, deduplicate based on exact matches
     df = df.drop_duplicates(subset=on, keep="first")
     print(f"Exact matches found: dropping them")
     print(f"Number of rows after exact match deduplication: {len(df)}")
 
     ### Now, deduplicate based on similarity threshold
     ## First, get the embeddings
     ### If len(on)>1, then we need to serialize the columns
     if isinstance(on, list):
-        strings = serialize_columns(df, on, sep_token=model)
+        strings = serialize_columns(df, on, model=model)
     else:
         strings = df[on].tolist()
     
     ## Infer embeddings for df
     embeddings = infer_embeddings(strings, model, batch_size=128, openai_key=openai_key)
     ## Normalize embedding tensors using numpy
     embeddings = embeddings / np.linalg.norm(embeddings, axis=1, keepdims=True)
     ### Now, cluster the embeddings based on similarity threshold
     labels = cluster(cluster_type, cluster_params, embeddings, corpus_ids=None)
-    print(labels)
     ### Now, keep only 1 row per cluster
     df["cluster"] = labels
-    df = df.drop_duplicates(subset="cluster", keep="first")
-    print(f"Similarity matches found: {len(df)}, dropping them")
-
     return df
 
 
-def lm_aggregate(
+
+
+
+def dedup_rows(
     df: DataFrame,
-    ref_df: DataFrame,
     model: str,
-    left_on: Union[str, List[str]],
-    right_on: Union[str, List[str]],
+    on: Union[str, List[str]],
+    cluster_type: str = "SLINK",
+    cluster_params: Dict[str, Any] = {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"},
     openai_key: str = None
 ) -> DataFrame:
     """
-    Aggregate the dataframe based on a reference dataframe using a language model.
-
-    Args:
-        df (DataFrame): Dataframe to aggregate.
-        ref_df (DataFrame): Reference dataframe to aggregate on.
-        model (str): Language model to use.
-        left_on (Union[str, List[str]]): Column(s) to aggregate on in df.
-        right_on (Union[str, List[str]]): Reference column(s) to aggregate on in ref_df.
+    Deduplicate a dataframe based on a similarity threshold. This is just clustering and keeping the first row in each cluster.
+    Refer to the docs for the cluster_rows function for more details.
 
-    Returns:
-        DataFrame: The aggregated dataframe.
+    :param df (DataFrame): Dataframe to deduplicate.
+    :param model (str): Language model to use.
+    :param on (Union[str, List[str]]): Column(s) to deduplicate on.
+    :param cluster_type (str): Clustering method to use. Defaults to "SLINK".
+    :param cluster_params (Dict[str, Any]): Parameters for clustering method. Defaults to {'threshold': 0.5, "min cluster size": 2, "metric": "cosine"}.
+    :param openai_key (str): OpenAI API key
+    :return: DataFrame: The deduplicated dataframe.
     """
 
-    df = df.copy()
-    ref_df = ref_df.copy()
-
-    ## Just use the merge function with merge type 1:m
-    df_lm_matched = lm_merge(df, ref_df, merge_type="1:1", on=None, model=model, left_on=left_on,
-                                right_on=right_on, suffixes=("_x", "_y"), use_gpu=False, batch_size=128,
-                                 openai_key=openai_key)
-
-    return df_lm_matched
-
-
-
-
+    print(f"Deduplicating dataframe with originally {len(df)} rows")
+    df = cluster_rows(df, model, on, cluster_type, cluster_params, openai_key)
+    df = df.drop_duplicates(subset="cluster", keep="first")
+    df = df.drop(columns=["cluster"])
+    print(f"Number of rows after deduplication: {len(df)}")
 
-    
+    return df
```

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/LinkTransformer.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/LinkTransformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,27 @@
                  use_auth_token: Union[bool, str, None] = None
                  ):
 
         print("LinkTransformer's custom LinkTransformer class")
 
         super().__init__(model_name_or_path=model_name_or_path, modules=modules, device=device, cache_folder=cache_folder, use_auth_token=use_auth_token)
 
+        ##If it is a local path, we need to load the config (LT) from the file FLAG - CLEAN THIS UP
+        if os.path.isdir(model_name_or_path):
+            ###If config file exists, load it. It will be in the parent folder of the model
+            if os.path.isfile(os.path.join(os.path.dirname(model_name_or_path), 'LT_training_config.json')):
+                with open(os.path.join(os.path.dirname(model_name_or_path), 'LT_training_config.json'), 'r') as fIn:
+                    self._lt_model_config = json.load(fIn)
+                    print("Loaded LinkTransformer model config from {}".format(os.path.join(model_name_or_path, 'LT_training_config.json')))
+                self.base_model_name_or_path = self._lt_model_config['base_model_path']
+        else:
+            ###If huggningface model, then assign ##Implement later
+            self.base_model_name_or_path = model_name_or_path
+
+
 
     def save(self, path: str, model_name: Optional[str] = None, create_model_card: bool = True, train_datasets: Optional[List[str]] = None):
         """
         Saves all elements for this seq. sentence embedder into different sub-folders
         :param path: Path on disc
         :param model_name: Optional model name
         :param create_model_card: If True, create a README.md with basic information about this model
@@ -103,33 +116,32 @@
         """
         if self._model_card_text is not None and len(self._model_card_text) > 0:
             model_card = self._model_card_text
         else:
             tags = ModelCardTemplate.__TAGS__.copy()
             model_card = ModelCardTemplate.__MODEL_CARD__
 
-            if len(self._modules) == 2 and isinstance(self._first_module(), Transformer) and isinstance(self._last_module(), Pooling) and self._last_module().get_pooling_mode_str() in ['cls', 'max', 'mean']:
-                pooling_module = self._last_module()
-                pooling_mode = pooling_module.get_pooling_mode_str()
-                model_card = model_card.replace("{USAGE_TRANSFORMERS_SECTION}", ModelCardTemplate.__USAGE_TRANSFORMERS__)
-                pooling_fct_name, pooling_fct = ModelCardTemplate.model_card_get_pooling_function(pooling_mode)
-                model_card = model_card.replace("{POOLING_FUNCTION}", pooling_fct).replace("{POOLING_FUNCTION_NAME}", pooling_fct_name).replace("{POOLING_MODE}", pooling_mode)
-                tags.append('transformers')
+            # if len(self._modules) == 2 and isinstance(self._first_module(), Transformer) and isinstance(self._last_module(), Pooling) and self._last_module().get_pooling_mode_str() in ['cls', 'max', 'mean']:
+            #     # pooling_fct_name, pooling_fct = ModelCardTemplate.model_card_get_pooling_function(pooling_mode)
+            #     # model_card = model_card.replace("{POOLING_FUNCTION}", pooling_fct).replace("{POOLING_FUNCTION_NAME}", pooling_fct_name).replace("{POOLING_MODE}", pooling_mode)
+            #     tags.append('transformers')
 
             # Print full model
             model_card = model_card.replace("{FULL_MODEL_STR}", str(self))
 
             # Add tags
             model_card = model_card.replace("{TAGS}", "\n".join(["- "+t for t in tags]))
 
             datasets_str = ""
             if train_datasets is not None:
                 datasets_str = "datasets:\n"+"\n".join(["- " + d for d in train_datasets])
             model_card = model_card.replace("{DATASETS}", datasets_str)
 
+            ###Add base model name
+            model_card=model_card.replace("{BASE_MODEL}",self.base_model_name_or_path)
 
             # Add dim info
             self._model_card_vars["{NUM_DIMENSIONS}"] = self.get_sentence_embedding_dimension()
 
             # Replace vars we created while using the model
             for name, value in self._model_card_vars.items():
                 model_card = model_card.replace(name, str(value))
@@ -150,15 +162,15 @@
                     private: Optional[bool] = None,
                     commit_message: str = "Add new LinkTransformer model.",
                     local_model_path: Optional[str] = None,
                     exist_ok: bool = False,
                     replace_model_card: bool = False,
                     train_datasets: Optional[List[str]] = None):
         """
-        Uploads all elements of this LinkTransformer (Sentence Transformer) to a new HuggingFace Hub repository.
+        Uploads all elements of this LinkTransformer (inherited Sentence Transformer) to a new HuggingFace Hub repository.
 
         :param repo_name: Repository name for your model in the Hub.
         :param organization:  Organization in which you want to push your model or tokenizer (you must be a member of this organization).
         :param private: Set to true, for hosting a prive model
         :param commit_message: Message to commit while pushing.
         :param local_model_path: Path of the model locally. If set, this file path will be uploaded. Otherwise, the current model will be uploaded
         :param exist_ok: If true, saving to an existing repository is OK. If false, saving only to a new repository is possible
@@ -199,14 +211,18 @@
             # If user provides local files, copy them.
             if local_model_path:
                 copy_tree(local_model_path, tmp_dir)
             else:  # Else, save model directly into local repo.
                 create_model_card = replace_model_card or not os.path.exists(os.path.join(tmp_dir, 'README.md'))
                 self.save(tmp_dir, model_name=full_model_name, create_model_card=create_model_card, train_datasets=train_datasets)
 
+            ##Save the model config (_lt_model_config) to the repo
+            with open(os.path.join(tmp_dir, 'LT_training_config.json'), 'w') as fOut:
+                json.dump(self._lt_model_config, fOut, indent=2)
+
             #Find files larger 5M and track with git-lfs
             large_files = []
             for root, dirs, files in os.walk(tmp_dir):
                 for filename in files:
                     file_path = os.path.join(root, filename)
                     rel_path = os.path.relpath(file_path, tmp_dir)
```

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/cluster_fns.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/cluster_fns.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/data_loaders.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/data_loaders.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/evaluation.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from sentence_transformers import evaluation, LoggingHandler
 import logging
 from transformers import logging as lg
 import wandb
 from typing import List, Dict, Set, Callable
 from torch import Tensor
 
+from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
+from sklearn.metrics import average_precision_score
+
 currentdir = os.path.dirname(os.path.realpath(__file__))
 parentdir = os.path.dirname(currentdir)
 sys.path.append(parentdir)
 
 from tqdm.autonotebook import trange
 import torch
 import heapq
@@ -393,7 +396,93 @@
             ###save the df as a csv 
             df.to_csv("current_best_matches.csv", index=False,encoding="utf-8")
 
  
         return {'accuracy@k': num_hits_at_k, 'precision@k': precisions_at_k, 'recall@k': recall_at_k, 'ndcg@k': ndcg, 'mrr@k': MRR, 'map@k': AveP_at_k}
 
 
+
+
+class BinaryClassificationEvaluator_wandb(evaluation.BinaryClassificationEvaluator):
+
+
+    def __init__(self, sentences1: List[str], sentences2: List[str], labels: List[int], name: str = '', batch_size: int = 32, show_progress_bar: bool = False, write_csv: bool = True, wandb_names=None):
+        self.sentences1 = sentences1
+        self.sentences2 = sentences2
+        self.labels = labels
+        self.wandb_names = wandb_names
+
+        assert len(self.sentences1) == len(self.sentences2)
+        assert len(self.sentences1) == len(self.labels)
+        for label in labels:
+            assert (label == 0 or label == 1)
+
+        self.write_csv = write_csv
+        self.name = name
+        self.batch_size = batch_size
+        if show_progress_bar is None:
+            show_progress_bar = (logger.getEffectiveLevel() == logging.INFO or logger.getEffectiveLevel() == logging.DEBUG)
+        self.show_progress_bar = show_progress_bar
+
+        self.csv_file = "binary_classification_evaluation" + ("_"+name if name else '') + "_results.csv"
+        self.csv_headers = ["epoch", "steps",
+                            "cossim_accuracy", "cossim_accuracy_threshold", "cossim_f1", "cossim_precision", "cossim_recall", "cossim_f1_threshold", "cossim_ap",
+                            "manhattan_accuracy", "manhattan_accuracy_threshold", "manhattan_f1", "manhattan_precision", "manhattan_recall", "manhattan_f1_threshold", "manhattan_ap",
+                            "euclidean_accuracy", "euclidean_accuracy_threshold", "euclidean_f1", "euclidean_precision", "euclidean_recall", "euclidean_f1_threshold", "euclidean_ap",
+                            "dot_accuracy", "dot_accuracy_threshold", "dot_f1", "dot_precision", "dot_recall", "dot_f1_threshold", "dot_ap"]
+
+
+
+    def compute_metrices(self, model):
+
+        print("*********************EVALUATION STARTED******************************")
+
+        sentences = list(set(self.sentences1 + self.sentences2))
+        embeddings = model.encode(sentences, batch_size=self.batch_size, show_progress_bar=self.show_progress_bar, convert_to_numpy=True)
+        emb_dict = {sent: emb for sent, emb in zip(sentences, embeddings)}
+        embeddings1 = [emb_dict[sent] for sent in self.sentences1]
+        embeddings2 = [emb_dict[sent] for sent in self.sentences2]
+
+        cosine_scores = 1 - paired_cosine_distances(embeddings1, embeddings2)
+        manhattan_distances = paired_manhattan_distances(embeddings1, embeddings2)
+        euclidean_distances = paired_euclidean_distances(embeddings1, embeddings2)
+
+        embeddings1_np = np.asarray(embeddings1)
+        embeddings2_np = np.asarray(embeddings2)
+        dot_scores = [np.dot(embeddings1_np[i], embeddings2_np[i]) for i in range(len(embeddings1_np))]
+
+        labels = np.asarray(self.labels)
+        output_scores = {}
+        for short_name, name, scores, reverse in [['cossim', 'Cosine-Similarity', cosine_scores, True], ['manhattan', 'Manhattan-Distance', manhattan_distances, False], ['euclidean', 'Euclidean-Distance', euclidean_distances, False], ['dot', 'Dot-Product', dot_scores, True]]:
+            # Note: newer versions of sbert have updated the spelling on manhatten to manhattan
+
+            acc, acc_threshold = self.find_best_acc_and_threshold(scores, labels, reverse)
+            f1, precision, recall, f1_threshold = self.find_best_f1_and_threshold(scores, labels, reverse)
+            ap = average_precision_score(labels, scores * (1 if reverse else -1))
+
+            logger.info("Accuracy with {}:           {:.2f}\t(Threshold: {:.4f})".format(name, acc * 100, acc_threshold))
+            logger.info("F1 with {}:                 {:.2f}\t(Threshold: {:.4f})".format(name, f1 * 100, f1_threshold))
+            logger.info("Precision with {}:          {:.2f}".format(name, precision * 100))
+            logger.info("Recall with {}:             {:.2f}".format(name, recall * 100))
+            logger.info("Average Precision with {}:  {:.2f}\n".format(name, ap * 100))
+
+            output_scores[short_name] = {
+                'accuracy': acc,
+                'accuracy_threshold': acc_threshold,
+                'f1': f1,
+                'f1_threshold': f1_threshold,
+                'precision': precision,
+                'recall': recall,
+                'ap': ap
+            }
+            if self.wandb_names:
+                wandb.log({
+                    f"Classification Accuracy {name}": acc,
+                    f"Classification Accuracy threshold {name}": acc_threshold,
+                    f"Classification F1 {name}": f1,
+                    f"Classification F1 threshold {name}": f1_threshold,
+                    f"Classification Precision {name}": precision,
+                    f"Classification Recall {name}": recall,
+                    f"Classification Average precision {name}": ap
+                })
+
+        return output_scores
```

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/losses.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/losses.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.0/src/linktransformer/modified_sbert/train.py` & `linktransformer-0.1.1/src/linktransformer/modified_sbert/train.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,24 +29,27 @@
                     handlers=[LoggingHandler()])
 logger = logging.getLogger(__name__)
 
 
 def train_biencoder(
         train_data: dict = None,
         dev_data: dict = None,
+        test_data: dict = None,
         base_model='colorfulscoop/sbert-base-ja',
         add_pooling_layer=False,
         train_batch_size=64,# The train_batch_size is an argument - you can change it for hard negatives training
         num_epochs=10,
         warm_up_perc=0.1,
         optimizer_params: Dict[str, object] = {'lr': 2e-7},
         loss_params=None,
         model_save_path="output",
         wandb_names=None,
         already_clustered_train=False,
+        eval_steps_perc=0.1,
+        eval_type="retrieval"
 ):
 
     # Logging
     if wandb_names: 
         if 'run' in wandb_names:
             wandb.init(project=wandb_names['project'], entity=wandb_names['id'], reinit=True, name=wandb_names['run'])
         else:
@@ -89,32 +92,61 @@
 
     # Load data as individuals
     ## train_data - You should organize it into cluster fformat
     train_samples = data_loaders.load_data_as_individuals(train_data, type="training",already_clustered=already_clustered_train)
     train_data_sampler = SentenceLabelDataset(train_samples)
     train_dataloader = DataLoader(train_data_sampler, batch_size=train_batch_size)
 
-    queries,corpus,relevant_docs=dev_data
-    evaluators = [evaluation.InformationRetrievalEvaluator_wandb(queries,corpus,relevant_docs,wandb_names=wandb_names)]
+    if eval_type=="retrieval":
+        print("Evaluating on retrieval task")
+        queries,corpus,relevant_docs=dev_data
+        evaluators = [evaluation.InformationRetrievalEvaluator_wandb(queries,corpus,relevant_docs,wandb_names=wandb_names)]
+        seq_evaluator = sentence_transformers.evaluation.SequentialEvaluator(evaluators, main_score_function=lambda scores: scores[-1])
+        ###We also want to evaluate on the test set
+        if test_data is not None:
+            queries,corpus,relevant_docs=test_data
+            test_evaluators = [evaluation.InformationRetrievalEvaluator_wandb(queries,corpus,relevant_docs,wandb_names=wandb_names)]
+            test_evaluator = sentence_transformers.evaluation.SequentialEvaluator(test_evaluators, main_score_function=lambda scores: scores[-1])
+
+    elif eval_type=="classification":
+        print("Evaluating on pair-wise classification task")
+        sentences1, sentences2, labels = dev_data
+        evaluators = [evaluation.BinaryClassificationEvaluator_wandb(sentences1, sentences2, labels,wandb_names=wandb_names)]
+        seq_evaluator = sentence_transformers.evaluation.SequentialEvaluator(evaluators, main_score_function=lambda scores: scores[-1])
+        ###We also want to evaluate on the test set
+        if test_data is not None:
+            sentences1, sentences2, labels = test_data
+            test_evaluators = [evaluation.BinaryClassificationEvaluator_wandb(sentences1, sentences2, labels,wandb_names=wandb_names)]
+            test_evaluator = sentence_transformers.evaluation.SequentialEvaluator(test_evaluators, main_score_function=lambda scores: scores[-1])
+    else:
+        raise ValueError("eval_type can only be either 'retrieval' or 'classification'")
+    
 
-    seq_evaluator = sentence_transformers.evaluation.SequentialEvaluator(evaluators, main_score_function=lambda scores: scores[-1])
 
     logger.info("Evaluate model without training")
     seq_evaluator(model, epoch=0, steps=0, output_path=model_save_path)
 
     # Train the model
     model.fit(
         train_objectives=[(train_dataloader, train_loss)],
         evaluator=seq_evaluator,
         epochs=num_epochs,
         warmup_steps=math.ceil(len(train_dataloader) * num_epochs * warm_up_perc),
         output_path=model_save_path,
-        evaluation_steps= math.ceil(len(train_dataloader)/10),
-        checkpoint_save_steps=math.ceil(len(train_dataloader)/10),
+        evaluation_steps= math.ceil(len(train_dataloader)/eval_steps_perc),
+        checkpoint_save_steps=math.ceil(len(train_dataloader)/eval_steps_perc),
         checkpoint_path=model_save_path,
         save_best_model=True,
         checkpoint_save_total_limit=2,
         optimizer_params = optimizer_params,
     )
 
+    ###Evaluate on the test set using the best model
+    if test_data is not None:
+        logger.info("Evaluating on the test set (0.5 of val data)")
+        ##Load the best model
+        print("Loading best model from:", model_save_path)
+        best_model=LinkTransformer(model_save_path)
+        test_evaluator(best_model, epoch=0, steps=0, output_path=model_save_path)
+
     return model_save_path
```

### Comparing `linktransformer-0.1.0/src/linktransformer/train_model.py` & `linktransformer-0.1.1/src/linktransformer/train_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
-from typing import List
+from typing import List, Union
 from linktransformer.modified_sbert.train import train_biencoder
-from linktransformer.preprocess import prep_linkage_data, preprocess_mexican_tarrif_data
+from linktransformer.preprocess import preprocess_any_data, preprocess_mexican_tarrif_data
 from linktransformer.configs import LINKAGE_CONFIG_PATH
+import pandas as pd
+import pickle
 
 
 def create_new_train_config(base_config_path:str=LINKAGE_CONFIG_PATH,
                             config_save_path:str="myconfig.json",
                             model_save_dir:str=None,
                             model_save_name:str=None,
                             train_batch_size:int=None,
@@ -75,92 +77,132 @@
     return config_save_path
     
     
 
 
 
 def train_model(
+    data: Union[str, pd.DataFrame] = None,
+    train_data: Union[str, pd.DataFrame] = None,
+    val_data: Union[str, pd.DataFrame] = None,
+    test_data: Union[str, pd.DataFrame] = None,
     model_path: str="sentence-transformers/paraphrase-xlm-r-multilingual-v1",
-    dataset_path: str = "data/es_mexican_products.xlsx",
     left_col_names: List[str] = ["description47"],
     right_col_names: List[str] = ['description48'],
     left_id_name: List[str] = ['tariffcode47'],
     right_id_name: List[str] = ['tariffcode48'],
+    label_col_name: str = None,
     config_path: str = LINKAGE_CONFIG_PATH,
     training_args: dict = {"num_epochs":10},
     log_wandb: bool = False,
 ) -> str:
     """
     Train the LinkTransformer model.
 
     :param: model_path (str): The name of the model to use.
-    :param: dataset_path (str): Path to the dataset in Excel format.
+    :param: data (str): Path to the dataset in Excel or CSV format or a dataframe object.
     :param: left_col_names (List[str]): List of column names to use as left side data.
     :param: right_col_names (List[str]): List of column names to use as right side data.
     :param: left_id_name (List[str]): List of column names to use as identifiers for the left data.
-    :param: right_id_name (List[str]): List of column names to use as identifiers for the right data.
+    :param: right_id_name (List[str]): List of column names to use as identifiers for the right data,
+    :param: label_col_name (str): Name of the column to use as labels. Specify this if you have data of the form (left, right, label). This type supports both positive and negative examples.
     :param: config_path (str): Path to the JSON configuration file.
     :param: training_args (dict): Dictionary of training arguments to override the config.
     :param: log_wandb (bool): Whether to log the training run on wandb.
     :return: The path to the saved best model.
     """
-    print(f"Using Training data from {dataset_path}")
 
     # Load the configuration from the JSON file
     with open(config_path, "r") as config_file:
         config = json.load(config_file)
 
     ####Override config using keys that are specified
     if training_args is not None:
         for key in training_args:
             config[key]=training_args[key]
+    
+    ##Make model dir
+    if not os.path.exists(config["model_save_dir"]):
+        os.makedirs(config["model_save_dir"])
+    ##Make dir for this model
+    if not os.path.exists(os.path.join(config["model_save_dir"], config["model_save_name"])):
+        os.makedirs(os.path.join(config["model_save_dir"], config["model_save_name"]))
         
     
     print(f"Loading config saved at {config_path}")
     print(f"Using base model: {model_path}")
 
     print(f"Currently wandb logging is set to {log_wandb}. Your training run can be logged on wandb by setting log_wandb=True , setting approriate parameters in the config and  making an account on wandb if you don't have one yet")
 
+    print("Testing at end: ", config["test_at_end"])
+
     print("loading wiki comp data - would only work with supcon loss")
-    train_data, val_data = prep_linkage_data(
-        dataset_path,
+    train_data, val_data, test_data = preprocess_any_data(
+        data=data,
+        train_data=train_data,
+        val_data=val_data,
+        test_data=test_data,
         left_col_names=left_col_names,
         right_col_names=right_col_names,
         left_id_name=left_id_name,
         right_id_name=right_id_name,
+        label_col_name=label_col_name,
         model=model_path,
-        val_perc=config["val_perc"]
+        val_perc=config["val_perc"],
+        large_val=config["large_val"],
+        test_at_end=config["test_at_end"]
     )
     
+    ##Save val and test pickles
+    if config["save_val_test_pickles"]:
+        print("Saving val and test pickles")
+        with open(os.path.join(config["model_save_dir"], config["model_save_name"], "val_data.pickle"), "wb") as val_file:
+            pickle.dump(val_data, val_file)
+        with open(os.path.join(config["model_save_dir"], config["model_save_name"], "test_data.pickle"), "wb") as test_file:
+            pickle.dump(test_data, test_file)
+
+        print("Saved val and test pickles")
+
+
+    ##If label_col_name is not None, specify that the eval type is classification
+    if label_col_name is not None:
+        config["eval_type"]="classification"
+    else:
+        config["eval_type"]="retrieval"
+
     ##Prep model directories if they don't exist
     if not os.path.exists(config["model_save_dir"]):
         os.makedirs(config["model_save_dir"])
 
     print("Training")
     best_model_path = train_biencoder(
         train_data=train_data,
         dev_data=val_data,
+        test_data=test_data,
         base_model=model_path,
         add_pooling_layer=config["add_pooling_layer"],
         train_batch_size=config["train_batch_size"],
         num_epochs=config["num_epochs"],
         warm_up_perc=config["warm_up_perc"],
         model_save_path=os.path.join(config["model_save_dir"], config["model_save_name"]),
         wandb_names=config["wandb_names"] if log_wandb else None,
-        optimizer_params={'lr': config["learning_rate"]}
+        optimizer_params={'lr': config["learning_rate"]},
+        eval_type=config["eval_type"]
     )
     print(f"Best model saved on the path: {best_model_path} ")
 
     ##Add the dataset used in the config 
-    config["training_dataset"]=dataset_path
+    config["training_dataset"]=data if isinstance(data,str) else "dataframe"
     ##Add the best model path in the config
     config["best_model_path"]=best_model_path
+    config["base_model_path"]=model_path
+
     ##Save the config
     with open(os.path.join(config["model_save_dir"], config["model_save_name"], "LT_training_config.json"), "w") as config_file:
         json.dump(config, config_file)
+        
     
 
     return best_model_path
 
 
 
-
```

### Comparing `linktransformer-0.1.0/src/linktransformer.egg-info/PKG-INFO` & `linktransformer-0.1.1/src/linktransformer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple way to do link dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <llmklinkpython@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 dell-research-harvard
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,32 +55,32 @@
 pip install linktransformer
 ```
 
 ## Getting Started
 
 ```python
 
-from linktransformer import lm_merge_df, dedup
-
+import linktransformer as lt
 # Example usage of lm_merge_df
-merged_df = lm_merge_df(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model')
+merged_df = lt.merge(df1, df2, merge_type='1:1', on='key_column', model='your-pretrained-model-from-huggingface')
 
 # Example usage of dedup
-deduplicated_df = dedup(df, model='your-pretrained-model', on='text_column', threshold=0.8)
+deduplicated_df = lt.dedup_rows(df, model='your-pretrained-model', on='text_column', threshold=0.8)
 ```
 
+All transformer based models from [HuggingFace](https://huggingface.co/) are supported. We recommend [sentence-transformers](https://www.sbert.net/docs/pretrained_models.html) for these tasks as they are trained for semantic similarity tasks. 
 
 ## Usage 
 
 ### Merging Pandas Dataframes
 
-The lm_merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
+The merge function is used to merge two dataframes using language model embeddings. It supports three types of merges: 1:1, 1:m, and m:1. The function takes the following parameters:
 
 ```python
-def lm_merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
+def merge(df1, df2, merge_type='1:1', on=None, model='your-pretrained-model', left_on=None, right_on=None, suffixes=('_x', '_y'),
                  use_gpu=False, batch_size=128, pooling_type='mean', openai_key=None):
     """
     Merge two dataframes using language model embeddings
     :param df1: first dataframe (left) 
     :param df2: second dataframe (right)
     :param merge_type: type of merge to perform 1:m or m:1 or 1:1
     :param model: language model to use
@@ -90,30 +90,66 @@
     :param suffixes: suffixes to use for overlapping columns
     :return: merged dataframe
     """
 
 
 ```
 
-A special case of merging is aggregation - when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, lm_merge_blocking can be used to merge within blocking keys. 
+A special case of merging is aggregation (use function: aggregate_rows)- when the left key is a list of items that need aggregation to the right keys. Semantic linking is also allowed with multiple columns as keys in both datasets. For larger datasets, merge_blocking can be used to merge within blocking keys. 
 
 
-### Deduplicating Data
+### Clustering or Deduplicating Data
 ```python
-def dedup(df, model, on, threshold=0.5, openai_key=None):
+def dedup_rows(df, model, on, threshold=0.5, openai_key=None):
+    """
+    A function to deduplicate a dataframe based on a similarity threshold
+    :param df: dataframe to deduplicate
+    :param model: language model to use
+    :param on: column to deduplicate on
+    :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
+    :return: deduplicated dataframe
+    """
+
+def cluster_rows(df, model, on, threshold=0.5, openai_key=None):
     """
     A function to deduplicate a dataframe based on a similarity threshold
     :param df: dataframe to deduplicate
     :param model: language model to use
     :param on: column to deduplicate on
     :param threshold: similarity threshold for clustering
+    :param openai_key: Open ai key. 
     :return: deduplicated dataframe
     """
+
+```
+
+We allow a simple clustering function to cluster rows based on a key. Deduplication is just keeping only one row per cluster.
+
+
+### Get similarity score between 2 sets of columns
+
+```python
+
+def evaluate_pairs(df,model,left_on,right_on,openai_key=None):
+    """
+    This function evaluates paired columns in a dataframe and gives a match score (cosine similarity). 
+    Typically, this can be though of as a way to evaluate already merged in dataframes.
+
+    :param df (DataFrame): Dataframe to evaluate.
+    :param model (str): Language model to use.
+    :param left_on (Union[str, List[str]]): Column(s) to evaluate on in df.
+    :param right_on (Union[str, List[str]]): Reference column(s) to evaluate on in df.
+    :return: DataFrame: The evaluated dataframe.
+    """
+
+
 ```
 
+
 ### Training your own LinkTransformer model
 
 ```python
 
 
 def train_model(
     model_path: str='your-pretrained-model',
@@ -125,38 +161,40 @@
     config_path: str = LINKAGE_CONFIG_PATH,
     training_args: dict = {"num_epochs":10},
     log_wandb: bool = False,
 ) -> str:
     """
     Train the LinkTransformer model.
 
-    Args:
-        model_path (str): The name of the model to use.
-        dataset_path (str): Path to the dataset in Excel format.
-        left_col_names (List[str]): List of column names to use as left side data.
-        right_col_names (List[str]): List of column names to use as right side data.
-        left_id_name (List[str]): List of column names to use as identifiers for the left data.
-        right_id_name (List[str]): List of column names to use as identifiers for the right data.
-        config_path (str): Path to the JSON configuration file.
-        training_args (dict): Dictionary of training arguments to override the config.
-        log_wandb (bool): Whether to log the training run on wandb.
-
-    Returns:
-        str: The path to the saved best model.
+    :param model_path (str): The name of the model to use.
+    :param dataset_path (str): Path to the dataset in Excel format.
+    :param left_col_names (List[str]): List of column names to use as left side data.
+    :param right_col_names (List[str]): List of column names to use as right side data.
+    :param left_id_name (List[str]): List of column names to use as identifiers for the left data.
+    :param right_id_name (List[str]): List of column names to use as identifiers for the right data.
+    :param config_path (str): Path to the JSON configuration file.
+    :param training_args (dict): Dictionary of training arguments to override the config.
+    :param log_wandb (bool): Whether to log the training run on wandb.
+    :returns: str: The path to the saved best model.
     """
 
 
 ```
 
 
+
+
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvement, please create a new issue or submit a pull request.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
 The sentence-transformers library and HugginFace for providing pre-trained NLP models
 The faiss library for efficient similarity search
 The sklearn and networkx libraries for clustering and graph operations
 OpenAI for providing language model embeddings
 
+
+## Roadmap 
+We will continue to come up with more feature rich updates and introduce more modalities like images using support for vision and multimodal models.
```

### Comparing `linktransformer-0.1.0/src/linktransformer.egg-info/SOURCES.txt` & `linktransformer-0.1.1/src/linktransformer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/linktransformer/data/coarse.csv
 src/linktransformer/data/es_mexican_products.xlsx
 src/linktransformer/data/fine.csv
 src/linktransformer/data/toy_comp_1.csv
 src/linktransformer/data/toy_comp_2.csv
 src/linktransformer/data/toy_multi_1.csv
 src/linktransformer/data/toy_multi_2.csv
+src/linktransformer/data/toy_pairs.csv
 src/linktransformer/data/translation_1.csv
 src/linktransformer/data/translation_2.csv
 src/linktransformer/modified_sbert/LinkTransformer.py
 src/linktransformer/modified_sbert/__init__.py
 src/linktransformer/modified_sbert/cluster_fns.py
 src/linktransformer/modified_sbert/data_loaders.py
 src/linktransformer/modified_sbert/evaluation.py
```

