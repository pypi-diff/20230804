# Comparing `tmp/types-aiobotocore-opsworkscm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-opsworkscm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-opsworkscm-2.5.2.post1.tar` & `types-aiobotocore-opsworkscm-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.325505 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18749 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14212 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12682 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1499 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1498 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19181 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19148 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9143 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9141 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5487 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5481 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18776 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18749 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1638 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1637 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14212 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      949 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/LICENSE` & `types-aiobotocore-opsworkscm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-opsworkscm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,96 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_opsworkscm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpsWorksCM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/literals/).
+
 ```python
-from types_aiobotocore_opsworkscm.literals import (
-    BackupStatusType,
-    BackupTypeType,
-    DescribeBackupsPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeServersPaginatorName,
-    ListTagsForResourcePaginatorName,
-    MaintenanceStatusType,
-    NodeAssociatedWaiterName,
-    NodeAssociationStatusType,
-    ServerStatusType,
-    OpsWorksCMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_opsworkscm.literals import BackupStatusType
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpsWorksCM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/type_defs/).
+
 ```python
-from types_aiobotocore_opsworkscm.type_defs import (
-    AccountAttributeTypeDef,
-    EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    BackupTypeDef,
-    TagTypeDef,
-    DeleteBackupRequestRequestTypeDef,
-    DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    ServerEventTypeDef,
-    WaiterConfigTypeDef,
-    DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreServerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateServerEngineAttributesRequestRequestTypeDef,
-    UpdateServerRequestRequestTypeDef,
-    AssociateNodeRequestRequestTypeDef,
-    DisassociateNodeRequestRequestTypeDef,
-    ExportServerEngineAttributeRequestRequestTypeDef,
-    ServerTypeDef,
-    StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    CreateBackupRequestRequestTypeDef,
-    CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    CreateServerResponseTypeDef,
-    DescribeServersResponseTypeDef,
-    RestoreServerResponseTypeDef,
-    StartMaintenanceResponseTypeDef,
-    UpdateServerEngineAttributesResponseTypeDef,
-    UpdateServerResponseTypeDef,
-)
+from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef
 
 
 def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/README.md` & `types-aiobotocore-opsworkscm-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-opsworkscm
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,96 +322,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_opsworkscm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpsWorksCM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/literals/).
+
 ```python
-from types_aiobotocore_opsworkscm.literals import (
-    BackupStatusType,
-    BackupTypeType,
-    DescribeBackupsPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeServersPaginatorName,
-    ListTagsForResourcePaginatorName,
-    MaintenanceStatusType,
-    NodeAssociatedWaiterName,
-    NodeAssociationStatusType,
-    ServerStatusType,
-    OpsWorksCMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_opsworkscm.literals import BackupStatusType
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpsWorksCM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/type_defs/).
+
 ```python
-from types_aiobotocore_opsworkscm.type_defs import (
-    AccountAttributeTypeDef,
-    EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    BackupTypeDef,
-    TagTypeDef,
-    DeleteBackupRequestRequestTypeDef,
-    DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    ServerEventTypeDef,
-    WaiterConfigTypeDef,
-    DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreServerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateServerEngineAttributesRequestRequestTypeDef,
-    UpdateServerRequestRequestTypeDef,
-    AssociateNodeRequestRequestTypeDef,
-    DisassociateNodeRequestRequestTypeDef,
-    ExportServerEngineAttributeRequestRequestTypeDef,
-    ServerTypeDef,
-    StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    CreateBackupRequestRequestTypeDef,
-    CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    CreateServerResponseTypeDef,
-    DescribeServersResponseTypeDef,
-    RestoreServerResponseTypeDef,
-    StartMaintenanceResponseTypeDef,
-    UpdateServerEngineAttributesResponseTypeDef,
-    UpdateServerResponseTypeDef,
-)
+from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef
 
 
 def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/setup.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworkscm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__main__.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorksCM 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.OpsWorksCM 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
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
@@ -178,14 +179,15 @@
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
@@ -264,26 +266,28 @@
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
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
@@ -176,14 +177,15 @@
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
@@ -262,26 +264,28 @@
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.py` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,96 +322,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_opsworkscm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpsWorksCM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/literals/).
+
 ```python
-from types_aiobotocore_opsworkscm.literals import (
-    BackupStatusType,
-    BackupTypeType,
-    DescribeBackupsPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeServersPaginatorName,
-    ListTagsForResourcePaginatorName,
-    MaintenanceStatusType,
-    NodeAssociatedWaiterName,
-    NodeAssociationStatusType,
-    ServerStatusType,
-    OpsWorksCMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_opsworkscm.literals import BackupStatusType
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpsWorksCM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/type_defs/).
+
 ```python
-from types_aiobotocore_opsworkscm.type_defs import (
-    AccountAttributeTypeDef,
-    EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    BackupTypeDef,
-    TagTypeDef,
-    DeleteBackupRequestRequestTypeDef,
-    DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    ServerEventTypeDef,
-    WaiterConfigTypeDef,
-    DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreServerRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateServerEngineAttributesRequestRequestTypeDef,
-    UpdateServerRequestRequestTypeDef,
-    AssociateNodeRequestRequestTypeDef,
-    DisassociateNodeRequestRequestTypeDef,
-    ExportServerEngineAttributeRequestRequestTypeDef,
-    ServerTypeDef,
-    StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    CreateBackupRequestRequestTypeDef,
-    CreateServerRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    DescribeEventsResponseTypeDef,
-    DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    CreateServerResponseTypeDef,
-    DescribeServersResponseTypeDef,
-    RestoreServerResponseTypeDef,
-    StartMaintenanceResponseTypeDef,
-    UpdateServerEngineAttributesResponseTypeDef,
-    UpdateServerResponseTypeDef,
-)
+from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef
 
 
 def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt` & `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

