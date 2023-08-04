# Comparing `tmp/kolena_client-0.80.0.tar.gz` & `tmp/kolena_client-0.80.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.80.0.tar", max compression
+gzip compressed data, was "kolena_client-0.80.1.tar", max compression
```

## Comparing `kolena_client-0.80.0.tar` & `kolena_client-0.80.1.tar`

### file list

```diff
@@ -1,118 +1,122 @@
--rw-r--r--   0        0        0    11346 2023-08-01 21:30:28.006610 kolena_client-0.80.0/LICENSE
--rw-r--r--   0        0        0      556 2023-08-01 21:30:28.006610 kolena_client-0.80.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1993 2023-08-01 21:30:28.006610 kolena_client-0.80.0/README.md
--rw-r--r--   0        0        0     1356 2023-08-01 21:38:48.892593 kolena_client-0.80.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/classification/__init__.py
--rw-r--r--   0        0        0     9888 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/classification/utils.py
--rw-r--r--   0        0        0     1553 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5165 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    18050 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    11891 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    14344 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     7238 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      785 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      921 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/initialize.py
--rw-r--r--   0        0        0     2493 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1150 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     3931 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    23730 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    11006 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      841 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     1910 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/_utils.py
--rw-r--r--   0        0        0     9419 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3032 2023-08-01 21:38:48.892593 kolena_client-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 kolena_client-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-08-04 15:19:56.981036 kolena_client-0.80.1/LICENSE
+-rw-r--r--   0        0        0      556 2023-08-04 15:19:56.981036 kolena_client-0.80.1/LICENSE_HEADER
+-rw-r--r--   0        0        0     1993 2023-08-04 15:19:56.981036 kolena_client-0.80.1/README.md
+-rw-r--r--   0        0        0     1356 2023-08-04 15:28:10.678513 kolena_client-0.80.1/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5880 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/classification/__init__.py
+-rw-r--r--   0        0        0     9888 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/classification/utils.py
+-rw-r--r--   0        0        0     1553 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5165 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    18050 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    11891 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    14344 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     7238 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      674 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/_internal/__init__.py
+-rw-r--r--   0        0        0     1198 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/_internal/datatypes.py
+-rw-r--r--   0        0        0     3015 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/embeddings.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      785 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      955 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     3337 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6825 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1928 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20984 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/initialize.py
+-rw-r--r--   0        0        0     2493 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1150 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3931 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    23730 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    11006 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3032 2023-08-04 15:28:10.678513 kolena_client-0.80.1/pyproject.toml
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 kolena_client-0.80.1/PKG-INFO
```

### Comparing `kolena_client-0.80.0/LICENSE` & `kolena_client-0.80.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/LICENSE_HEADER` & `kolena_client-0.80.1/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/README.md` & `kolena_client-0.80.1/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/__init__.py` & `kolena_client-0.80.1/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/__init__.py` & `kolena_client-0.80.1/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/__init__.py` & `kolena_client-0.80.1/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.80.1/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/client_log.py` & `kolena_client-0.80.1/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/core.py` & `kolena_client-0.80.1/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/detection.py` & `kolena_client-0.80.1/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/fr.py` & `kolena_client-0.80.1/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/generic.py` & `kolena_client-0.80.1/kolena/_api/v1/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,9 +162,22 @@
         aws_role_config: Optional["Workflow.EvaluatorRoleConfig"] = None
 
     @dataclass(frozen=True)
     class ListEvaluatorsResponse:
         evaluators: List["Workflow.EvaluatorResponse"]
 
 
+class Search:
+    class Path(str, Enum):
+        EMBEDDINGS = "/generic/search/embeddings"
+
+    @dataclass(frozen=True)
+    class UploadEmbeddingsRequest(BatchedLoad.WithLoadUUID):
+        ...
+
+    @dataclass(frozen=True)
+    class UploadEmbeddingsResponse:
+        n_samples: int
+
+
 Workflow.EvaluatorResponse.__pydantic_model__.update_forward_refs()
 Workflow.ListEvaluatorsResponse.__pydantic_model__.update_forward_refs()
