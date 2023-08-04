# Comparing `tmp/types-aiobotocore-cognito-sync-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cognito-sync-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-sync-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-sync-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-cognito-sync-2.5.2.post1.tar` & `types-aiobotocore-cognito-sync-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.025618 types-aiobotocore-cognito-sync-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-08-02 14:52:05.025618 types-aiobotocore-cognito-sync-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:05.025618 types-aiobotocore-cognito-sync-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.021618 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.025618 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-sync-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-sync-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-sync-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.363644 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-08-04 11:42:42.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/LICENSE` & `types-aiobotocore-cognito-sync-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cognito-sync-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,84 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cognito_sync.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CognitoSync` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/literals/).
+
 ```python
-from types_aiobotocore_cognito_sync.literals import (
-    BulkPublishStatusType,
-    OperationType,
-    PlatformType,
-    StreamingStatusType,
-    CognitoSyncServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cognito_sync.literals import BulkPublishStatusType
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cognito_sync.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CognitoSync` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/type_defs/).
+
 ```python
-from types_aiobotocore_cognito_sync.type_defs import (
-    BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CognitoStreamsTypeDef,
-    DatasetTypeDef,
-    DeleteDatasetRequestRequestTypeDef,
-    DescribeDatasetRequestRequestTypeDef,
-    DescribeIdentityPoolUsageRequestRequestTypeDef,
-    IdentityPoolUsageTypeDef,
-    DescribeIdentityUsageRequestRequestTypeDef,
-    IdentityUsageTypeDef,
-    GetBulkPublishDetailsRequestRequestTypeDef,
-    GetCognitoEventsRequestRequestTypeDef,
-    GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncOutputTypeDef,
-    ListDatasetsRequestRequestTypeDef,
-    ListIdentityPoolUsageRequestRequestTypeDef,
-    ListRecordsRequestRequestTypeDef,
-    RecordTypeDef,
-    PushSyncTypeDef,
-    TimestampTypeDef,
-    RegisterDeviceRequestRequestTypeDef,
-    SetCognitoEventsRequestRequestTypeDef,
-    SubscribeToDatasetRequestRequestTypeDef,
-    UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DescribeIdentityPoolUsageResponseTypeDef,
-    ListIdentityPoolUsageResponseTypeDef,
-    DescribeIdentityUsageResponseTypeDef,
-    GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationResponseTypeDef,
-    ListRecordsResponseTypeDef,
-    UpdateRecordsResponseTypeDef,
-    PushSyncUnionTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
-    RecordPatchTypeDef,
-    UpdateRecordsRequestRequestTypeDef,
-)
+from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
 
 
 def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/README.md` & `types-aiobotocore-cognito-sync-2.5.2.post2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,84 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cognito_sync.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CognitoSync` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/literals/).
