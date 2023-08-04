# Comparing `tmp/types-aiobotocore-kinesisanalytics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesisanalytics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1.tar` & `types-aiobotocore-kinesisanalytics-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:41:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26551 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26518 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12689 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11135 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.246643 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      514 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      513 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17025 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16997 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8548 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8546 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26021 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25990 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12689 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,121 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesisanalytics.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisAnalytics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/literals/).
+
 ```python
-from types_aiobotocore_kinesisanalytics.literals import (
-    ApplicationStatusType,
-    InputStartingPositionType,
-    RecordFormatTypeType,
-    KinesisAnalyticsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kinesisanalytics.literals import ApplicationStatusType
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesisanalytics.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KinesisAnalytics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/type_defs/).
+
 ```python
-from types_aiobotocore_kinesisanalytics.type_defs import (
-    CloudWatchLoggingOptionTypeDef,
-    CloudWatchLoggingOptionDescriptionTypeDef,
-    ApplicationSummaryTypeDef,
-    CloudWatchLoggingOptionUpdateTypeDef,
-    CSVMappingParametersTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    TimestampTypeDef,
-    DescribeApplicationRequestRequestTypeDef,
-    DestinationSchemaTypeDef,
-    InputStartingPositionConfigurationTypeDef,
-    S3ConfigurationTypeDef,
-    InputParallelismTypeDef,
-    KinesisFirehoseInputDescriptionTypeDef,
-    KinesisStreamsInputDescriptionTypeDef,
-    InputLambdaProcessorDescriptionTypeDef,
-    InputLambdaProcessorTypeDef,
-    InputLambdaProcessorUpdateTypeDef,
-    InputParallelismUpdateTypeDef,
-    RecordColumnTypeDef,
-    KinesisFirehoseInputTypeDef,
-    KinesisStreamsInputTypeDef,
-    KinesisFirehoseInputUpdateTypeDef,
-    KinesisStreamsInputUpdateTypeDef,
-    JSONMappingParametersTypeDef,
-    KinesisFirehoseOutputDescriptionTypeDef,
-    KinesisFirehoseOutputTypeDef,
-    KinesisFirehoseOutputUpdateTypeDef,
-    KinesisStreamsOutputDescriptionTypeDef,
-    KinesisStreamsOutputTypeDef,
-    KinesisStreamsOutputUpdateTypeDef,
-    LambdaOutputDescriptionTypeDef,
-    LambdaOutputTypeDef,
-    LambdaOutputUpdateTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3ReferenceDataSourceDescriptionTypeDef,
-    S3ReferenceDataSourceTypeDef,
-    S3ReferenceDataSourceUpdateTypeDef,
-    StopApplicationRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    InputConfigurationTypeDef,
-    InputProcessingConfigurationDescriptionTypeDef,
-    InputProcessingConfigurationTypeDef,
-    InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersTypeDef,
-    OutputDescriptionTypeDef,
-    OutputTypeDef,
-    OutputUpdateTypeDef,
-    StartApplicationRequestRequestTypeDef,
-    AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatTypeDef,
-    AddApplicationOutputRequestRequestTypeDef,
-    InputSchemaUpdateTypeDef,
-    SourceSchemaOutputTypeDef,
-    SourceSchemaTypeDef,
-    InputUpdateTypeDef,
-    DiscoverInputSchemaResponseTypeDef,
-    InputDescriptionTypeDef,
-    ReferenceDataSourceDescriptionTypeDef,
-    InputTypeDef,
-    ReferenceDataSourceTypeDef,
-    ReferenceDataSourceUpdateTypeDef,
-    ApplicationDetailTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    AddApplicationReferenceDataSourceRequestRequestTypeDef,
-    ApplicationUpdateTypeDef,
-    DescribeApplicationResponseTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-)
+from types_aiobotocore_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
 
 def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/README.md` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-kinesisanalytics
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore kinesisanalytics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,121 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesisanalytics.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisAnalytics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/literals/).
+
 ```python
