# Comparing `tmp/types-aiobotocore-machinelearning-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-machinelearning-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-machinelearning-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-machinelearning-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-machinelearning-2.5.2.post1.tar` & `types-aiobotocore-machinelearning-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18695 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31653 2023-08-02 14:42:41.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-08-02 14:42:41.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18695 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15096 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13546 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2128 2023-08-04 13:43:35.000000 types-aiobotocore-machinelearning-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2294 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2293 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      975 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28039 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27994 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10382 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10380 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6983 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6977 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31653 2023-08-04 13:43:38.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31628 2023-08-04 13:43:38.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6335 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6331 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15096 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1054 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/LICENSE` & `types-aiobotocore-machinelearning-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/PKG-INFO` & `types-aiobotocore-machinelearning-2.5.2.post2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,142 +342,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_machinelearning.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `MachineLearning` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/literals/).
+
 ```python
-from types_aiobotocore_machinelearning.literals import (
-    AlgorithmType,
-    BatchPredictionAvailableWaiterName,
-    BatchPredictionFilterVariableType,
-    DataSourceAvailableWaiterName,
-    DataSourceFilterVariableType,
-    DescribeBatchPredictionsPaginatorName,
-    DescribeDataSourcesPaginatorName,
-    DescribeEvaluationsPaginatorName,
-    DescribeMLModelsPaginatorName,
-    DetailsAttributesType,
-    EntityStatusType,
-    EvaluationAvailableWaiterName,
-    EvaluationFilterVariableType,
-    MLModelAvailableWaiterName,
-    MLModelFilterVariableType,
-    MLModelTypeType,
-    RealtimeEndpointStatusType,
-    SortOrderType,
-    TaggableResourceTypeType,
-    MachineLearningServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_machinelearning.literals import AlgorithmType
 
 
 def check_value(value: AlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_machinelearning.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MachineLearning` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/type_defs/).
+
 ```python
-from types_aiobotocore_machinelearning.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    BatchPredictionTypeDef,
-    CreateBatchPredictionInputRequestTypeDef,
-    S3DataSpecTypeDef,
-    CreateEvaluationInputRequestTypeDef,
-    CreateMLModelInputRequestTypeDef,
-    CreateRealtimeEndpointInputRequestTypeDef,
-    RealtimeEndpointInfoTypeDef,
-    DeleteBatchPredictionInputRequestTypeDef,
-    DeleteDataSourceInputRequestTypeDef,
-    DeleteEvaluationInputRequestTypeDef,
-    DeleteMLModelInputRequestTypeDef,
-    DeleteRealtimeEndpointInputRequestTypeDef,
-    DeleteTagsInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputRequestTypeDef,
-    DescribeTagsInputRequestTypeDef,
-    PerformanceMetricsTypeDef,
-    GetBatchPredictionInputRequestTypeDef,
-    GetDataSourceInputRequestTypeDef,
-    GetEvaluationInputRequestTypeDef,
-    GetMLModelInputRequestTypeDef,
-    PredictInputRequestTypeDef,
-    PredictionTypeDef,
-    RDSDatabaseCredentialsTypeDef,
-    RDSDatabaseTypeDef,
-    RedshiftDatabaseCredentialsTypeDef,
-    RedshiftDatabaseTypeDef,
-    UpdateBatchPredictionInputRequestTypeDef,
-    UpdateDataSourceInputRequestTypeDef,
-    UpdateEvaluationInputRequestTypeDef,
-    UpdateMLModelInputRequestTypeDef,
-    AddTagsInputRequestTypeDef,
-    AddTagsOutputTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
-    CreateEvaluationOutputTypeDef,
-    CreateMLModelOutputTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
-    DeleteDataSourceOutputTypeDef,
-    DeleteEvaluationOutputTypeDef,
-    DeleteMLModelOutputTypeDef,
-    DeleteTagsOutputTypeDef,
-    DescribeTagsOutputTypeDef,
-    GetBatchPredictionOutputTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
-    UpdateDataSourceOutputTypeDef,
-    UpdateEvaluationOutputTypeDef,
-    UpdateMLModelOutputTypeDef,
-    DescribeBatchPredictionsOutputTypeDef,
-    CreateDataSourceFromS3InputRequestTypeDef,
-    CreateRealtimeEndpointOutputTypeDef,
-    DeleteRealtimeEndpointOutputTypeDef,
-    GetMLModelOutputTypeDef,
-    MLModelTypeDef,
-    DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
-    DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
-    DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
-    DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
-    EvaluationTypeDef,
-    GetEvaluationOutputTypeDef,
-    PredictOutputTypeDef,
-    RDSDataSpecTypeDef,
-    RDSMetadataTypeDef,
-    RedshiftDataSpecTypeDef,
-    RedshiftMetadataTypeDef,
-    DescribeMLModelsOutputTypeDef,
-    DescribeEvaluationsOutputTypeDef,
-    CreateDataSourceFromRDSInputRequestTypeDef,
-    CreateDataSourceFromRedshiftInputRequestTypeDef,
-    DataSourceTypeDef,
-    GetDataSourceOutputTypeDef,
-    DescribeDataSourcesOutputTypeDef,
-)
+from types_aiobotocore_machinelearning.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/README.md` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-machinelearning
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore machinelearning type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,142 +342,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_machinelearning.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `MachineLearning` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/literals/).
+
 ```python
-from types_aiobotocore_machinelearning.literals import (
-    AlgorithmType,
-    BatchPredictionAvailableWaiterName,
-    BatchPredictionFilterVariableType,
-    DataSourceAvailableWaiterName,
-    DataSourceFilterVariableType,
-    DescribeBatchPredictionsPaginatorName,
-    DescribeDataSourcesPaginatorName,
-    DescribeEvaluationsPaginatorName,
-    DescribeMLModelsPaginatorName,
-    DetailsAttributesType,
-    EntityStatusType,
-    EvaluationAvailableWaiterName,
-    EvaluationFilterVariableType,
-    MLModelAvailableWaiterName,
-    MLModelFilterVariableType,
-    MLModelTypeType,
-    RealtimeEndpointStatusType,
-    SortOrderType,
-    TaggableResourceTypeType,
-    MachineLearningServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_machinelearning.literals import AlgorithmType
 
 
 def check_value(value: AlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_machinelearning.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MachineLearning` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/type_defs/).