+
 ```python
-from types_aiobotocore_cognito_sync.literals import (
-    BulkPublishStatusType,
-    OperationType,
-    PlatformType,
-    StreamingStatusType,
-    CognitoSyncServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cognito_sync.literals import BulkPublishStatusType
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cognito_sync.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CognitoSync` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/type_defs/).
+
 ```python
-from types_aiobotocore_cognito_sync.type_defs import (
-    BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CognitoStreamsTypeDef,
-    DatasetTypeDef,
-    DeleteDatasetRequestRequestTypeDef,
-    DescribeDatasetRequestRequestTypeDef,
-    DescribeIdentityPoolUsageRequestRequestTypeDef,
-    IdentityPoolUsageTypeDef,
-    DescribeIdentityUsageRequestRequestTypeDef,
-    IdentityUsageTypeDef,
-    GetBulkPublishDetailsRequestRequestTypeDef,
-    GetCognitoEventsRequestRequestTypeDef,
-    GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncOutputTypeDef,
-    ListDatasetsRequestRequestTypeDef,
-    ListIdentityPoolUsageRequestRequestTypeDef,
-    ListRecordsRequestRequestTypeDef,
-    RecordTypeDef,
-    PushSyncTypeDef,
-    TimestampTypeDef,
-    RegisterDeviceRequestRequestTypeDef,
-    SetCognitoEventsRequestRequestTypeDef,
-    SubscribeToDatasetRequestRequestTypeDef,
-    UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DescribeIdentityPoolUsageResponseTypeDef,
-    ListIdentityPoolUsageResponseTypeDef,
-    DescribeIdentityUsageResponseTypeDef,
-    GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationResponseTypeDef,
-    ListRecordsResponseTypeDef,
-    UpdateRecordsResponseTypeDef,
-    PushSyncUnionTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
-    RecordPatchTypeDef,
-    UpdateRecordsRequestRequestTypeDef,
-)
+from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
 
 
 def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/setup.py` & `types-aiobotocore-cognito-sync-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-sync",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/__main__.py` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoSync 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CognitoSync 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
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

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/client.py` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     ListRecordsResponseTypeDef,
-    PushSyncUnionTypeDef,
+    PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     UpdateRecordsResponseTypeDef,
 )
 
 __all__ = ("CognitoSyncClient",)
@@ -254,15 +254,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_cognito_events)
         """
 
     async def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
-        PushSync: PushSyncUnionTypeDef = ...,
+        PushSync: PushSyncTypeDef = ...,
         CognitoStreams: CognitoStreamsTypeDef = ...
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_identity_pool_configuration)
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/client.pyi` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     ListRecordsResponseTypeDef,
-    PushSyncUnionTypeDef,
+    PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceResponseTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     UpdateRecordsResponseTypeDef,
 )
 
 __all__ = ("CognitoSyncClient",)
@@ -234,15 +234,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_cognito_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_cognito_events)
         """
     async def set_identity_pool_configuration(
         self,
         *,
         IdentityPoolId: str,
-        PushSync: PushSyncUnionTypeDef = ...,
+        PushSync: PushSyncTypeDef = ...,
         CognitoStreams: CognitoStreamsTypeDef = ...
     ) -> SetIdentityPoolConfigurationResponseTypeDef:
         """
         Sets the necessary configuration for push sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/client/#set_identity_pool_configuration)
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/literals.py` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/literals.pyi` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/type_defs.py` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,35 +18,33 @@
 from .literals import BulkPublishStatusType, OperationType, PlatformType, StreamingStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
-    "PushSyncOutputTypeDef",
+    "PushSyncTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
-    "PushSyncTypeDef",
     "TimestampTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -56,19 +54,18 @@
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
+    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
-    "PushSyncUnionTypeDef",
-    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "RecordPatchTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
@@ -184,16 +181,16 @@
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-PushSyncOutputTypeDef = TypedDict(
-    "PushSyncOutputTypeDef",
+PushSyncTypeDef = TypedDict(
+    "PushSyncTypeDef",
     {
         "ApplicationArns": List[str],
         "RoleArn": str,
     },
     total=False,
 )
 
@@ -209,21 +206,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasetsRequestRequestTypeDef(
     _RequiredListDatasetsRequestRequestTypeDef, _OptionalListDatasetsRequestRequestTypeDef
 ):
     pass
 
-
 ListIdentityPoolUsageRequestRequestTypeDef = TypedDict(
     "ListIdentityPoolUsageRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -244,43 +239,32 @@
         "NextToken": str,
         "MaxResults": int,
         "SyncSessionToken": str,
     },
     total=False,
 )
 
-
 class ListRecordsRequestRequestTypeDef(
     _RequiredListRecordsRequestRequestTypeDef, _OptionalListRecordsRequestRequestTypeDef
 ):
     pass
 
-
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "Key": str,
         "Value": str,
         "SyncCount": int,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "DeviceLastModifiedDate": datetime,
     },
     total=False,
 )
 
-PushSyncTypeDef = TypedDict(
-    "PushSyncTypeDef",
-    {
-        "ApplicationArns": Sequence[str],
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 RegisterDeviceRequestRequestTypeDef = TypedDict(
     "RegisterDeviceRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
@@ -412,25 +396,46 @@
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncOutputTypeDef,
+        "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "IdentityPoolId": str,
+    },
+)
+_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "PushSync": PushSyncTypeDef,
+        "CognitoStreams": CognitoStreamsTypeDef,
+    },
+    total=False,
+)
+
+class SetIdentityPoolConfigurationRequestRequestTypeDef(
+    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
+    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
+):
+    pass
+
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncOutputTypeDef,
+        "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
@@ -452,38 +457,14 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PushSyncUnionTypeDef = Union[PushSyncTypeDef, PushSyncOutputTypeDef]
-_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "IdentityPoolId": str,
-    },
-)
-_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
-    },
-    total=False,
-)
-
-
-class SetIdentityPoolConfigurationRequestRequestTypeDef(
-    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
-    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredRecordPatchTypeDef = TypedDict(
     "_RequiredRecordPatchTypeDef",
     {
         "Op": OperationType,
         "Key": str,
         "SyncCount": int,
     },
@@ -493,19 +474,17 @@
     {
         "Value": str,
         "DeviceLastModifiedDate": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
     pass
 
-
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
@@ -517,12 +496,11 @@
         "DeviceId": str,
         "RecordPatches": Sequence[RecordPatchTypeDef],
         "ClientContext": str,
     },
     total=False,
 )
 
-
 class UpdateRecordsRequestRequestTypeDef(
     _RequiredUpdateRecordsRequestRequestTypeDef, _OptionalUpdateRecordsRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync/type_defs.pyi` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 from .literals import BulkPublishStatusType, OperationType, PlatformType, StreamingStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
