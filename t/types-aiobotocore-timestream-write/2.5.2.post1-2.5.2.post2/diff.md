# Comparing `tmp/types-aiobotocore-timestream-write-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-timestream-write-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-write-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-write-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-timestream-write-2.5.2.post1.tar` & `types-aiobotocore-timestream-write-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.069438 types-aiobotocore-timestream-write-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:07.069438 types-aiobotocore-timestream-write-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-08-02 14:50:36.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23903 2023-08-02 14:50:36.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.826643 types-aiobotocore-timestream-write-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12684 2023-08-04 13:59:28.826643 types-aiobotocore-timestream-write-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11131 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.826643 types-aiobotocore-timestream-write-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2134 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.806643 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      509 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      508 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      977 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16894 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16867 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8851 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8849 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21327 2023-08-04 13:55:06.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21296 2023-08-04 13:55:06.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:05.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.826643 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12684 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/LICENSE` & `types-aiobotocore-timestream-write-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/PKG-INFO` & `types-aiobotocore-timestream-write-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-write
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,117 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_timestream_write.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `TimestreamWrite` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/literals/).
+
 ```python
-from types_aiobotocore_timestream_write.literals import (
-    BatchLoadDataFormatType,
-    BatchLoadStatusType,
-    DimensionValueTypeType,
-    MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
-    S3EncryptionOptionType,
-    ScalarMeasureValueTypeType,
-    TableStatusType,
-    TimeUnitType,
-    TimestreamWriteServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_timestream_write.literals import BatchLoadDataFormatType
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_timestream_write.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `TimestreamWrite` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/type_defs/).
+
 ```python
-from types_aiobotocore_timestream_write.type_defs import (
-    BatchLoadProgressReportTypeDef,
-    BatchLoadTaskTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DatabaseTypeDef,
-    RetentionPropertiesTypeDef,
-    CsvConfigurationTypeDef,
-    DataModelS3ConfigurationTypeDef,
-    DimensionMappingTypeDef,
-    DataSourceS3ConfigurationTypeDef,
-    DeleteDatabaseRequestRequestTypeDef,
-    DeleteTableRequestRequestTypeDef,
-    DescribeBatchLoadTaskRequestRequestTypeDef,
-    DescribeDatabaseRequestRequestTypeDef,
-    EndpointTypeDef,
-    DescribeTableRequestRequestTypeDef,
-    DimensionTypeDef,
-    ListBatchLoadTasksRequestRequestTypeDef,
-    ListDatabasesRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3ConfigurationTypeDef,
-    MeasureValueTypeDef,
-    MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyTypeDef,
-    RecordsIngestedTypeDef,
-    ReportS3ConfigurationTypeDef,
-    ResumeBatchLoadTaskRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDatabaseRequestRequestTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBatchLoadTasksResponseTypeDef,
-    CreateDatabaseRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateDatabaseResponseTypeDef,
-    DescribeDatabaseResponseTypeDef,
-    ListDatabasesResponseTypeDef,
-    UpdateDatabaseResponseTypeDef,
-    DataSourceConfigurationTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    MagneticStoreRejectedDataLocationTypeDef,
-    RecordTypeDef,
-    MixedMeasureMappingOutputTypeDef,
-    MixedMeasureMappingTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
-    MultiMeasureMappingsTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
-    WriteRecordsResponseTypeDef,
-    ReportConfigurationTypeDef,
-    MagneticStoreWritePropertiesTypeDef,
-    WriteRecordsRequestRequestTypeDef,
-    DataModelOutputTypeDef,
-    DataModelTypeDef,
-    SchemaUnionTypeDef,
-    CreateTableRequestRequestTypeDef,
-    TableTypeDef,
-    UpdateTableRequestRequestTypeDef,
-    DataModelConfigurationOutputTypeDef,
-    DataModelConfigurationTypeDef,
-    CreateTableResponseTypeDef,
-    DescribeTableResponseTypeDef,
-    ListTablesResponseTypeDef,
-    UpdateTableResponseTypeDef,
-    BatchLoadTaskDescriptionTypeDef,
-    CreateBatchLoadTaskRequestRequestTypeDef,
-    DataModelConfigurationUnionTypeDef,
-    DescribeBatchLoadTaskResponseTypeDef,
-)
+from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
 
 def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/README.md` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-timestream-write
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore timestream-write type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,117 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_timestream_write.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `TimestreamWrite` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/literals/).
+
 ```python