-from types_aiobotocore_kinesisanalytics.literals import (
-    ApplicationStatusType,
-    InputStartingPositionType,
-    RecordFormatTypeType,
-    KinesisAnalyticsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kinesisanalytics.literals import ApplicationStatusType
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesisanalytics.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KinesisAnalytics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/type_defs/).
+
 ```python
-from types_aiobotocore_kinesisanalytics.type_defs import (
-    CloudWatchLoggingOptionTypeDef,
-    CloudWatchLoggingOptionDescriptionTypeDef,
-    ApplicationSummaryTypeDef,
-    CloudWatchLoggingOptionUpdateTypeDef,
-    CSVMappingParametersTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    TimestampTypeDef,
-    DescribeApplicationRequestRequestTypeDef,
-    DestinationSchemaTypeDef,
-    InputStartingPositionConfigurationTypeDef,
-    S3ConfigurationTypeDef,
-    InputParallelismTypeDef,
-    KinesisFirehoseInputDescriptionTypeDef,
-    KinesisStreamsInputDescriptionTypeDef,
-    InputLambdaProcessorDescriptionTypeDef,
-    InputLambdaProcessorTypeDef,
-    InputLambdaProcessorUpdateTypeDef,
-    InputParallelismUpdateTypeDef,
-    RecordColumnTypeDef,
-    KinesisFirehoseInputTypeDef,
-    KinesisStreamsInputTypeDef,
-    KinesisFirehoseInputUpdateTypeDef,
-    KinesisStreamsInputUpdateTypeDef,
-    JSONMappingParametersTypeDef,
-    KinesisFirehoseOutputDescriptionTypeDef,
-    KinesisFirehoseOutputTypeDef,
-    KinesisFirehoseOutputUpdateTypeDef,
-    KinesisStreamsOutputDescriptionTypeDef,
-    KinesisStreamsOutputTypeDef,
-    KinesisStreamsOutputUpdateTypeDef,
-    LambdaOutputDescriptionTypeDef,
-    LambdaOutputTypeDef,
-    LambdaOutputUpdateTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3ReferenceDataSourceDescriptionTypeDef,
-    S3ReferenceDataSourceTypeDef,
-    S3ReferenceDataSourceUpdateTypeDef,
-    StopApplicationRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    InputConfigurationTypeDef,
-    InputProcessingConfigurationDescriptionTypeDef,
-    InputProcessingConfigurationTypeDef,
-    InputProcessingConfigurationUpdateTypeDef,
-    MappingParametersTypeDef,
-    OutputDescriptionTypeDef,
-    OutputTypeDef,
-    OutputUpdateTypeDef,
-    StartApplicationRequestRequestTypeDef,
-    AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DiscoverInputSchemaRequestRequestTypeDef,
-    RecordFormatTypeDef,
-    AddApplicationOutputRequestRequestTypeDef,
-    InputSchemaUpdateTypeDef,
-    SourceSchemaOutputTypeDef,
-    SourceSchemaTypeDef,
-    InputUpdateTypeDef,
-    DiscoverInputSchemaResponseTypeDef,
-    InputDescriptionTypeDef,
-    ReferenceDataSourceDescriptionTypeDef,
-    InputTypeDef,
-    ReferenceDataSourceTypeDef,
-    ReferenceDataSourceUpdateTypeDef,
-    ApplicationDetailTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    AddApplicationReferenceDataSourceRequestRequestTypeDef,
-    ApplicationUpdateTypeDef,
-    DescribeApplicationResponseTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-)
+from types_aiobotocore_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
 
 def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalytics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__main__.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisAnalytics 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
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
@@ -148,14 +149,15 @@
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
@@ -234,26 +236,28 @@
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

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,26 +85,25 @@
     "OutputUpdateTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
-    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "ReferenceDataSourceDescriptionTypeDef",
     "InputTypeDef",
+    "ReferenceDataSourceDescriptionTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -744,36 +743,14 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
-_RequiredSourceSchemaOutputTypeDef = TypedDict(
-    "_RequiredSourceSchemaOutputTypeDef",
-    {
-        "RecordFormat": RecordFormatTypeDef,
-        "RecordColumns": List[RecordColumnTypeDef],
-    },
-)
-_OptionalSourceSchemaOutputTypeDef = TypedDict(
-    "_OptionalSourceSchemaOutputTypeDef",
-    {
-        "RecordEncoding": str,
-    },
-    total=False,
-)
-
-
-class SourceSchemaOutputTypeDef(
-    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
-):
-    pass
-
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -813,15 +790,15 @@
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -830,64 +807,64 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
+_RequiredInputTypeDef = TypedDict(
+    "_RequiredInputTypeDef",
     {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+        "NamePrefix": str,
+        "InputSchema": SourceSchemaTypeDef,
     },
 )
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
+_OptionalInputTypeDef = TypedDict(
+    "_OptionalInputTypeDef",
     {
-        "ReferenceSchema": SourceSchemaOutputTypeDef,
+        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
+        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
+        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
 
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
 
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
+        "ReferenceSchema": SourceSchemaTypeDef,
     },
     total=False,
 )
 
 
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
     pass
 
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
@@ -928,45 +905,14 @@
 
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
 
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
-
-
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -994,14 +940,45 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
+
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,26 +84,25 @@
     "OutputUpdateTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
-    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "ReferenceDataSourceDescriptionTypeDef",
     "InputTypeDef",
+    "ReferenceDataSourceDescriptionTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -729,34 +728,14 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
-_RequiredSourceSchemaOutputTypeDef = TypedDict(
-    "_RequiredSourceSchemaOutputTypeDef",
-    {
-        "RecordFormat": RecordFormatTypeDef,
-        "RecordColumns": List[RecordColumnTypeDef],
-    },
-)
-_OptionalSourceSchemaOutputTypeDef = TypedDict(
-    "_OptionalSourceSchemaOutputTypeDef",
-    {
-        "RecordEncoding": str,
-    },
-    total=False,
-)
-
-class SourceSchemaOutputTypeDef(
-    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
-):
-    pass
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -792,15 +771,15 @@
 
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -809,42 +788,21 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
-    },
-)
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceSchema": SourceSchemaOutputTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
-    pass
-
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -858,14 +816,35 @@
     },
     total=False,
 )
 
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+    },
+)
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceSchema": SourceSchemaTypeDef,
+    },
+    total=False,
+)
+
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
+
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -899,43 +878,14 @@
 )
 
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
-
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -961,14 +911,43 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

