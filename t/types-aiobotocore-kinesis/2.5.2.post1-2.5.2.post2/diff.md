# Comparing `tmp/types-aiobotocore-kinesis-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesis-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-2.5.2.post1.tar` & `types-aiobotocore-kinesis-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.185549 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26489 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31967 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31906 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-02 14:41:28.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.036643 types-aiobotocore-kinesis-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14113 2023-08-04 13:59:14.036643 types-aiobotocore-kinesis-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12595 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.036643 types-aiobotocore-kinesis-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.036643 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1583 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1582 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26533 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26489 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9928 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9926 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5614 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5608 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31967 2023-08-04 13:41:58.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31906 2023-08-04 13:41:58.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2729 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2727 2023-08-04 13:41:57.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.036643 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14113 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:13.000000 types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesis-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/README.md` & `types-aiobotocore-kinesis-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-kinesis
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Kinesis 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore kinesis type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesis"></a>
 
 # types-aiobotocore-kinesis
 
 [![PyPI - types-aiobotocore-kinesis](https://img.shields.io/pypi/v/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/)
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
 [types-aiobotocore-kinesis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,137 +322,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Kinesis` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/literals/).
+
 ```python
-from types_aiobotocore_kinesis.literals import (
-    ConsumerStatusType,
-    DescribeStreamPaginatorName,
-    EncryptionTypeType,
-    ListShardsPaginatorName,
-    ListStreamConsumersPaginatorName,
-    ListStreamsPaginatorName,
-    MetricsNameType,
-    ScalingTypeType,
-    ShardFilterTypeType,
-    ShardIteratorTypeType,
-    StreamExistsWaiterName,
-    StreamModeType,
-    StreamNotExistsWaiterName,
-    StreamStatusType,
-    KinesisServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_kinesis.literals import ConsumerStatusType
 
 
 def check_value(value: ConsumerStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Kinesis` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis.type_defs import (
-    AddTagsToStreamInputRequestTypeDef,
-    BlobTypeDef,
-    HashKeyRangeTypeDef,
-    ConsumerDescriptionTypeDef,
-    ConsumerTypeDef,
-    StreamModeDetailsTypeDef,
-    DecreaseStreamRetentionPeriodInputRequestTypeDef,
-    DeleteStreamInputRequestTypeDef,
-    DeregisterStreamConsumerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeStreamConsumerInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeStreamSummaryInputRequestTypeDef,
-    DisableEnhancedMonitoringInputRequestTypeDef,
-    EnableEnhancedMonitoringInputRequestTypeDef,
-    EnhancedMetricsTypeDef,
-    GetRecordsInputRequestTypeDef,
-    RecordTypeDef,
-    TimestampTypeDef,
-    IncreaseStreamRetentionPeriodInputRequestTypeDef,
-    InternalFailureExceptionTypeDef,
-    KMSAccessDeniedExceptionTypeDef,
-    KMSDisabledExceptionTypeDef,
-    KMSInvalidStateExceptionTypeDef,
-    KMSNotFoundExceptionTypeDef,
-    KMSOptInRequiredTypeDef,
-    KMSThrottlingExceptionTypeDef,
-    ListStreamsInputRequestTypeDef,
-    ListTagsForStreamInputRequestTypeDef,
-    TagTypeDef,
-    MergeShardsInputRequestTypeDef,
-    PutRecordsResultEntryTypeDef,
-    RegisterStreamConsumerInputRequestTypeDef,
-    RemoveTagsFromStreamInputRequestTypeDef,
-    ResourceInUseExceptionTypeDef,
-    ResourceNotFoundExceptionTypeDef,
-    SequenceNumberRangeTypeDef,
-    SplitShardInputRequestTypeDef,
-    StartStreamEncryptionInputRequestTypeDef,
-    StopStreamEncryptionInputRequestTypeDef,
-    UpdateShardCountInputRequestTypeDef,
-    PutRecordInputRequestTypeDef,
-    PutRecordsRequestEntryTypeDef,
-    ChildShardTypeDef,
-    CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
-    UpdateStreamModeInputRequestTypeDef,
-    DescribeLimitsOutputTypeDef,
-    DescribeStreamConsumerOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnhancedMonitoringOutputTypeDef,
-    GetShardIteratorOutputTypeDef,
-    ListStreamConsumersOutputTypeDef,
-    PutRecordOutputTypeDef,
-    RegisterStreamConsumerOutputTypeDef,
-    UpdateShardCountOutputTypeDef,
-    DescribeStreamInputDescribeStreamPaginateTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
-    DescribeStreamInputStreamExistsWaitTypeDef,
-    DescribeStreamInputStreamNotExistsWaitTypeDef,
-    StreamDescriptionSummaryTypeDef,
-    GetShardIteratorInputRequestTypeDef,
-    ListStreamConsumersInputListStreamConsumersPaginateTypeDef,
-    ListStreamConsumersInputRequestTypeDef,
-    ShardFilterTypeDef,
-    StartingPositionTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    PutRecordsOutputTypeDef,
-    ShardTypeDef,
-    PutRecordsInputRequestTypeDef,
-    GetRecordsOutputTypeDef,
-    SubscribeToShardEventTypeDef,
-    ListStreamsOutputTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
-    ListShardsInputListShardsPaginateTypeDef,
-    ListShardsInputRequestTypeDef,
-    SubscribeToShardInputRequestTypeDef,
-    ListShardsOutputTypeDef,
-    StreamDescriptionTypeDef,
-    SubscribeToShardEventStreamTypeDef,
-    DescribeStreamOutputTypeDef,
-    SubscribeToShardOutputTypeDef,
-)
+from types_aiobotocore_kinesis.type_defs import AddTagsToStreamInputRequestTypeDef
 
 
 def get_value() -> AddTagsToStreamInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/setup.py` & `types-aiobotocore-kinesis-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Kinesis 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__init__.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__init__.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/__main__.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Kinesis 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Kinesis 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis\nOther"
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

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/client.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/client.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/literals.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ConsumerStatusType",
     "DescribeStreamPaginatorName",
     "EncryptionTypeType",
     "ListShardsPaginatorName",
     "ListStreamConsumersPaginatorName",
     "ListStreamsPaginatorName",
@@ -38,15 +37,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ConsumerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 DescribeStreamPaginatorName = Literal["describe_stream"]
 EncryptionTypeType = Literal["KMS", "NONE"]
 ListShardsPaginatorName = Literal["list_shards"]
 ListStreamConsumersPaginatorName = Literal["list_stream_consumers"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MetricsNameType = Literal[
@@ -87,14 +85,15 @@
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
@@ -190,14 +189,15 @@
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
@@ -276,26 +276,28 @@
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
@@ -458,14 +460,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/literals.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ConsumerStatusType",
     "DescribeStreamPaginatorName",
     "EncryptionTypeType",
     "ListShardsPaginatorName",
     "ListStreamConsumersPaginatorName",
     "ListStreamsPaginatorName",
@@ -37,14 +38,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ConsumerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 DescribeStreamPaginatorName = Literal["describe_stream"]
 EncryptionTypeType = Literal["KMS", "NONE"]
 ListShardsPaginatorName = Literal["list_shards"]
 ListStreamConsumersPaginatorName = Literal["list_stream_consumers"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MetricsNameType = Literal[
@@ -85,14 +87,15 @@
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
@@ -188,14 +191,15 @@
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
@@ -274,26 +278,28 @@
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
@@ -456,14 +462,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/paginator.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/paginator.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/type_defs.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/type_defs.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/waiter.py` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis/waiter.pyi` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.5.2.post1/types_aiobotocore_kinesis.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-2.5.2.post2/types_aiobotocore_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

