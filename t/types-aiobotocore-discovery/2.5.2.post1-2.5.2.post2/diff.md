# Comparing `tmp/types-aiobotocore-discovery-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-discovery-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-discovery-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-discovery-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:45 2023, max compression
```

## Comparing `types-aiobotocore-discovery-2.5.2.post1.tar` & `types-aiobotocore-discovery-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24585 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-02 14:36:28.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-02 14:36:28.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:45.015862 types-aiobotocore-discovery-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-04 12:00:45.011861 types-aiobotocore-discovery-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:45.015862 types-aiobotocore-discovery-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.995861 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24585 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-04 11:43:49.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-04 11:43:49.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:47.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:45.011861 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:00:44.000000 types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-discovery-2.5.2.post1/LICENSE` & `types-aiobotocore-discovery-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/PKG-INFO` & `types-aiobotocore-discovery-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,131 +309,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_discovery.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ApplicationDiscoveryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/literals/).
+
 ```python
-from types_aiobotocore_discovery.literals import (
-    AgentStatusType,
-    BatchDeleteImportDataErrorCodeType,
-    ConfigurationItemTypeType,
-    ContinuousExportStatusType,
-    DataSourceType,
-    DescribeAgentsPaginatorName,
-    DescribeContinuousExportsPaginatorName,
-    DescribeExportConfigurationsPaginatorName,
-    DescribeExportTasksPaginatorName,
-    DescribeTagsPaginatorName,
-    ExportDataFormatType,
-    ExportStatusType,
-    ImportStatusType,
-    ImportTaskFilterNameType,
-    ListConfigurationsPaginatorName,
-    OfferingClassType,
-    PurchasingOptionType,
-    TenancyType,
-    TermLengthType,
-    orderStringType,
-    ApplicationDiscoveryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_discovery.literals import AgentStatusType
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ApplicationDiscoveryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/type_defs/).
+
 ```python
-from types_aiobotocore_discovery.type_defs import (
-    AgentConfigurationStatusTypeDef,
-    AgentNetworkInfoTypeDef,
-    AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
-    BatchDeleteImportDataErrorTypeDef,
-    BatchDeleteImportDataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ConfigurationTagTypeDef,
-    ContinuousExportDescriptionTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagTypeDef,
-    CustomerAgentInfoTypeDef,
-    CustomerAgentlessCollectorInfoTypeDef,
-    CustomerConnectorInfoTypeDef,
-    CustomerMeCollectorInfoTypeDef,
-    DeleteApplicationsRequestRequestTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeConfigurationsRequestRequestTypeDef,
-    DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestRequestTypeDef,
-    ExportInfoTypeDef,
-    ExportFilterTypeDef,
-    ImportTaskFilterTypeDef,
-    ImportTaskTypeDef,
-    TagFilterTypeDef,
-    DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
-    ReservedInstanceOptionsTypeDef,
-    UsageMetricBasisTypeDef,
-    OrderByElementTypeDef,
-    ListServerNeighborsRequestRequestTypeDef,
-    NeighborConnectionDetailTypeDef,
-    StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    TimestampTypeDef,
-    StartImportTaskRequestRequestTypeDef,
-    StopContinuousExportRequestRequestTypeDef,
-    StopDataCollectionByAgentIdsRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    AgentInfoTypeDef,
-    BatchDeleteImportDataResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    ExportConfigurationsResponseTypeDef,
-    ListConfigurationsResponseTypeDef,
-    StartContinuousExportResponseTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StartExportTaskResponseTypeDef,
-    StopContinuousExportResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
-    DescribeTagsResponseTypeDef,
-    DescribeContinuousExportsResponseTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    DeleteTagsRequestRequestTypeDef,
-    GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestRequestTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
-    DescribeExportConfigurationsResponseTypeDef,
-    DescribeExportTasksResponseTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeExportTasksRequestRequestTypeDef,
-    DescribeImportTasksRequestRequestTypeDef,
-    DescribeImportTasksResponseTypeDef,
-    StartImportTaskResponseTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
-    DescribeTagsRequestRequestTypeDef,
-    Ec2RecommendationsExportPreferencesTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListConfigurationsRequestRequestTypeDef,
-    ListServerNeighborsResponseTypeDef,
-    DescribeAgentsResponseTypeDef,
-    ExportPreferencesTypeDef,
-    StartExportTaskRequestRequestTypeDef,
-)
+from types_aiobotocore_discovery.type_defs import AgentConfigurationStatusTypeDef
 
 
 def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-discovery-2.5.2.post1/README.md` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-discovery
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore discovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,131 +309,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_discovery.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ApplicationDiscoveryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/literals/).
+
 ```python
