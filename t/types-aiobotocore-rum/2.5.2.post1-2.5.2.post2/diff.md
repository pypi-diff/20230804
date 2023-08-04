# Comparing `tmp/types-aiobotocore-rum-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rum-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rum-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-rum-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-rum-2.5.2.post1.tar` & `types-aiobotocore-rum-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.221474 types-aiobotocore-rum-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-08-02 14:52:55.221474 types-aiobotocore-rum-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.221474 types-aiobotocore-rum-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.221474 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-02 14:48:16.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-08-02 14:48:16.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-08-02 14:48:16.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-08-02 14:48:16.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:15.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.221474 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:55.000000 types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13418 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11906 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2030 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1455 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1454 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      936 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18059 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18029 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8887 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8885 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5894 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5888 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20184 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20149 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13418 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/LICENSE` & `types-aiobotocore-rum-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post1/PKG-INFO` & `types-aiobotocore-rum-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
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
 [types-aiobotocore-rum docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,102 +303,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rum.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CloudWatchRUM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/literals/).
+
 ```python
-from types_aiobotocore_rum.literals import (
-    BatchGetRumMetricDefinitionsPaginatorName,
-    CustomEventsStatusType,
-    GetAppMonitorDataPaginatorName,
-    ListAppMonitorsPaginatorName,
-    ListRumMetricsDestinationsPaginatorName,
-    MetricDestinationType,
-    StateEnumType,
-    TelemetryType,
-    CloudWatchRUMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rum.literals import BatchGetRumMetricDefinitionsPaginatorName
 
 
 def check_value(value: BatchGetRumMetricDefinitionsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rum.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchRUM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/type_defs/).
+
 ```python
-from types_aiobotocore_rum.type_defs import (
-    AppMonitorConfigurationOutputTypeDef,
-    AppMonitorConfigurationTypeDef,
-    AppMonitorDetailsTypeDef,
-    AppMonitorSummaryTypeDef,
-    CustomEventsTypeDef,
-    MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteRumMetricDefinitionsErrorTypeDef,
-    BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CwLogTypeDef,
-    DeleteAppMonitorRequestRequestTypeDef,
-    DeleteRumMetricsDestinationRequestRequestTypeDef,
-    QueryFilterTypeDef,
-    TimeRangeTypeDef,
-    GetAppMonitorRequestRequestTypeDef,
-    ListAppMonitorsRequestRequestTypeDef,
-    ListRumMetricsDestinationsRequestRequestTypeDef,
-    MetricDestinationSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    MetricDefinitionRequestTypeDef,
-    UserDetailsTypeDef,
-    PutRumMetricsDestinationRequestRequestTypeDef,
-    TimestampTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AppMonitorConfigurationUnionTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
-    BatchCreateRumMetricDefinitionsErrorTypeDef,
-    BatchGetRumMetricDefinitionsResponseTypeDef,
-    CreateAppMonitorResponseTypeDef,
-    GetAppMonitorDataResponseTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    BatchDeleteRumMetricDefinitionsResponseTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    DataStorageTypeDef,
-    GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
-    GetAppMonitorDataRequestRequestTypeDef,
-    ListRumMetricsDestinationsResponseTypeDef,
-    MetricDefinitionRequestUnionTypeDef,
-    UpdateRumMetricDefinitionRequestRequestTypeDef,
-    RumEventTypeDef,
-    BatchCreateRumMetricDefinitionsResponseTypeDef,
-    AppMonitorTypeDef,
-    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    PutRumEventsRequestRequestTypeDef,
-    GetAppMonitorResponseTypeDef,
-)
+from types_aiobotocore_rum.type_defs import AppMonitorConfigurationTypeDef
 
 
-def get_value() -> AppMonitorConfigurationOutputTypeDef:
+def get_value() -> AppMonitorConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/README.md` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-rum
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore rum type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rum"></a>
 
 # types-aiobotocore-rum
 
 [![PyPI - types-aiobotocore-rum](https://img.shields.io/pypi/v/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
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
 [types-aiobotocore-rum docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,102 +303,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rum.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CloudWatchRUM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/literals/).
+
 ```python