-    "PushSyncOutputTypeDef",
+    "PushSyncTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
-    "PushSyncTypeDef",
     "TimestampTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -55,19 +55,18 @@
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
+    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
-    "PushSyncUnionTypeDef",
-    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "RecordPatchTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
@@ -183,16 +182,16 @@
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-PushSyncOutputTypeDef = TypedDict(
-    "PushSyncOutputTypeDef",
+PushSyncTypeDef = TypedDict(
+    "PushSyncTypeDef",
     {
         "ApplicationArns": List[str],
         "RoleArn": str,
     },
     total=False,
 )
 
@@ -208,19 +207,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasetsRequestRequestTypeDef(
     _RequiredListDatasetsRequestRequestTypeDef, _OptionalListDatasetsRequestRequestTypeDef
 ):
     pass
 
+
 ListIdentityPoolUsageRequestRequestTypeDef = TypedDict(
     "ListIdentityPoolUsageRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -241,41 +242,34 @@
         "NextToken": str,
         "MaxResults": int,
         "SyncSessionToken": str,
     },
     total=False,
 )
 
+
 class ListRecordsRequestRequestTypeDef(
     _RequiredListRecordsRequestRequestTypeDef, _OptionalListRecordsRequestRequestTypeDef
 ):
     pass
 
+
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "Key": str,
         "Value": str,
         "SyncCount": int,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "DeviceLastModifiedDate": datetime,
     },
     total=False,
 )
 