-from types_aiobotocore_discovery.literals import (
-    AgentStatusType,
-    BatchDeleteImportDataErrorCodeType,
-    ConfigurationItemTypeType,
-    ContinuousExportStatusType,
-    DataSourceType,
-    DescribeAgentsPaginatorName,
-    DescribeContinuousExportsPaginatorName,
-    DescribeExportConfigurationsPaginatorName,
-    DescribeExportTasksPaginatorName,
-    DescribeTagsPaginatorName,
-    ExportDataFormatType,
-    ExportStatusType,
-    ImportStatusType,
-    ImportTaskFilterNameType,
-    ListConfigurationsPaginatorName,
-    OfferingClassType,
-    PurchasingOptionType,
-    TenancyType,
-    TermLengthType,
-    orderStringType,
-    ApplicationDiscoveryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_discovery.literals import AgentStatusType
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ApplicationDiscoveryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/type_defs/).
+
 ```python
-from types_aiobotocore_discovery.type_defs import (
-    AgentConfigurationStatusTypeDef,
-    AgentNetworkInfoTypeDef,
-    AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
-    BatchDeleteImportDataErrorTypeDef,
-    BatchDeleteImportDataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ConfigurationTagTypeDef,
-    ContinuousExportDescriptionTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagTypeDef,
-    CustomerAgentInfoTypeDef,
-    CustomerAgentlessCollectorInfoTypeDef,
-    CustomerConnectorInfoTypeDef,
-    CustomerMeCollectorInfoTypeDef,
-    DeleteApplicationsRequestRequestTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeConfigurationsRequestRequestTypeDef,
-    DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestRequestTypeDef,
-    ExportInfoTypeDef,
-    ExportFilterTypeDef,
-    ImportTaskFilterTypeDef,
-    ImportTaskTypeDef,
-    TagFilterTypeDef,
-    DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
-    ReservedInstanceOptionsTypeDef,
-    UsageMetricBasisTypeDef,
-    OrderByElementTypeDef,
-    ListServerNeighborsRequestRequestTypeDef,
-    NeighborConnectionDetailTypeDef,
-    StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    TimestampTypeDef,
-    StartImportTaskRequestRequestTypeDef,
-    StopContinuousExportRequestRequestTypeDef,
-    StopDataCollectionByAgentIdsRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    AgentInfoTypeDef,
-    BatchDeleteImportDataResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    ExportConfigurationsResponseTypeDef,
-    ListConfigurationsResponseTypeDef,
-    StartContinuousExportResponseTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StartExportTaskResponseTypeDef,
-    StopContinuousExportResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
-    DescribeTagsResponseTypeDef,
-    DescribeContinuousExportsResponseTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    DeleteTagsRequestRequestTypeDef,
-    GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestRequestTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
-    DescribeExportConfigurationsResponseTypeDef,
-    DescribeExportTasksResponseTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeExportTasksRequestRequestTypeDef,
-    DescribeImportTasksRequestRequestTypeDef,
-    DescribeImportTasksResponseTypeDef,
-    StartImportTaskResponseTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
-    DescribeTagsRequestRequestTypeDef,
-    Ec2RecommendationsExportPreferencesTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListConfigurationsRequestRequestTypeDef,
-    ListServerNeighborsResponseTypeDef,
-    DescribeAgentsResponseTypeDef,
-    ExportPreferencesTypeDef,
-    StartExportTaskRequestRequestTypeDef,
-)
+from types_aiobotocore_discovery.type_defs import AgentConfigurationStatusTypeDef
 
 
 def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-discovery-2.5.2.post1/setup.py` & `types-aiobotocore-discovery-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-discovery",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.pyi` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__main__.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.pyi` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.pyi` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.pyi` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.py` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.pyi` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/PKG-INFO` & `types-aiobotocore-discovery-2.5.2.post2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-discovery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore discovery type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,131 +277,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_discovery.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ApplicationDiscoveryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/literals/).
+
 ```python