+
 ```python
-from types_aiobotocore_machinelearning.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    BatchPredictionTypeDef,
-    CreateBatchPredictionInputRequestTypeDef,
-    S3DataSpecTypeDef,
-    CreateEvaluationInputRequestTypeDef,
-    CreateMLModelInputRequestTypeDef,
-    CreateRealtimeEndpointInputRequestTypeDef,
-    RealtimeEndpointInfoTypeDef,
-    DeleteBatchPredictionInputRequestTypeDef,
-    DeleteDataSourceInputRequestTypeDef,
-    DeleteEvaluationInputRequestTypeDef,
-    DeleteMLModelInputRequestTypeDef,
-    DeleteRealtimeEndpointInputRequestTypeDef,
-    DeleteTagsInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputRequestTypeDef,
-    DescribeTagsInputRequestTypeDef,
-    PerformanceMetricsTypeDef,
-    GetBatchPredictionInputRequestTypeDef,
-    GetDataSourceInputRequestTypeDef,
-    GetEvaluationInputRequestTypeDef,
-    GetMLModelInputRequestTypeDef,
-    PredictInputRequestTypeDef,
-    PredictionTypeDef,
-    RDSDatabaseCredentialsTypeDef,
-    RDSDatabaseTypeDef,
-    RedshiftDatabaseCredentialsTypeDef,
-    RedshiftDatabaseTypeDef,
-    UpdateBatchPredictionInputRequestTypeDef,
-    UpdateDataSourceInputRequestTypeDef,
-    UpdateEvaluationInputRequestTypeDef,
-    UpdateMLModelInputRequestTypeDef,
-    AddTagsInputRequestTypeDef,
-    AddTagsOutputTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
-    CreateEvaluationOutputTypeDef,
-    CreateMLModelOutputTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
-    DeleteDataSourceOutputTypeDef,
-    DeleteEvaluationOutputTypeDef,
-    DeleteMLModelOutputTypeDef,
-    DeleteTagsOutputTypeDef,
-    DescribeTagsOutputTypeDef,
-    GetBatchPredictionOutputTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
-    UpdateDataSourceOutputTypeDef,
-    UpdateEvaluationOutputTypeDef,
-    UpdateMLModelOutputTypeDef,
-    DescribeBatchPredictionsOutputTypeDef,
-    CreateDataSourceFromS3InputRequestTypeDef,
-    CreateRealtimeEndpointOutputTypeDef,
-    DeleteRealtimeEndpointOutputTypeDef,
-    GetMLModelOutputTypeDef,
-    MLModelTypeDef,
-    DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
-    DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
-    DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
-    DescribeMLModelsInputMLModelAvailableWaitTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
-    EvaluationTypeDef,
-    GetEvaluationOutputTypeDef,
-    PredictOutputTypeDef,
-    RDSDataSpecTypeDef,
-    RDSMetadataTypeDef,
-    RedshiftDataSpecTypeDef,
-    RedshiftMetadataTypeDef,
-    DescribeMLModelsOutputTypeDef,
-    DescribeEvaluationsOutputTypeDef,
-    CreateDataSourceFromRDSInputRequestTypeDef,
-    CreateDataSourceFromRedshiftInputRequestTypeDef,
-    DataSourceTypeDef,
-    GetDataSourceOutputTypeDef,
-    DescribeDataSourcesOutputTypeDef,
-)
+from types_aiobotocore_machinelearning.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/setup.py` & `types-aiobotocore-machinelearning-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-machinelearning",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__main__.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MachineLearning 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlgorithmType",
     "BatchPredictionAvailableWaiterName",
     "BatchPredictionFilterVariableType",
     "DataSourceAvailableWaiterName",
     "DataSourceFilterVariableType",
     "DescribeBatchPredictionsPaginatorName",
@@ -43,15 +42,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlgorithmType = Literal["sgd"]
 BatchPredictionAvailableWaiterName = Literal["batch_prediction_available"]
 BatchPredictionFilterVariableType = Literal[
     "CreatedAt",
     "DataSourceId",
     "DataURI",
     "IAMUser",
@@ -110,14 +108,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -213,14 +212,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -299,26 +299,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AlgorithmType",
     "BatchPredictionAvailableWaiterName",
     "BatchPredictionFilterVariableType",
     "DataSourceAvailableWaiterName",
     "DataSourceFilterVariableType",
     "DescribeBatchPredictionsPaginatorName",
@@ -42,14 +43,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AlgorithmType = Literal["sgd"]
 BatchPredictionAvailableWaiterName = Literal["batch_prediction_available"]
 BatchPredictionFilterVariableType = Literal[
     "CreatedAt",
     "DataSourceId",
     "DataURI",
     "IAMUser",
@@ -108,14 +110,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -211,14 +214,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -297,26 +301,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.py` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.pyi` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt` & `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

