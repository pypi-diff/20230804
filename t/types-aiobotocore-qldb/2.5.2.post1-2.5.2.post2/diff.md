# Comparing `tmp/types-aiobotocore-qldb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-qldb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qldb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-qldb-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-qldb-2.5.2.post1.tar` & `types-aiobotocore-qldb-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.033491 types-aiobotocore-qldb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-08-02 14:52:50.029491 types-aiobotocore-qldb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.033491 types-aiobotocore-qldb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.025491 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.029491 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.966643 types-aiobotocore-qldb-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12083 2023-08-04 13:59:21.966643 types-aiobotocore-qldb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10577 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.966643 types-aiobotocore-qldb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2027 2023-08-04 13:47:19.000000 types-aiobotocore-qldb-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.966643 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      418 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      417 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      920 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16612 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16584 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8633 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8631 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17819 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17792 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:20.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.966643 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12083 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      683 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qldb-2.5.2.post1/LICENSE` & `types-aiobotocore-qldb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2.post1/PKG-INFO` & `types-aiobotocore-qldb-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
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
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,93 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_qldb.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `QLDB` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/literals/).
+
 ```python
-from types_aiobotocore_qldb.literals import (
-    EncryptionStatusType,
-    ErrorCauseType,
-    ExportStatusType,
-    LedgerStateType,
-    OutputFormatType,
-    PermissionsModeType,
-    S3ObjectEncryptionTypeType,
-    StreamStatusType,
-    QLDBServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_qldb.literals import EncryptionStatusType
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_qldb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `QLDB` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/type_defs/).
+
 ```python
-from types_aiobotocore_qldb.type_defs import (
-    CancelJournalKinesisStreamRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateLedgerRequestRequestTypeDef,
-    DeleteLedgerRequestRequestTypeDef,
-    DescribeJournalKinesisStreamRequestRequestTypeDef,
-    DescribeJournalS3ExportRequestRequestTypeDef,
-    DescribeLedgerRequestRequestTypeDef,
-    LedgerEncryptionDescriptionTypeDef,
-    TimestampTypeDef,
-    ValueHolderTypeDef,
-    GetDigestRequestRequestTypeDef,
-    KinesisConfigurationTypeDef,
-    LedgerSummaryTypeDef,
-    ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
-    ListJournalS3ExportsForLedgerRequestRequestTypeDef,
-    ListJournalS3ExportsRequestRequestTypeDef,
-    ListLedgersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3EncryptionConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
-    CreateLedgerResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
-    DescribeLedgerResponseTypeDef,
-    UpdateLedgerResponseTypeDef,
-    GetBlockRequestRequestTypeDef,
-    GetBlockResponseTypeDef,
-    GetDigestResponseTypeDef,
-    GetRevisionRequestRequestTypeDef,
-    GetRevisionResponseTypeDef,
-    JournalKinesisStreamDescriptionTypeDef,
-    StreamJournalToKinesisRequestRequestTypeDef,
-    ListLedgersResponseTypeDef,
-    S3ExportConfigurationTypeDef,
-    DescribeJournalKinesisStreamResponseTypeDef,
-    ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    ExportJournalToS3RequestRequestTypeDef,
-    JournalS3ExportDescriptionTypeDef,
-    DescribeJournalS3ExportResponseTypeDef,
-    ListJournalS3ExportsForLedgerResponseTypeDef,
-    ListJournalS3ExportsResponseTypeDef,
-)
+from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
 
 def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-qldb-2.5.2.post1/README.md` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-qldb
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore qldb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
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
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -232,93 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_qldb.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `QLDB` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/literals/).
+
 ```python
-from types_aiobotocore_qldb.literals import (
-    EncryptionStatusType,
-    ErrorCauseType,
-    ExportStatusType,
-    LedgerStateType,
-    OutputFormatType,
-    PermissionsModeType,
-    S3ObjectEncryptionTypeType,
-    StreamStatusType,
-    QLDBServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_qldb.literals import EncryptionStatusType
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_qldb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `QLDB` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/type_defs/).
+
 ```python
-from types_aiobotocore_qldb.type_defs import (
-    CancelJournalKinesisStreamRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateLedgerRequestRequestTypeDef,
-    DeleteLedgerRequestRequestTypeDef,
-    DescribeJournalKinesisStreamRequestRequestTypeDef,
-    DescribeJournalS3ExportRequestRequestTypeDef,
-    DescribeLedgerRequestRequestTypeDef,
-    LedgerEncryptionDescriptionTypeDef,
-    TimestampTypeDef,
-    ValueHolderTypeDef,
-    GetDigestRequestRequestTypeDef,
-    KinesisConfigurationTypeDef,
-    LedgerSummaryTypeDef,
-    ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
-    ListJournalS3ExportsForLedgerRequestRequestTypeDef,
-    ListJournalS3ExportsRequestRequestTypeDef,
-    ListLedgersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3EncryptionConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
-    CreateLedgerResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
-    DescribeLedgerResponseTypeDef,
-    UpdateLedgerResponseTypeDef,
-    GetBlockRequestRequestTypeDef,
-    GetBlockResponseTypeDef,
-    GetDigestResponseTypeDef,
-    GetRevisionRequestRequestTypeDef,
-    GetRevisionResponseTypeDef,
-    JournalKinesisStreamDescriptionTypeDef,
-    StreamJournalToKinesisRequestRequestTypeDef,
-    ListLedgersResponseTypeDef,
-    S3ExportConfigurationTypeDef,
-    DescribeJournalKinesisStreamResponseTypeDef,
-    ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    ExportJournalToS3RequestRequestTypeDef,
-    JournalS3ExportDescriptionTypeDef,
-    DescribeJournalS3ExportResponseTypeDef,
-    ListJournalS3ExportsForLedgerResponseTypeDef,
-    ListJournalS3ExportsResponseTypeDef,
-)
+from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
 
 def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-qldb-2.5.2.post1/setup.py` & `types-aiobotocore-qldb-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qldb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__main__.py` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QLDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.QLDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.py` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.pyi` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.py` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -158,14 +159,15 @@
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
@@ -244,26 +246,28 @@
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

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.pyi` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -156,14 +157,15 @@
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
@@ -242,26 +244,28 @@
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

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.py` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.pyi` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/SOURCES.txt` & `types-aiobotocore-qldb-2.5.2.post2/types_aiobotocore_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