```

### Comparing `kolena_client-0.80.0/kolena/_api/v1/repository.py` & `kolena_client-0.80.1/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/token.py` & `kolena_client-0.80.1/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_api/v1/workflow.py` & `kolena_client-0.80.1/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/__init__.py` & `kolena_client-0.80.1/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/classification/__init__.py` & `kolena_client-0.80.1/kolena/_experimental/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/classification/utils.py` & `kolena_client-0.80.1/kolena/_experimental/classification/utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_experimental/object_detection/workflow.py` & `kolena_client-0.80.1/kolena/_experimental/object_detection/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_extras/__init__.py` & `kolena_client-0.80.1/kolena/_experimental/search/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_extras/metrics/__init__.py` & `kolena_client-0.80.1/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.80.1/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/__init__.py` & `kolena_client-0.80.1/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.80.1/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/batched_load.py` & `kolena_client-0.80.1/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/cli.py` & `kolena_client-0.80.1/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/consts.py` & `kolena_client-0.80.1/kolena/_utils/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from enum import Enum
 
 
 class BatchSize(int, Enum):
     UPLOAD_CHIPS = 1_000
     UPLOAD_RECORDS = 10_000_000
     UPLOAD_RESULTS = 1_000_000
+    UPLOAD_EMBEDDINGS = 1_000_000
 
     LOAD_RECORDS = UPLOAD_RECORDS
     LOAD_SAMPLES = 1_000_000
 
 
 class FieldName(str, Enum):
     TEST_CASE_NAME = "Test Case name"
```

### Comparing `kolena_client-0.80.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.80.1/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.80.1/kolena/_utils/dataframes/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,19 +54,34 @@
 
 
 # Share Registered check methods for validation
 # https://pandera.readthedocs.io/en/stable/reference/generated/pandera.extensions.html?highlight=register_check_method#pandera.extensions.register_check_method
 
 
 def _is_locator_cell_valid(cell: pa.typing.String) -> bool:
-    matcher = re.compile(r"^(s3|gs|http|https)://(.+/)+.+\.(png|jpe?g|gif|tiff?)$")
+    matcher = re.compile(r"^(s3|gs|https)://(.+/)+.+$")
+    return isinstance(cell, str) and bool(matcher.match(cell.lower()))
+
+
+def _is_image_locator_cell_valid(cell: pa.typing.String) -> bool:
+    matcher = re.compile(r"^(s3|gs|https)://(.+/)+.+\.(png|jpe?g|gif|tiff?)$")
     return isinstance(cell, str) and bool(matcher.match(cell.lower()))
 
 
 @register_check_method(check_type="element_wise")
 def _element_wise_validate_locator(cell: pa.typing.String) -> bool:
     return _is_locator_cell_valid(cell)
 
 
+@register_check_method(check_type="element_wise")
+def _element_wise_validate_image_locator(cell: pa.typing.String) -> bool:
+    return _is_image_locator_cell_valid(cell)
+
+
 @register_check_method()
 def _validate_locator(series: Series) -> bool:
     return series.dropna().apply(_is_locator_cell_valid).all()
