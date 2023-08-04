# Comparing `tmp/optuna-integration-3.2.0b0.tar.gz` & `tmp/optuna-integration-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-integration-3.2.0b0.tar", last modified: Thu May 25 06:17:48 2023, max compression
+gzip compressed data, was "optuna-integration-3.3.0.tar", last modified: Fri Aug  4 06:58:58 2023, max compression
```

## Comparing `optuna-integration-3.2.0b0.tar` & `optuna-integration-3.3.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.175664 optuna-integration-3.2.0b0/optuna_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/optuna_integration/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_dump_best_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/chainermn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/skorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/tfkeras.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/optuna_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_chainermn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_skorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_tfkeras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:58.259367 optuna-integration-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-04 06:58:58.259367 optuna-integration-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:58.255367 optuna-integration-3.3.0/optuna_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:58.259367 optuna-integration-3.3.0/optuna_integration/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/_dump_best_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/allennlp/_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/mxnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/tfkeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/optuna_integration/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:58.255367 optuna-integration-3.3.0/optuna_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-04 06:58:58.000000 optuna-integration-3.3.0/optuna_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-04 06:58:58.000000 optuna-integration-3.3.0/optuna_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 06:58:58.000000 optuna-integration-3.3.0/optuna_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-04 06:58:58.000000 optuna-integration-3.3.0/optuna_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 06:58:58.000000 optuna-integration-3.3.0/optuna_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 06:58:58.259367 optuna-integration-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:58:58.259367 optuna-integration-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_mxnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-04 06:58:39.000000 optuna-integration-3.3.0/tests/test_tfkeras.py
```

### Comparing `optuna-integration-3.2.0b0/LICENSE` & `optuna-integration-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/PKG-INFO` & `optuna-integration-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-integration
-Version: 3.2.0b0
+Version: 3.3.0
 Summary: Integration libraries of Optuna.
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -67,14 +67,15 @@
 Optuna-Integration API reference is [here](https://optuna-integration.readthedocs.io/en/stable/reference/index.html).
 
 * [AllenNLP](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#allennlp)  ([example](https://github.com/optuna/optuna-examples/tree/main/allennlp))
 * [Catalyst](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#catalyst)  ([example](https://github.com/optuna/optuna-examples/blob/main/pytorch/catalyst_simple.py))
 * [Chainer](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainer)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py))
 * [ChainerMN](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainermn)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainermn_simple.py))
 * [Keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#keras)  ([example](https://github.com/optuna/optuna-examples/tree/main/keras))
+* [MXNet](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#mxnet)  ([example](https://github.com/optuna/optuna-examples/tree/main/mxnet))
 * [skorch](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#skorch)  ([example](https://github.com/optuna/optuna-examples/tree/main/pytorch/skorch_simple.py))
 * [tf.keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#tensorflow)  ([example](https://github.com/optuna/optuna-examples/tree/main/tfkeras/tfkeras_integration.py))
 
 ## Installation
 
 Optuna-Integration is available at [the Python Package Index](https://pypi.org/project/optuna-integration/) and on [Anaconda Cloud](https://anaconda.org/conda-forge/optuna-integration).
```

### Comparing `optuna-integration-3.2.0b0/README.md` & `optuna-integration-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Optuna-Integration API reference is [here](https://optuna-integration.readthedocs.io/en/stable/reference/index.html).
 
 * [AllenNLP](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#allennlp)  ([example](https://github.com/optuna/optuna-examples/tree/main/allennlp))
 * [Catalyst](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#catalyst)  ([example](https://github.com/optuna/optuna-examples/blob/main/pytorch/catalyst_simple.py))
 * [Chainer](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainer)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py))
 * [ChainerMN](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainermn)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainermn_simple.py))
 * [Keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#keras)  ([example](https://github.com/optuna/optuna-examples/tree/main/keras))
+* [MXNet](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#mxnet)  ([example](https://github.com/optuna/optuna-examples/tree/main/mxnet))
 * [skorch](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#skorch)  ([example](https://github.com/optuna/optuna-examples/tree/main/pytorch/skorch_simple.py))
 * [tf.keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#tensorflow)  ([example](https://github.com/optuna/optuna-examples/tree/main/tfkeras/tfkeras_integration.py))
 
 ## Installation
 
 Optuna-Integration is available at [the Python Package Index](https://pypi.org/project/optuna-integration/) and on [Anaconda Cloud](https://anaconda.org/conda-forge/optuna-integration).
```

### Comparing `optuna-integration-3.2.0b0/optuna_integration/_imports.py` & `optuna-integration-3.3.0/optuna_integration/_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/allennlp/_dump_best_config.py` & `optuna-integration-3.3.0/optuna_integration/allennlp/_dump_best_config.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/allennlp/_executor.py` & `optuna-integration-3.3.0/optuna_integration/allennlp/_executor.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/allennlp/_pruner.py` & `optuna-integration-3.3.0/optuna_integration/allennlp/_pruner.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/allennlp/_variables.py` & `optuna-integration-3.3.0/optuna_integration/allennlp/_variables.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/catalyst.py` & `optuna-integration-3.3.0/optuna_integration/catalyst.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/chainer.py` & `optuna-integration-3.3.0/optuna_integration/chainer.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/chainermn.py` & `optuna-integration-3.3.0/optuna_integration/chainermn.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/keras.py` & `optuna-integration-3.3.0/optuna_integration/keras.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/skorch.py` & `optuna-integration-3.3.0/optuna_integration/skorch.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/tensorflow.py` & `optuna-integration-3.3.0/optuna_integration/tensorflow.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration/tfkeras.py` & `optuna-integration-3.3.0/optuna_integration/tfkeras.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/optuna_integration.egg-info/PKG-INFO` & `optuna-integration-3.3.0/optuna_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-integration
-Version: 3.2.0b0
+Version: 3.3.0
 Summary: Integration libraries of Optuna.
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -67,14 +67,15 @@
 Optuna-Integration API reference is [here](https://optuna-integration.readthedocs.io/en/stable/reference/index.html).
 
 * [AllenNLP](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#allennlp)  ([example](https://github.com/optuna/optuna-examples/tree/main/allennlp))
 * [Catalyst](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#catalyst)  ([example](https://github.com/optuna/optuna-examples/blob/main/pytorch/catalyst_simple.py))
 * [Chainer](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainer)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainer_integration.py))
 * [ChainerMN](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#chainermn)  ([example](https://github.com/optuna/optuna-examples/tree/main/chainer/chainermn_simple.py))
 * [Keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#keras)  ([example](https://github.com/optuna/optuna-examples/tree/main/keras))
+* [MXNet](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#mxnet)  ([example](https://github.com/optuna/optuna-examples/tree/main/mxnet))
 * [skorch](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#skorch)  ([example](https://github.com/optuna/optuna-examples/tree/main/pytorch/skorch_simple.py))
 * [tf.keras](https://optuna-integration.readthedocs.io/en/stable/reference/index.html#tensorflow)  ([example](https://github.com/optuna/optuna-examples/tree/main/tfkeras/tfkeras_integration.py))
 
 ## Installation
 
 Optuna-Integration is available at [the Python Package Index](https://pypi.org/project/optuna-integration/) and on [Anaconda Cloud](https://anaconda.org/conda-forge/optuna-integration).
```

### Comparing `optuna-integration-3.2.0b0/optuna_integration.egg-info/SOURCES.txt` & `optuna-integration-3.3.0/optuna_integration.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 optuna_integration/__init__.py
 optuna_integration/_imports.py
 optuna_integration/catalyst.py
 optuna_integration/chainer.py
 optuna_integration/chainermn.py
 optuna_integration/keras.py
+optuna_integration/mxnet.py
 optuna_integration/skorch.py
 optuna_integration/tensorflow.py
 optuna_integration/tfkeras.py
 optuna_integration/version.py
 optuna_integration.egg-info/PKG-INFO
 optuna_integration.egg-info/SOURCES.txt
 optuna_integration.egg-info/dependency_links.txt
@@ -24,10 +25,11 @@
 optuna_integration/allennlp/_executor.py
 optuna_integration/allennlp/_pruner.py
 optuna_integration/allennlp/_variables.py
 tests/test_catalyst.py
 tests/test_chainer.py
 tests/test_chainermn.py
 tests/test_keras.py
+tests/test_mxnet.py
 tests/test_skorch.py
 tests/test_tensorflow.py
 tests/test_tfkeras.py
```

### Comparing `optuna-integration-3.2.0b0/pyproject.toml` & `optuna-integration-3.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -49,19 +49,20 @@
 ]
 document = [
     "sphinx",
     "sphinx_rtd_theme",
 ]
 all = [
   "allennlp>=2.2.0; python_version<'3.11'",
-  "catalyst>=21.3; python_version<'3.11'",
+  "catalyst",
   "chainer>=5.0.0",
   "mpi4py",
-  "skorch; python_version<'3.11'",
-  "tensorflow; python_version<'3.11'",
+  "mxnet",
+  "skorch",
+  "tensorflow",
 ]
 
 [tool.setuptools.packages.find]
 # where = ["."]
 include = ["optuna_integration*"]
 
 [tool.setuptools.dynamic]
```

### Comparing `optuna-integration-3.2.0b0/tests/test_chainer.py` & `optuna-integration-3.3.0/tests/test_chainer.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0b0/tests/test_chainermn.py` & `optuna-integration-3.3.0/tests/test_chainermn.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,14 @@
     _available = True
 except ImportError:
     _available = False
 
 STORAGE_MODES = ["sqlite"]
 PRUNER_INIT_FUNCS = [lambda: pruners.MedianPruner(), lambda: pruners.SuccessiveHalvingPruner()]
 
-pytestmark = pytest.mark.integration
-
 
 class Func:
     def __init__(self) -> None:
         self.suggested_values: dict[int, dict[str, Any]] = {}
 
     def __call__(self, trial: ChainerMNTrial, comm: "CommunicatorBase") -> float:
         x = trial.suggest_float("x", -10, 10)
```

### Comparing `optuna-integration-3.2.0b0/tests/test_keras.py` & `optuna-integration-3.3.0/tests/test_keras.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from optuna_integration.keras import KerasPruningCallback
 
 
 with try_import():
     from keras import Sequential
     from keras.layers import Dense
 
-pytestmark = pytest.mark.integration
-
 
 @pytest.mark.parametrize("interval, epochs", [(1, 1), (2, 1), (2, 2)])
 def test_keras_pruning_callback(interval: int, epochs: int) -> None:
     def objective(trial: optuna.trial.Trial) -> float:
         model = Sequential()
         model.add(Dense(1, activation="sigmoid", input_dim=20))
         model.compile(optimizer="rmsprop", loss="binary_crossentropy", metrics=["accuracy"])
```

### Comparing `optuna-integration-3.2.0b0/tests/test_skorch.py` & `optuna-integration-3.3.0/tests/test_skorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any
 
 import optuna
 from optuna.testing.pruners import DeterministicPruner
-import pytest
 
 from optuna_integration._imports import try_import
 from optuna_integration.skorch import SkorchPruningCallback
 
 
 with try_import() as _imports:
     import torch
@@ -14,16 +13,14 @@
     from torch.nn import Module
 
     import skorch
 
 if not _imports.is_successful():
     Module = object  # type: ignore # NOQA
 
-pytestmark = pytest.mark.integration
-
 
 class ClassifierModule(Module):
     def __init__(self) -> None:
         super().__init__()
         self.dense0 = nn.Linear(4, 8)
 
     def forward(self, X: "torch.Tensor", **kwargs: Any) -> "torch.Tensor":
```

### Comparing `optuna-integration-3.2.0b0/tests/test_tensorflow.py` & `optuna-integration-3.3.0/tests/test_tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 import math
 import typing
 from unittest.mock import patch
 
 import numpy as np
 import optuna
 from optuna.testing.pruners import DeterministicPruner
-import pytest
 
 from optuna_integration._imports import try_import
 from optuna_integration.tensorflow import TensorFlowPruningHook
 
 
 with try_import():
     import tensorflow as tf
 
-pytestmark = pytest.mark.integration
-
 
 def fixed_value_input_fn() -> typing.Tuple[typing.Dict[str, "tf.Tensor"], "tf.Tensor"]:
     x_train = np.zeros([16, 20])
     y_train = np.zeros(16)
     dataset = tf.data.Dataset.from_tensor_slices((x_train, y_train))
     dataset = dataset.repeat().batch(8)
     iterator = tf.compat.v1.data.make_one_shot_iterator(dataset)
```

### Comparing `optuna-integration-3.2.0b0/tests/test_tfkeras.py` & `optuna-integration-3.3.0/tests/test_tfkeras.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from optuna_integration._imports import try_import
 from optuna_integration.tfkeras import TFKerasPruningCallback
 
 
 with try_import():
     import tensorflow as tf
 
-pytestmark = pytest.mark.integration
-
 
 def test_tfkeras_pruning_callback() -> None:
     def objective(trial: optuna.trial.Trial) -> float:
         model = tf.keras.Sequential()
         model.add(tf.keras.layers.Dense(1, activation="sigmoid", input_dim=20))
         model.compile(optimizer="rmsprop", loss="binary_crossentropy", metrics=["accuracy"])
```