-PushSyncTypeDef = TypedDict(
-    "PushSyncTypeDef",
-    {
-        "ApplicationArns": Sequence[str],
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 RegisterDeviceRequestRequestTypeDef = TypedDict(
     "RegisterDeviceRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "Platform": PlatformType,
@@ -407,25 +401,48 @@
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncOutputTypeDef,
+        "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "IdentityPoolId": str,
+    },
+)
+_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "PushSync": PushSyncTypeDef,
+        "CognitoStreams": CognitoStreamsTypeDef,
+    },
+    total=False,
+)
+
+
+class SetIdentityPoolConfigurationRequestRequestTypeDef(
+    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
+    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncOutputTypeDef,
+        "PushSync": PushSyncTypeDef,
         "CognitoStreams": CognitoStreamsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
@@ -447,36 +464,14 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PushSyncUnionTypeDef = Union[PushSyncTypeDef, PushSyncOutputTypeDef]
-_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "IdentityPoolId": str,
-    },
-)
-_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
-    },
-    total=False,
-)
-
-class SetIdentityPoolConfigurationRequestRequestTypeDef(
-    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
-    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredRecordPatchTypeDef = TypedDict(
     "_RequiredRecordPatchTypeDef",
     {
         "Op": OperationType,
         "Key": str,
         "SyncCount": int,
     },
@@ -486,17 +481,19 @@
     {
         "Value": str,
         "DeviceLastModifiedDate": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class RecordPatchTypeDef(_RequiredRecordPatchTypeDef, _OptionalRecordPatchTypeDef):
     pass
 
+
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
@@ -508,11 +505,12 @@
         "DeviceId": str,
         "RecordPatches": Sequence[RecordPatchTypeDef],
         "ClientContext": str,
     },
     total=False,
 )
 
+
 class UpdateRecordsRequestRequestTypeDef(
     _RequiredUpdateRecordsRequestRequestTypeDef, _OptionalUpdateRecordsRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/PKG-INFO` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
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
 [types-aiobotocore-cognito-sync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,84 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cognito_sync.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CognitoSync` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/literals/).
+
 ```python
-from types_aiobotocore_cognito_sync.literals import (
-    BulkPublishStatusType,
-    OperationType,
-    PlatformType,
-    StreamingStatusType,
-    CognitoSyncServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cognito_sync.literals import BulkPublishStatusType
 
 
 def check_value(value: BulkPublishStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cognito_sync.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CognitoSync` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/type_defs/).
+
 ```python
-from types_aiobotocore_cognito_sync.type_defs import (
-    BulkPublishRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CognitoStreamsTypeDef,
-    DatasetTypeDef,
-    DeleteDatasetRequestRequestTypeDef,
-    DescribeDatasetRequestRequestTypeDef,
-    DescribeIdentityPoolUsageRequestRequestTypeDef,
-    IdentityPoolUsageTypeDef,
-    DescribeIdentityUsageRequestRequestTypeDef,
-    IdentityUsageTypeDef,
-    GetBulkPublishDetailsRequestRequestTypeDef,
-    GetCognitoEventsRequestRequestTypeDef,
-    GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncOutputTypeDef,
-    ListDatasetsRequestRequestTypeDef,
-    ListIdentityPoolUsageRequestRequestTypeDef,
-    ListRecordsRequestRequestTypeDef,
-    RecordTypeDef,
-    PushSyncTypeDef,
-    TimestampTypeDef,
-    RegisterDeviceRequestRequestTypeDef,
-    SetCognitoEventsRequestRequestTypeDef,
-    SubscribeToDatasetRequestRequestTypeDef,
-    UnsubscribeFromDatasetRequestRequestTypeDef,
-    BulkPublishResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBulkPublishDetailsResponseTypeDef,
-    GetCognitoEventsResponseTypeDef,
-    RegisterDeviceResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DescribeDatasetResponseTypeDef,
-    ListDatasetsResponseTypeDef,
-    DescribeIdentityPoolUsageResponseTypeDef,
-    ListIdentityPoolUsageResponseTypeDef,
-    DescribeIdentityUsageResponseTypeDef,
-    GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationResponseTypeDef,
-    ListRecordsResponseTypeDef,
-    UpdateRecordsResponseTypeDef,
-    PushSyncUnionTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
-    RecordPatchTypeDef,
-    UpdateRecordsRequestRequestTypeDef,
-)
+from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestRequestTypeDef
 
 
 def get_value() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post1/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-sync-2.5.2.post2/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