+
+
+@register_check_method()
+def _validate_image_locator(series: Series) -> bool:
+    return series.dropna().apply(_is_image_locator_cell_valid).all()
```

### Comparing `kolena_client-0.80.0/kolena/_utils/datatypes.py` & `kolena_client-0.80.1/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/endpoints.py` & `kolena_client-0.80.1/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/frozen.py` & `kolena_client-0.80.1/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/geometry.py` & `kolena_client-0.80.1/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/inference_validators.py` & `kolena_client-0.80.1/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/instrumentation.py` & `kolena_client-0.80.1/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/krequests.py` & `kolena_client-0.80.1/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/log.py` & `kolena_client-0.80.1/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/repository.py` & `kolena_client-0.80.1/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/serde.py` & `kolena_client-0.80.1/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/serializable.py` & `kolena_client-0.80.1/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/state.py` & `kolena_client-0.80.1/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.80.1/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/_utils/validators.py` & `kolena_client-0.80.1/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/__init__.py` & `kolena_client-0.80.1/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/metadata.py` & `kolena_client-0.80.1/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/model.py` & `kolena_client-0.80.1/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.80.1/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.80.1/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.80.1/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.80.1/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.80.1/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/test_case.py` & `kolena_client-0.80.1/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/test_config.py` & `kolena_client-0.80.1/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/test_image.py` & `kolena_client-0.80.1/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/test_run.py` & `kolena_client-0.80.1/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/classification/test_suite.py` & `kolena_client-0.80.1/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/__init__.py` & `kolena_client-0.80.1/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_datatypes.py` & `kolena_client-0.80.1/kolena/detection/_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     return series.dropna().apply(validate_cell).all()
 
 
 JSONObject = object
 
 
 class TestImageDataFrameSchema(pa.SchemaModel):
-    locator: Series[pa.typing.String] = pa.Field(coerce=True, _element_wise_validate_locator=())
+    locator: Series[pa.typing.String] = pa.Field(coerce=True, _element_wise_validate_image_locator=())
     dataset: Series[pa.typing.String] = pa.Field(coerce=True)
     ground_truths: Series[object] = pa.Field(coerce=True, nullable=True, _validate_ground_truths=())
     metadata: Series[JSONObject] = pa.Field(coerce=True)
 
 
 class ImageResultDataFrameSchema(pa.SchemaModel):
     test_run_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
```

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.80.1/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.80.1/kolena/detection/_internal/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from kolena._utils.datatypes import LoadableDataFrame
 
 JSONObject = object
 
 
 class LoadTestImagesDataFrameSchema(pa.SchemaModel):
     test_sample_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
-    locator: Series[pa.typing.String] = pa.Field(coerce=True, _validate_locator=())
+    locator: Series[pa.typing.String] = pa.Field(coerce=True, _validate_image_locator=())
     dataset: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True)
     metadata: Series[JSONObject] = pa.Field(coerce=True)
 
 
 class LoadTestImagesDataFrame(
     pa.typing.DataFrame[LoadTestImagesDataFrameSchema],
     LoadableDataFrame["LoadTestImagesDataFrame"],
```

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.80.1/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/inference.py` & `kolena_client-0.80.1/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.80.1/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/model.py` & `kolena_client-0.80.1/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.80.1/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.80.1/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.80.1/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.80.1/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.80.1/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/ground_truth.py` & `kolena_client-0.80.1/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/inference.py` & `kolena_client-0.80.1/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/metadata.py` & `kolena_client-0.80.1/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/model.py` & `kolena_client-0.80.1/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/test_case.py` & `kolena_client-0.80.1/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/test_config.py` & `kolena_client-0.80.1/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/test_image.py` & `kolena_client-0.80.1/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/test_run.py` & `kolena_client-0.80.1/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/detection/test_suite.py` & `kolena_client-0.80.1/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/errors.py` & `kolena_client-0.80.1/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/__init__.py` & `kolena_client-0.80.1/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/_utils.py` & `kolena_client-0.80.1/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/datatypes.py` & `kolena_client-0.80.1/kolena/fr/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,27 @@
     return json.loads(value) if value is not None else None
 
 
 class TestImageDataFrameSchema(pa.SchemaModel):
     image_id: Series[pa.typing.Int64] = pa.Field(coerce=True)
     """Internal ID corresponding to this image."""
 
