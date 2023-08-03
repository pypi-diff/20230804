# Comparing `tmp/sotai-0.3.2.tar.gz` & `tmp/sotai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotai-0.3.2.tar", last modified: Sat Jul 29 01:10:59 2023, max compression
+gzip compressed data, was "sotai-0.4.0.tar", last modified: Thu Aug  3 23:26:55 2023, max compression
```

## Comparing `sotai-0.3.2.tar` & `sotai-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 01:10:42.000000 sotai-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 01:10:59.257522 sotai-0.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.253522 sotai-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 01:10:42.000000 sotai-0.3.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-29 01:10:42.000000 sotai-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 01:10:59.257522 sotai-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26347 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/trained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-29 01:10:42.000000 sotai-0.3.2/sotai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/sotai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 01:10:59.000000 sotai-0.3.2/sotai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:10:59.257522 sotai-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-29 01:10:42.000000 sotai-0.3.2/tests/test_trained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.534155 sotai-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-03 23:26:44.000000 sotai-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-03 23:26:55.534155 sotai-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.530155 sotai-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-03 23:26:44.000000 sotai-0.4.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-03 23:26:44.000000 sotai-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:26:55.534155 sotai-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.534155 sotai-0.4.0/sotai/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.534155 sotai-0.4.0/sotai/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-08-03 23:26:44.000000 sotai-0.4.0/sotai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.534155 sotai-0.4.0/sotai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-03 23:26:55.000000 sotai-0.4.0/sotai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 23:26:55.000000 sotai-0.4.0/sotai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:26:55.000000 sotai-0.4.0/sotai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 23:26:55.000000 sotai-0.4.0/sotai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 23:26:55.000000 sotai-0.4.0/sotai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:26:55.534155 sotai-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-03 23:26:44.000000 sotai-0.4.0/tests/test_trained_model.py
```

### Comparing `sotai-0.3.2/LICENSE` & `sotai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/PKG-INFO` & `sotai-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.2/docs/README.md` & `sotai-0.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/pyproject.toml` & `sotai-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sotai"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release. Use Semantic Versioning.
-version = "0.3.2"
+version = "0.4.0"
 description = "A Python Library For Calibrated Modeling Built With PyTorch"
 readme = "docs/README.md"
 license = {text = "MIT"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `sotai-0.3.2/sotai/api.py` & `sotai-0.4.0/sotai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     training_results = trained_model.training_results
     train_primary_metrics = training_results.train_primary_metric_by_epoch
     val_primary_metrics = training_results.val_primary_metric_by_epoch
     overall_model_results_dict = {
         "epochs": trained_model.training_config.epochs,
         "batch_size": trained_model.training_config.batch_size,
         "learning_rate": trained_model.training_config.learning_rate,
-        "runtime_in_seconds": training_results.training_time,
+        "runtime_in_seconds": round(training_results.training_time),
         "train_loss_per_epoch": training_results.train_loss_by_epoch,
         "train_primary_metric_per_epoch": train_primary_metrics,
         "validation_loss_per_epoch": training_results.val_loss_by_epoch,
         "validation_primary_metric_per_epoch": val_primary_metrics,
         "test_loss": training_results.test_loss,
         "test_primary_metric": training_results.test_primary_metric,
         "feature_names": [
```

### Comparing `sotai-0.3.2/sotai/data.py` & `sotai-0.4.0/sotai/data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/enums.py` & `sotai-0.4.0/sotai/enums.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/features.py` & `sotai-0.4.0/sotai/features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/layers/categorical_calibrator.py` & `sotai-0.4.0/sotai/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/layers/linear.py` & `sotai-0.4.0/sotai/layers/linear.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/layers/numerical_calibrator.py` & `sotai-0.4.0/sotai/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/models.py` & `sotai-0.4.0/sotai/models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/pipeline.py` & `sotai-0.4.0/sotai/pipeline.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/trained_model.py` & `sotai-0.4.0/sotai/trained_model.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai/training.py` & `sotai-0.4.0/sotai/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
 import torchmetrics
 from pydantic import BaseModel
+from tqdm import trange
 
 from .constants import MISSING_CATEGORY_VALUE, MISSING_NUMERICAL_VALUE
 from .data import CSVData
 from .enums import FeatureType, LossType, Metric
 from .features import CategoricalFeature, NumericalFeature
 from .models import CalibratedLinear
 from .types import (
@@ -132,15 +133,15 @@
     train_loss_by_epoch = []
     train_primary_metric_by_epoch = []
     val_loss_by_epoch = []
     val_primary_metric_by_epoch = []
     train_csv_data.prepare(features, target)
     val_csv_data.prepare(features, target)
     val_examples, val_targets = list(val_csv_data.batch(val_csv_data.num_examples))[0]
-    for _ in range(training_config.epochs):
+    for _ in trange(training_config.epochs, desc="Training Progress"):
         train_prediction_tensors = []
         train_target_tensors = []
         for example_batch, target_batch in train_csv_data.batch(
             training_config.batch_size
         ):
             optimizer.zero_grad()
             outputs = model(example_batch)
```

### Comparing `sotai-0.3.2/sotai/types.py` & `sotai-0.4.0/sotai/types.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/sotai.egg-info/PKG-INFO` & `sotai-0.4.0/sotai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotai
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python Library For Calibrated Modeling Built With PyTorch
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: MIT
 Project-URL: Source, https://github.com/SOTAI-Labs/sotai
 Project-URL: Documentation, https://github.com/SOTAI-Labs/sotai/tree/main/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

### Comparing `sotai-0.3.2/sotai.egg-info/SOURCES.txt` & `sotai-0.4.0/sotai.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 pyproject.toml
 docs/README.md
 sotai/__init__.py
 sotai/api.py
 sotai/constants.py
 sotai/data.py
+sotai/demo.py
 sotai/enums.py
 sotai/features.py
 sotai/models.py
 sotai/pipeline.py
 sotai/trained_model.py
 sotai/training.py
 sotai/types.py
```

### Comparing `sotai-0.3.2/tests/test_api.py` & `sotai-0.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/tests/test_data.py` & `sotai-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/tests/test_features.py` & `sotai-0.4.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/tests/test_models.py` & `sotai-0.4.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/tests/test_pipeline.py` & `sotai-0.4.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `sotai-0.3.2/tests/test_trained_model.py` & `sotai-0.4.0/tests/test_trained_model.py`

 * *Files identical despite different names*