-from types_aiobotocore_rum.literals import (
-    BatchGetRumMetricDefinitionsPaginatorName,
-    CustomEventsStatusType,
-    GetAppMonitorDataPaginatorName,
-    ListAppMonitorsPaginatorName,
-    ListRumMetricsDestinationsPaginatorName,
-    MetricDestinationType,
-    StateEnumType,
-    TelemetryType,
-    CloudWatchRUMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rum.literals import BatchGetRumMetricDefinitionsPaginatorName
 
 
 def check_value(value: BatchGetRumMetricDefinitionsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rum.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchRUM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/type_defs/).
+
 ```python
-from types_aiobotocore_rum.type_defs import (
-    AppMonitorConfigurationOutputTypeDef,
-    AppMonitorConfigurationTypeDef,
-    AppMonitorDetailsTypeDef,
-    AppMonitorSummaryTypeDef,
-    CustomEventsTypeDef,
-    MetricDefinitionRequestOutputTypeDef,
-    MetricDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteRumMetricDefinitionsErrorTypeDef,
-    BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CwLogTypeDef,
-    DeleteAppMonitorRequestRequestTypeDef,
-    DeleteRumMetricsDestinationRequestRequestTypeDef,
-    QueryFilterTypeDef,
-    TimeRangeTypeDef,
-    GetAppMonitorRequestRequestTypeDef,
-    ListAppMonitorsRequestRequestTypeDef,
-    ListRumMetricsDestinationsRequestRequestTypeDef,
-    MetricDestinationSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    MetricDefinitionRequestTypeDef,
-    UserDetailsTypeDef,
-    PutRumMetricsDestinationRequestRequestTypeDef,
-    TimestampTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AppMonitorConfigurationUnionTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
-    BatchCreateRumMetricDefinitionsErrorTypeDef,
-    BatchGetRumMetricDefinitionsResponseTypeDef,
-    CreateAppMonitorResponseTypeDef,
-    GetAppMonitorDataResponseTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    BatchDeleteRumMetricDefinitionsResponseTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    DataStorageTypeDef,
-    GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
-    GetAppMonitorDataRequestRequestTypeDef,
-    ListRumMetricsDestinationsResponseTypeDef,
-    MetricDefinitionRequestUnionTypeDef,
-    UpdateRumMetricDefinitionRequestRequestTypeDef,
-    RumEventTypeDef,
-    BatchCreateRumMetricDefinitionsResponseTypeDef,
-    AppMonitorTypeDef,
-    BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    PutRumEventsRequestRequestTypeDef,
-    GetAppMonitorResponseTypeDef,
-)
+from types_aiobotocore_rum.type_defs import AppMonitorConfigurationTypeDef
 
 
-def get_value() -> AppMonitorConfigurationOutputTypeDef:
+def get_value() -> AppMonitorConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/setup.py` & `types-aiobotocore-rum-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rum",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/__init__.py` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/__init__.pyi` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/client.py` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
-    AppMonitorConfigurationUnionTypeDef,
+    AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricDefinitionRequestUnionTypeDef,
+    MetricDefinitionRequestTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -93,15 +93,15 @@
         """
 
     async def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[MetricDefinitionRequestUnionTypeDef],
+        MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -158,15 +158,15 @@
         """
 
     async def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -314,15 +314,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#untag_resource)
         """
 
     async def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -331,15 +331,15 @@
         """
 
     async def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: MetricDefinitionRequestUnionTypeDef,
+        MetricDefinition: MetricDefinitionRequestTypeDef,
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/client.pyi` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 from .paginator import (
     BatchGetRumMetricDefinitionsPaginator,
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 from .type_defs import (
-    AppMonitorConfigurationUnionTypeDef,
+    AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     CustomEventsTypeDef,
     GetAppMonitorDataResponseTypeDef,
     GetAppMonitorResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricDefinitionRequestUnionTypeDef,
+    MetricDefinitionRequestTypeDef,
     QueryFilterTypeDef,
     RumEventTypeDef,
     TimeRangeTypeDef,
     UserDetailsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -88,15 +88,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#exceptions)
         """
     async def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinitions: Sequence[MetricDefinitionRequestUnionTypeDef],
+        MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
         DestinationArn: str = ...
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch RUM
         app monitor to send to a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -148,15 +148,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#close)
         """
     async def create_app_monitor(
         self,
         *,
         Domain: str,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to RUM.
@@ -291,15 +291,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#untag_resource)
         """
     async def update_app_monitor(
         self,
         *,
         Name: str,
-        AppMonitorConfiguration: AppMonitorConfigurationUnionTypeDef = ...,
+        AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
         Domain: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
@@ -307,15 +307,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#update_app_monitor)
         """
     async def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
-        MetricDefinition: MetricDefinitionRequestUnionTypeDef,
+        MetricDefinition: MetricDefinitionRequestTypeDef,
         MetricDefinitionId: str,
         DestinationArn: str = ...
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/literals.py` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginatorName",
     "CustomEventsStatusType",
     "GetAppMonitorDataPaginatorName",
     "ListAppMonitorsPaginatorName",
     "ListRumMetricsDestinationsPaginatorName",
     "MetricDestinationType",
@@ -31,15 +30,14 @@
     "CloudWatchRUMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchGetRumMetricDefinitionsPaginatorName = Literal["batch_get_rum_metric_definitions"]
 CustomEventsStatusType = Literal["DISABLED", "ENABLED"]
 GetAppMonitorDataPaginatorName = Literal["get_app_monitor_data"]
 ListAppMonitorsPaginatorName = Literal["list_app_monitors"]
 ListRumMetricsDestinationsPaginatorName = Literal["list_rum_metrics_destinations"]
 MetricDestinationType = Literal["CloudWatch", "Evidently"]
 StateEnumType = Literal["ACTIVE", "CREATED", "DELETING"]
@@ -56,14 +54,15 @@
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
@@ -159,14 +158,15 @@
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
@@ -245,26 +245,28 @@
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

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/literals.pyi` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.py`

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
     "BatchGetRumMetricDefinitionsPaginatorName",
     "CustomEventsStatusType",
     "GetAppMonitorDataPaginatorName",
     "ListAppMonitorsPaginatorName",
     "ListRumMetricsDestinationsPaginatorName",
     "MetricDestinationType",
@@ -30,14 +31,15 @@
     "CloudWatchRUMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 BatchGetRumMetricDefinitionsPaginatorName = Literal["batch_get_rum_metric_definitions"]
 CustomEventsStatusType = Literal["DISABLED", "ENABLED"]
 GetAppMonitorDataPaginatorName = Literal["get_app_monitor_data"]
 ListAppMonitorsPaginatorName = Literal["list_app_monitors"]
 ListRumMetricsDestinationsPaginatorName = Literal["list_rum_metrics_destinations"]
 MetricDestinationType = Literal["CloudWatch", "Evidently"]
 StateEnumType = Literal["ACTIVE", "CREATED", "DELETING"]
@@ -54,14 +56,15 @@
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
@@ -157,14 +160,15 @@
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
@@ -243,26 +247,28 @@
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

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/paginator.py` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/paginator.pyi` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/type_defs.py` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for rum service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rum.type_defs import AppMonitorConfigurationOutputTypeDef
+    from types_aiobotocore_rum.type_defs import AppMonitorConfigurationTypeDef
 
-    data: AppMonitorConfigurationOutputTypeDef = ...
+    data: AppMonitorConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
@@ -20,20 +20,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
-    "MetricDefinitionRequestOutputTypeDef",
+    "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
     "CwLogTypeDef",
@@ -42,63 +41,44 @@
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MetricDefinitionRequestTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
     "TimestampTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AppMonitorConfigurationUnionTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
+    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
-    "MetricDefinitionRequestUnionTypeDef",
-    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "RumEventTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
-    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
-AppMonitorConfigurationOutputTypeDef = TypedDict(
-    "AppMonitorConfigurationOutputTypeDef",
-    {
-        "AllowCookies": bool,
-        "EnableXRay": bool,
-        "ExcludedPages": List[str],
-        "FavoritePages": List[str],
-        "GuestRoleArn": str,
-        "IdentityPoolId": str,
-        "IncludedPages": List[str],
-        "SessionSampleRate": float,
-        "Telemetries": List[TelemetryType],
-    },
-    total=False,
-)
-
 AppMonitorConfigurationTypeDef = TypedDict(
     "AppMonitorConfigurationTypeDef",
     {
         "AllowCookies": bool,
         "EnableXRay": bool,
         "ExcludedPages": Sequence[str],
         "FavoritePages": Sequence[str],
@@ -137,35 +117,35 @@
     "CustomEventsTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
-_RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestOutputTypeDef",
+_RequiredMetricDefinitionRequestTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalMetricDefinitionRequestOutputTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestOutputTypeDef",
+_OptionalMetricDefinitionRequestTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestTypeDef",
     {
-        "DimensionKeys": Dict[str, str],
+        "DimensionKeys": Mapping[str, str],
         "EventPattern": str,
         "Namespace": str,
         "UnitLabel": str,
         "ValueKey": str,
     },
     total=False,
 )
 
 
-class MetricDefinitionRequestOutputTypeDef(
-    _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
+class MetricDefinitionRequestTypeDef(
+    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
 ):
     pass
 
 
 _RequiredMetricDefinitionTypeDef = TypedDict(
     "_RequiredMetricDefinitionTypeDef",
     {
@@ -388,39 +368,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredMetricDefinitionRequestTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMetricDefinitionRequestTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestTypeDef",
-    {
-        "DimensionKeys": Mapping[str, str],
-        "EventPattern": str,
-        "Namespace": str,
-        "UnitLabel": str,
-        "ValueKey": str,
-    },
-    total=False,
-)
-
-
-class MetricDefinitionRequestTypeDef(
-    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
-):
-    pass
-
-
 UserDetailsTypeDef = TypedDict(
     "UserDetailsTypeDef",
     {
         "sessionId": str,
         "userId": str,
     },
     total=False,
@@ -463,17 +418,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AppMonitorConfigurationUnionTypeDef = Union[
-    AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-]
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -520,18 +472,67 @@
 
 
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
     },
 )
 
+_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinitions": Sequence[MetricDefinitionRequestTypeDef],
+    },
+)
+_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+
+class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
+    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinitionId": str,
+    },
+)
+_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateRumMetricDefinitionRequestRequestTypeDef(
+    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
+    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -696,42 +697,14 @@
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricDefinitionRequestUnionTypeDef = Union[
-    MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
-]
-_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
-        "MetricDefinitionId": str,
-    },
-)
-_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-
-class UpdateRumMetricDefinitionRequestRequestTypeDef(
-    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
-    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": TimestampTypeDef,
         "type": str,
@@ -758,52 +731,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
-        "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
         "Created": str,
         "CustomEvents": CustomEventsTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[MetricDefinitionRequestUnionTypeDef],
-    },
-)
-_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-
-class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
-    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-):
-    pass
-
-
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
         "BatchId": str,
         "Id": str,
         "RumEvents": Sequence[RumEventTypeDef],
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum/type_defs.pyi` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 Type annotations for rum service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rum.type_defs import AppMonitorConfigurationOutputTypeDef
+    from types_aiobotocore_rum.type_defs import AppMonitorConfigurationTypeDef
 
-    data: AppMonitorConfigurationOutputTypeDef = ...
+    data: AppMonitorConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import CustomEventsStatusType, MetricDestinationType, StateEnumType, TelemetryType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
-    "MetricDefinitionRequestOutputTypeDef",
+    "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
     "CwLogTypeDef",
@@ -41,63 +40,44 @@
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MetricDefinitionRequestTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
     "TimestampTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AppMonitorConfigurationUnionTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
+    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
-    "MetricDefinitionRequestUnionTypeDef",
-    "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "RumEventTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
-    "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "GetAppMonitorResponseTypeDef",
 )
 