-    locator: Series[pa.typing.String] = pa.Field(coerce=True, _validate_locator=())
+    locator: Series[pa.typing.String] = pa.Field(coerce=True, _validate_image_locator=())
     """External locator pointing to image in bucket."""
 
     data_source: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True)
     """Specify source dataset, e.g. "CIFAR-10"."""
 
     width: Series[pa.typing.Int64] = pa.Field(coerce=True, _validate_optional_dimension=())
     """Width of the image, in pixels. The value `-1` is used to specify "unspecified"."""
 
     height: Series[pa.typing.Int64] = pa.Field(coerce=True, _validate_optional_dimension=())
     """Height of the image, in pixels. The value `-1` is used to specify "unspecified"."""
 
-    original_locator: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True, _validate_locator=())
+    original_locator: Series[pa.typing.String] = pa.Field(coerce=True, nullable=True, _validate_image_locator=())
     """Specify that this image is an augmented version of another (registered) image."""
 
     augmentation_spec: Series[JSONObject] = pa.Field(coerce=True, nullable=True, _validate_json_object=())
     """
     Free-form specification describing the augmentation applied to the image, e.g. `{"rotate": 90}`. Should not be
     specified unless original_locator is present.
     """
@@ -201,16 +201,16 @@
     "bounding_box",
     "landmarks",
     "tags",
 ]
 
 
 class TestCaseDataFrameSchema(pa.SchemaModel):
-    locator_a: Series[pa.typing.String] = pa.Field(coerce=True, _validate_locator=())
-    locator_b: Series[pa.typing.String] = pa.Field(coerce=True, _validate_locator=())
+    locator_a: Series[pa.typing.String] = pa.Field(coerce=True, _validate_image_locator=())
+    locator_b: Series[pa.typing.String] = pa.Field(coerce=True, _validate_image_locator=())
     is_same: Series[pa.typing.Bool] = pa.Field(coerce=True)
 
 
 TestCaseRecord = Tuple[str, str, bool]
 TEST_CASE_COLUMNS = ["locator_a", "locator_b", "is_same"]
```

### Comparing `kolena_client-0.80.0/kolena/fr/model.py` & `kolena_client-0.80.1/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/test_case.py` & `kolena_client-0.80.1/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/test_images.py` & `kolena_client-0.80.1/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/test_run.py` & `kolena_client-0.80.1/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/fr/test_suite.py` & `kolena_client-0.80.1/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/initialize.py` & `kolena_client-0.80.1/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/__init__.py` & `kolena_client-0.80.1/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/_datatypes.py` & `kolena_client-0.80.1/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/_validators.py` & `kolena_client-0.80.1/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/annotation.py` & `kolena_client-0.80.1/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/asset.py` & `kolena_client-0.80.1/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/define_workflow.py` & `kolena_client-0.80.1/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/evaluator.py` & `kolena_client-0.80.1/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.80.1/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/ground_truth.py` & `kolena_client-0.80.1/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/inference.py` & `kolena_client-0.80.1/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.80.1/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/metrics/_formula.py` & `kolena_client-0.80.1/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.80.1/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/model.py` & `kolena_client-0.80.1/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/plot.py` & `kolena_client-0.80.1/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/test_case.py` & `kolena_client-0.80.1/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/test_run.py` & `kolena_client-0.80.1/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/test_sample.py` & `kolena_client-0.80.1/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/test_suite.py` & `kolena_client-0.80.1/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/visualization/__init__.py` & `kolena_client-0.80.1/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/visualization/_activation_map.py` & `kolena_client-0.80.1/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/visualization/_utils.py` & `kolena_client-0.80.1/kolena/workflow/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/kolena/workflow/workflow.py` & `kolena_client-0.80.1/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.0/pyproject.toml` & `kolena_client-0.80.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.80.0"  # version is automatically set to latest git tag during release process
+version = "0.80.1"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.80.0/PKG-INFO` & `kolena_client-0.80.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.80.0
+Version: 0.80.1
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.80.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.80.1 Summary: Client for
 Kolena's machine learning testing platform. Home-page: https://kolena.io
 License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering
 Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