-from types_aiobotocore_timestream_write.literals import (
-    BatchLoadDataFormatType,
-    BatchLoadStatusType,
-    DimensionValueTypeType,
-    MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
-    S3EncryptionOptionType,
-    ScalarMeasureValueTypeType,
-    TableStatusType,
-    TimeUnitType,
-    TimestreamWriteServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_timestream_write.literals import BatchLoadDataFormatType
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_timestream_write.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `TimestreamWrite` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/type_defs/).
+
 ```python
-from types_aiobotocore_timestream_write.type_defs import (
-    BatchLoadProgressReportTypeDef,
-    BatchLoadTaskTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DatabaseTypeDef,
-    RetentionPropertiesTypeDef,
-    CsvConfigurationTypeDef,
-    DataModelS3ConfigurationTypeDef,
-    DimensionMappingTypeDef,
-    DataSourceS3ConfigurationTypeDef,
-    DeleteDatabaseRequestRequestTypeDef,
-    DeleteTableRequestRequestTypeDef,
-    DescribeBatchLoadTaskRequestRequestTypeDef,
-    DescribeDatabaseRequestRequestTypeDef,
-    EndpointTypeDef,
-    DescribeTableRequestRequestTypeDef,
-    DimensionTypeDef,
-    ListBatchLoadTasksRequestRequestTypeDef,
-    ListDatabasesRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3ConfigurationTypeDef,
-    MeasureValueTypeDef,
-    MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyTypeDef,
-    RecordsIngestedTypeDef,
-    ReportS3ConfigurationTypeDef,
-    ResumeBatchLoadTaskRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDatabaseRequestRequestTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBatchLoadTasksResponseTypeDef,
-    CreateDatabaseRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateDatabaseResponseTypeDef,
-    DescribeDatabaseResponseTypeDef,
-    ListDatabasesResponseTypeDef,
-    UpdateDatabaseResponseTypeDef,
-    DataSourceConfigurationTypeDef,
-    DescribeEndpointsResponseTypeDef,
-    MagneticStoreRejectedDataLocationTypeDef,
-    RecordTypeDef,
-    MixedMeasureMappingOutputTypeDef,
-    MixedMeasureMappingTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
-    MultiMeasureMappingsTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
-    WriteRecordsResponseTypeDef,
-    ReportConfigurationTypeDef,
-    MagneticStoreWritePropertiesTypeDef,
-    WriteRecordsRequestRequestTypeDef,
-    DataModelOutputTypeDef,
-    DataModelTypeDef,
-    SchemaUnionTypeDef,
-    CreateTableRequestRequestTypeDef,
-    TableTypeDef,
-    UpdateTableRequestRequestTypeDef,
-    DataModelConfigurationOutputTypeDef,
-    DataModelConfigurationTypeDef,
-    CreateTableResponseTypeDef,
-    DescribeTableResponseTypeDef,
-    ListTablesResponseTypeDef,
-    UpdateTableResponseTypeDef,
-    BatchLoadTaskDescriptionTypeDef,
-    CreateBatchLoadTaskRequestRequestTypeDef,
-    DataModelConfigurationUnionTypeDef,
-    DescribeBatchLoadTaskResponseTypeDef,
-)
+from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
 
 def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/setup.py` & `types-aiobotocore-timestream-write-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-write",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__main__.py` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.TimestreamWrite 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.py` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from botocore.client import ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationUnionTypeDef,
+    DataModelConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaUnionTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -107,15 +107,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
+        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
@@ -135,15 +135,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...
+        Schema: SchemaTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -301,15 +301,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...
+        Schema: SchemaTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#update_table)
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.pyi` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from botocore.client import ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationUnionTypeDef,
+    DataModelConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaUnionTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -101,15 +101,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
+        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
@@ -127,15 +127,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...
+        Schema: SchemaTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -277,15 +277,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...
+        Schema: SchemaTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#update_table)
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.py` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,26 +252,28 @@
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

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.pyi` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -162,14 +163,15 @@
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
@@ -248,26 +250,28 @@
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

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.py` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
     data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -77,39 +77,32 @@
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
-    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
-    "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
-    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
-    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -590,38 +583,14 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
-_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_RequiredMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureValueType": MeasureValueTypeType,
-    },
-)
-_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_OptionalMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureName": str,
-        "SourceColumn": str,
-        "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class MixedMeasureMappingOutputTypeDef(
-    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
-):
-    pass
-
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -638,35 +607,14 @@
 
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
 
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
-
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
@@ -680,22 +628,14 @@
 
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
 
-SchemaOutputTypeDef = TypedDict(
-    "SchemaOutputTypeDef",
-    {
-        "CompositePartitionKey": List[PartitionKeyTypeDef],
-    },
-    total=False,
-)
-
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
@@ -756,37 +696,14 @@
 
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDataModelOutputTypeDef = TypedDict(
-    "_RequiredDataModelOutputTypeDef",
-    {
-        "DimensionMappings": List[DimensionMappingTypeDef],
-    },
-)
-_OptionalDataModelOutputTypeDef = TypedDict(
-    "_OptionalDataModelOutputTypeDef",
-    {
-        "TimeColumn": str,
-        "TimeUnit": TimeUnitType,
-        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
-        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
-        "MeasureNameColumn": str,
-    },
-    total=False,
-)
-
-
-class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
-    pass
-
-
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -802,15 +719,14 @@
 )
 
 
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
 
-SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -839,15 +755,15 @@
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaOutputTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -868,23 +784,14 @@
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
 
-DataModelConfigurationOutputTypeDef = TypedDict(
-    "DataModelConfigurationOutputTypeDef",
-    {
-        "DataModel": DataModelOutputTypeDef,
-        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
-    },
-    total=False,
-)
-
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
@@ -927,15 +834,15 @@
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
         "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
+        "DataModelConfiguration": DataModelConfigurationTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -966,17 +873,14 @@
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
 
-DataModelConfigurationUnionTypeDef = Union[
-    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
-]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.pyi` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
     data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -76,39 +76,32 @@
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
-    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
-    "DataModelOutputTypeDef",
     "DataModelTypeDef",
