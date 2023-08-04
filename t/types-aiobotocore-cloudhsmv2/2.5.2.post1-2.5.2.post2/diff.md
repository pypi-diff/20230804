# Comparing `tmp/types-aiobotocore-cloudhsmv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudhsmv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1.tar` & `types-aiobotocore-cloudhsmv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-02 14:34:41.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-02 14:34:41.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.895436 types-aiobotocore-cloudhsmv2-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-08-04 12:00:33.895436 types-aiobotocore-cloudhsmv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.895436 types-aiobotocore-cloudhsmv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.883435 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-04 11:41:56.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-04 11:41:55.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.895436 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,86 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudhsmv2.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CloudHSMV2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/literals/).
+
 ```python
-from types_aiobotocore_cloudhsmv2.literals import (
-    BackupPolicyType,
-    BackupRetentionTypeType,
-    BackupStateType,
-    ClusterStateType,
-    DescribeBackupsPaginatorName,
-    DescribeClustersPaginatorName,
-    HsmStateType,
-    ListTagsPaginatorName,
-    CloudHSMV2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloudhsmv2.literals import BackupPolicyType
 
 
 def check_value(value: BackupPolicyType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudHSMV2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/type_defs/).
+
 ```python
-from types_aiobotocore_cloudhsmv2.type_defs import (
-    BackupRetentionPolicyTypeDef,
-    TagTypeDef,
-    CertificatesTypeDef,
-    HsmTypeDef,
-    DestinationBackupTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHsmRequestRequestTypeDef,
-    DeleteBackupRequestRequestTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteHsmRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestRequestTypeDef,
-    InitializeClusterRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    ModifyBackupAttributesRequestRequestTypeDef,
-    RestoreBackupRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ModifyClusterRequestRequestTypeDef,
-    BackupTypeDef,
-    CopyBackupToRegionRequestRequestTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ClusterTypeDef,
-    CopyBackupToRegionResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    DeleteBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    ModifyBackupAttributesResponseTypeDef,
-    RestoreBackupResponseTypeDef,
-    CreateClusterResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DescribeClustersResponseTypeDef,
-    ModifyClusterResponseTypeDef,
-)
+from types_aiobotocore_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
 
 def get_value() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/README.md` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-cloudhsmv2
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore cloudhsmv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,86 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudhsmv2.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CloudHSMV2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/literals/).
+
 ```python
-from types_aiobotocore_cloudhsmv2.literals import (
-    BackupPolicyType,
-    BackupRetentionTypeType,
-    BackupStateType,
-    ClusterStateType,
-    DescribeBackupsPaginatorName,
-    DescribeClustersPaginatorName,
-    HsmStateType,
-    ListTagsPaginatorName,
-    CloudHSMV2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloudhsmv2.literals import BackupPolicyType
 
 
 def check_value(value: BackupPolicyType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudHSMV2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/type_defs/).
+
 ```python
-from types_aiobotocore_cloudhsmv2.type_defs import (
-    BackupRetentionPolicyTypeDef,
-    TagTypeDef,
-    CertificatesTypeDef,
-    HsmTypeDef,
-    DestinationBackupTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHsmRequestRequestTypeDef,
-    DeleteBackupRequestRequestTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteHsmRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestRequestTypeDef,
-    InitializeClusterRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    ModifyBackupAttributesRequestRequestTypeDef,
-    RestoreBackupRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ModifyClusterRequestRequestTypeDef,
-    BackupTypeDef,
-    CopyBackupToRegionRequestRequestTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ClusterTypeDef,
-    CopyBackupToRegionResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    DeleteBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    ModifyBackupAttributesResponseTypeDef,
-    RestoreBackupResponseTypeDef,
-    CreateClusterResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DescribeClustersResponseTypeDef,
-    ModifyClusterResponseTypeDef,
-)
+from types_aiobotocore_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
 
 def get_value() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsmv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsmv2-2.5.2.post2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