-from types_aiobotocore_discovery.literals import (
-    AgentStatusType,
-    BatchDeleteImportDataErrorCodeType,
-    ConfigurationItemTypeType,
-    ContinuousExportStatusType,
-    DataSourceType,
-    DescribeAgentsPaginatorName,
-    DescribeContinuousExportsPaginatorName,
-    DescribeExportConfigurationsPaginatorName,
-    DescribeExportTasksPaginatorName,
-    DescribeTagsPaginatorName,
-    ExportDataFormatType,
-    ExportStatusType,
-    ImportStatusType,
-    ImportTaskFilterNameType,
-    ListConfigurationsPaginatorName,
-    OfferingClassType,
-    PurchasingOptionType,
-    TenancyType,
-    TermLengthType,
-    orderStringType,
-    ApplicationDiscoveryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_discovery.literals import AgentStatusType
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ApplicationDiscoveryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/type_defs/).
+
 ```python
-from types_aiobotocore_discovery.type_defs import (
-    AgentConfigurationStatusTypeDef,
-    AgentNetworkInfoTypeDef,
-    AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
-    BatchDeleteImportDataErrorTypeDef,
-    BatchDeleteImportDataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ConfigurationTagTypeDef,
-    ContinuousExportDescriptionTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagTypeDef,
-    CustomerAgentInfoTypeDef,
-    CustomerAgentlessCollectorInfoTypeDef,
-    CustomerConnectorInfoTypeDef,
-    CustomerMeCollectorInfoTypeDef,
-    DeleteApplicationsRequestRequestTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeConfigurationsRequestRequestTypeDef,
-    DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestRequestTypeDef,
-    ExportInfoTypeDef,
-    ExportFilterTypeDef,
-    ImportTaskFilterTypeDef,
-    ImportTaskTypeDef,
-    TagFilterTypeDef,
-    DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
-    ReservedInstanceOptionsTypeDef,
-    UsageMetricBasisTypeDef,
-    OrderByElementTypeDef,
-    ListServerNeighborsRequestRequestTypeDef,
-    NeighborConnectionDetailTypeDef,
-    StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    TimestampTypeDef,
-    StartImportTaskRequestRequestTypeDef,
-    StopContinuousExportRequestRequestTypeDef,
-    StopDataCollectionByAgentIdsRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    AgentInfoTypeDef,
-    BatchDeleteImportDataResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    ExportConfigurationsResponseTypeDef,
-    ListConfigurationsResponseTypeDef,
-    StartContinuousExportResponseTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StartExportTaskResponseTypeDef,
-    StopContinuousExportResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
-    DescribeTagsResponseTypeDef,
-    DescribeContinuousExportsResponseTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    DeleteTagsRequestRequestTypeDef,
-    GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestRequestTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
-    DescribeExportConfigurationsResponseTypeDef,
-    DescribeExportTasksResponseTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeExportTasksRequestRequestTypeDef,
-    DescribeImportTasksRequestRequestTypeDef,
-    DescribeImportTasksResponseTypeDef,
-    StartImportTaskResponseTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
-    DescribeTagsRequestRequestTypeDef,
-    Ec2RecommendationsExportPreferencesTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListConfigurationsRequestRequestTypeDef,
-    ListServerNeighborsResponseTypeDef,
-    DescribeAgentsResponseTypeDef,
-    ExportPreferencesTypeDef,
-    StartExportTaskRequestRequestTypeDef,
-)
+from types_aiobotocore_discovery.type_defs import AgentConfigurationStatusTypeDef
 
 
 def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/SOURCES.txt` & `types-aiobotocore-discovery-2.5.2.post2/types_aiobotocore_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