-    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
-    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
-    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -575,36 +568,14 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
-_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_RequiredMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureValueType": MeasureValueTypeType,
-    },
-)
-_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_OptionalMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureName": str,
-        "SourceColumn": str,
-        "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-    total=False,
-)
-
-class MixedMeasureMappingOutputTypeDef(
-    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
-):
-    pass
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -619,33 +590,14 @@
 )
 
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
@@ -657,22 +609,14 @@
 )
 
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-SchemaOutputTypeDef = TypedDict(
-    "SchemaOutputTypeDef",
-    {
-        "CompositePartitionKey": List[PartitionKeyTypeDef],
-    },
-    total=False,
-)
-
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
@@ -729,35 +673,14 @@
 )
 
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
-_RequiredDataModelOutputTypeDef = TypedDict(
-    "_RequiredDataModelOutputTypeDef",
-    {
-        "DimensionMappings": List[DimensionMappingTypeDef],
-    },
-)
-_OptionalDataModelOutputTypeDef = TypedDict(
-    "_OptionalDataModelOutputTypeDef",
-    {
-        "TimeColumn": str,
-        "TimeUnit": TimeUnitType,
-        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
-        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
-        "MeasureNameColumn": str,
-    },
-    total=False,
-)
-
-class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
-    pass
-
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -771,15 +694,14 @@
     },
     total=False,
 )
 
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
-SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -806,15 +728,15 @@
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaOutputTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -833,23 +755,14 @@
 )
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-DataModelConfigurationOutputTypeDef = TypedDict(
-    "DataModelConfigurationOutputTypeDef",
-    {
-        "DataModel": DataModelOutputTypeDef,
-        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
-    },
-    total=False,
-)
-
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
@@ -892,15 +805,15 @@
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
         "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
+        "DataModelConfiguration": DataModelConfigurationTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -929,17 +842,14 @@
 
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
-DataModelConfigurationUnionTypeDef = Union[
-    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
-]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-write-2.5.2.post2/types_aiobotocore_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