-AppMonitorConfigurationOutputTypeDef = TypedDict(
-    "AppMonitorConfigurationOutputTypeDef",
-    {
-        "AllowCookies": bool,
-        "EnableXRay": bool,
-        "ExcludedPages": List[str],
-        "FavoritePages": List[str],
-        "GuestRoleArn": str,
-        "IdentityPoolId": str,
-        "IncludedPages": List[str],
-        "SessionSampleRate": float,
-        "Telemetries": List[TelemetryType],
-    },
-    total=False,
-)
-
 AppMonitorConfigurationTypeDef = TypedDict(
     "AppMonitorConfigurationTypeDef",
     {
         "AllowCookies": bool,
         "EnableXRay": bool,
         "ExcludedPages": Sequence[str],
         "FavoritePages": Sequence[str],
@@ -136,34 +116,34 @@
     "CustomEventsTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
-_RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestOutputTypeDef",
+_RequiredMetricDefinitionRequestTypeDef = TypedDict(
+    "_RequiredMetricDefinitionRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalMetricDefinitionRequestOutputTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestOutputTypeDef",
+_OptionalMetricDefinitionRequestTypeDef = TypedDict(
+    "_OptionalMetricDefinitionRequestTypeDef",
     {
-        "DimensionKeys": Dict[str, str],
+        "DimensionKeys": Mapping[str, str],
         "EventPattern": str,
         "Namespace": str,
         "UnitLabel": str,
         "ValueKey": str,
     },
     total=False,
 )
 
-class MetricDefinitionRequestOutputTypeDef(
-    _RequiredMetricDefinitionRequestOutputTypeDef, _OptionalMetricDefinitionRequestOutputTypeDef
+class MetricDefinitionRequestTypeDef(
+    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
 ):
     pass
 
 _RequiredMetricDefinitionTypeDef = TypedDict(
     "_RequiredMetricDefinitionTypeDef",
     {
         "MetricDefinitionId": str,
@@ -373,37 +353,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredMetricDefinitionRequestTypeDef = TypedDict(
-    "_RequiredMetricDefinitionRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMetricDefinitionRequestTypeDef = TypedDict(
-    "_OptionalMetricDefinitionRequestTypeDef",
-    {
-        "DimensionKeys": Mapping[str, str],
-        "EventPattern": str,
-        "Namespace": str,
-        "UnitLabel": str,
-        "ValueKey": str,
-    },
-    total=False,
-)
-
-class MetricDefinitionRequestTypeDef(
-    _RequiredMetricDefinitionRequestTypeDef, _OptionalMetricDefinitionRequestTypeDef
-):
-    pass
-
 UserDetailsTypeDef = TypedDict(
     "UserDetailsTypeDef",
     {
         "sessionId": str,
         "userId": str,
     },
     total=False,
@@ -444,17 +401,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AppMonitorConfigurationUnionTypeDef = Union[
-    AppMonitorConfigurationTypeDef, AppMonitorConfigurationOutputTypeDef
-]
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -497,17 +451,62 @@
     pass
 
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
-        "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
+    },
+)
+
+_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinitions": Sequence[MetricDefinitionRequestTypeDef],
     },
 )
+_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
+    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+        "MetricDefinition": MetricDefinitionRequestTypeDef,
+        "MetricDefinitionId": str,
+    },
+)
+_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+class UpdateRumMetricDefinitionRequestRequestTypeDef(
+    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
+    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
+):
+    pass
 
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -665,40 +664,14 @@
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricDefinitionRequestUnionTypeDef = Union[
-    MetricDefinitionRequestTypeDef, MetricDefinitionRequestOutputTypeDef
-]
-_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinition": MetricDefinitionRequestTypeDef,
-        "MetricDefinitionId": str,
-    },
-)
-_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRumMetricDefinitionRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-class UpdateRumMetricDefinitionRequestRequestTypeDef(
-    _RequiredUpdateRumMetricDefinitionRequestRequestTypeDef,
-    _OptionalUpdateRumMetricDefinitionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": TimestampTypeDef,
         "type": str,
@@ -723,50 +696,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
-        "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
         "Created": str,
         "CustomEvents": CustomEventsTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-        "MetricDefinitions": Sequence[MetricDefinitionRequestUnionTypeDef],
-    },
-)
-_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef",
-    {
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
-class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(
-    _RequiredBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-    _OptionalBatchCreateRumMetricDefinitionsRequestRequestTypeDef,
-):
-    pass
-
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
         "BatchId": str,
         "Id": str,
         "RumEvents": Sequence[RumEventTypeDef],
```

### Comparing `types-aiobotocore-rum-2.5.2.post1/types_aiobotocore_rum.egg-info/SOURCES.txt` & `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

