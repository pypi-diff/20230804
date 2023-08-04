# Comparing `tmp/types-aiobotocore-secretsmanager-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-secretsmanager-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-secretsmanager-2.5.2.post1.tar` & `types-aiobotocore-secretsmanager-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:08.000000 types-aiobotocore-secretsmanager-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.361462 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13292 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11746 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.756643 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      685 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      684 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20286 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20254 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8696 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8694 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2251 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2248 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19547 2023-08-04 13:52:44.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19524 2023-08-04 13:52:44.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13292 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/LICENSE` & `types-aiobotocore-secretsmanager-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,97 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_secretsmanager.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SecretsManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/literals/).
+
 ```python
-from types_aiobotocore_secretsmanager.literals import (
-    FilterNameStringTypeType,
-    ListSecretsPaginatorName,
-    SortOrderTypeType,
-    StatusTypeType,
-    SecretsManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_secretsmanager.literals import FilterNameStringTypeType
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SecretsManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/type_defs/).
+
 ```python
-from types_aiobotocore_secretsmanager.type_defs import (
-    BlobTypeDef,
-    CancelRotateSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ReplicaRegionTypeTypeDef,
-    TagTypeDef,
-    ReplicationStatusTypeTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteSecretRequestRequestTypeDef,
-    DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
-    FilterTypeDef,
-    GetRandomPasswordRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    GetSecretValueRequestRequestTypeDef,
-    ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
-    PaginatorConfigTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    RemoveRegionsFromReplicationRequestRequestTypeDef,
-    RestoreSecretRequestRequestTypeDef,
-    StopReplicationToReplicaRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateSecretVersionStageRequestRequestTypeDef,
-    ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
-    DeleteSecretResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRandomPasswordResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSecretValueResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueResponseTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
-    UpdateSecretResponseTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
-    ReplicateSecretToRegionsRequestRequestTypeDef,
-    CreateSecretRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
-    ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
-)
+from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/README.md` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-secretsmanager
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,97 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_secretsmanager.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SecretsManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/literals/).
+
 ```python
-from types_aiobotocore_secretsmanager.literals import (
-    FilterNameStringTypeType,
-    ListSecretsPaginatorName,
-    SortOrderTypeType,
-    StatusTypeType,
-    SecretsManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_secretsmanager.literals import FilterNameStringTypeType
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SecretsManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/type_defs/).
+
 ```python
-from types_aiobotocore_secretsmanager.type_defs import (
-    BlobTypeDef,
-    CancelRotateSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ReplicaRegionTypeTypeDef,
-    TagTypeDef,
-    ReplicationStatusTypeTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteSecretRequestRequestTypeDef,
-    DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
-    FilterTypeDef,
-    GetRandomPasswordRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    GetSecretValueRequestRequestTypeDef,
-    ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
-    PaginatorConfigTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    RemoveRegionsFromReplicationRequestRequestTypeDef,
-    RestoreSecretRequestRequestTypeDef,
-    StopReplicationToReplicaRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateSecretVersionStageRequestRequestTypeDef,
-    ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
-    DeleteSecretResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRandomPasswordResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSecretValueResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueResponseTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
-    UpdateSecretResponseTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
-    ReplicateSecretToRegionsRequestRequestTypeDef,
-    CreateSecretRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
-    ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
-)
+from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/setup.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-secretsmanager",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__main__.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SecretsManager 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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
@@ -420,14 +424,15 @@
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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
@@ -418,14 +422,15 @@
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.py` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-secretsmanager
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,97 +257,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_secretsmanager.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SecretsManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/literals/).
+
 ```python
-from types_aiobotocore_secretsmanager.literals import (
-    FilterNameStringTypeType,
-    ListSecretsPaginatorName,
-    SortOrderTypeType,
-    StatusTypeType,
-    SecretsManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_secretsmanager.literals import FilterNameStringTypeType
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SecretsManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/type_defs/).
+
 ```python
-from types_aiobotocore_secretsmanager.type_defs import (
-    BlobTypeDef,
-    CancelRotateSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ReplicaRegionTypeTypeDef,
-    TagTypeDef,
-    ReplicationStatusTypeTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteSecretRequestRequestTypeDef,
-    DescribeSecretRequestRequestTypeDef,
-    RotationRulesTypeTypeDef,
-    FilterTypeDef,
-    GetRandomPasswordRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    GetSecretValueRequestRequestTypeDef,
-    ListSecretVersionIdsRequestRequestTypeDef,
-    SecretVersionsListEntryTypeDef,
-    PaginatorConfigTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    RemoveRegionsFromReplicationRequestRequestTypeDef,
-    RestoreSecretRequestRequestTypeDef,
-    StopReplicationToReplicaRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateSecretVersionStageRequestRequestTypeDef,
-    ValidateResourcePolicyRequestRequestTypeDef,
-    ValidationErrorsEntryTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
-    DeleteSecretResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRandomPasswordResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSecretValueResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueResponseTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
-    UpdateSecretResponseTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
-    ReplicateSecretToRegionsRequestRequestTypeDef,
-    CreateSecretRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateSecretResponseTypeDef,
-    RemoveRegionsFromReplicationResponseTypeDef,
-    ReplicateSecretToRegionsResponseTypeDef,
-    DescribeSecretResponseTypeDef,
-    RotateSecretRequestRequestTypeDef,
-    SecretListEntryTypeDef,
-    ListSecretsRequestRequestTypeDef,
-    ListSecretVersionIdsResponseTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
-    ValidateResourcePolicyResponseTypeDef,
-    ListSecretsResponseTypeDef,
-)
+from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt` & `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

