# Comparing `tmp/types-aiobotocore-cloudhsm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudhsm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsm-2.5.2.post1.tar` & `types-aiobotocore-cloudhsm-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.061637 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.843434 types-aiobotocore-cloudhsm-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-08-04 12:00:33.843434 types-aiobotocore-cloudhsm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.843434 types-aiobotocore-cloudhsm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.843434 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-08-04 11:41:54.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:53.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.843434 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:33.000000 types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudhsm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,90 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudhsm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CloudHSM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/literals/).
+
 ```python
-from types_aiobotocore_cloudhsm.literals import (
-    ClientVersionType,
-    CloudHsmObjectStateType,
-    HsmStatusType,
-    ListHapgsPaginatorName,
-    ListHsmsPaginatorName,
-    ListLunaClientsPaginatorName,
-    SubscriptionTypeType,
-    CloudHSMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloudhsm.literals import ClientVersionType
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudHSM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/type_defs/).
+
 ```python
-from types_aiobotocore_cloudhsm.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHapgRequestRequestTypeDef,
-    CreateHsmRequestRequestTypeDef,
-    CreateLunaClientRequestRequestTypeDef,
-    DeleteHapgRequestRequestTypeDef,
-    DeleteHsmRequestRequestTypeDef,
-    DeleteLunaClientRequestRequestTypeDef,
-    DescribeHapgRequestRequestTypeDef,
-    DescribeHsmRequestRequestTypeDef,
-    DescribeLunaClientRequestRequestTypeDef,
-    GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListHapgsRequestRequestTypeDef,
-    ListHsmsRequestRequestTypeDef,
-    ListLunaClientsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ModifyHapgRequestRequestTypeDef,
-    ModifyHsmRequestRequestTypeDef,
-    ModifyLunaClientRequestRequestTypeDef,
-    RemoveTagsFromResourceRequestRequestTypeDef,
-    AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
-)
+from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/README.md` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-cloudhsm
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,90 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudhsm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CloudHSM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/literals/).
+
 ```python
-from types_aiobotocore_cloudhsm.literals import (
-    ClientVersionType,
-    CloudHsmObjectStateType,
-    HsmStatusType,
-    ListHapgsPaginatorName,
-    ListHsmsPaginatorName,
-    ListLunaClientsPaginatorName,
-    SubscriptionTypeType,
-    CloudHSMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloudhsm.literals import ClientVersionType
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudHSM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/type_defs/).
+
 ```python
-from types_aiobotocore_cloudhsm.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHapgRequestRequestTypeDef,
-    CreateHsmRequestRequestTypeDef,
-    CreateLunaClientRequestRequestTypeDef,
-    DeleteHapgRequestRequestTypeDef,
-    DeleteHsmRequestRequestTypeDef,
-    DeleteLunaClientRequestRequestTypeDef,
-    DescribeHapgRequestRequestTypeDef,
-    DescribeHsmRequestRequestTypeDef,
-    DescribeLunaClientRequestRequestTypeDef,
-    GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListHapgsRequestRequestTypeDef,
-    ListHsmsRequestRequestTypeDef,
-    ListLunaClientsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ModifyHapgRequestRequestTypeDef,
-    ModifyHsmRequestRequestTypeDef,
-    ModifyLunaClientRequestRequestTypeDef,
-    RemoveTagsFromResourceRequestRequestTypeDef,
-    AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
-)
+from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/setup.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__main__.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSM 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSM 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.py` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-cloudhsm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,90 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudhsm.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CloudHSM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/literals/).
+
 ```python
-from types_aiobotocore_cloudhsm.literals import (
-    ClientVersionType,
-    CloudHsmObjectStateType,
-    HsmStatusType,
-    ListHapgsPaginatorName,
-    ListHsmsPaginatorName,
-    ListLunaClientsPaginatorName,
-    SubscriptionTypeType,
-    CloudHSMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloudhsm.literals import ClientVersionType
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudHSM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/type_defs/).
+
 ```python
-from types_aiobotocore_cloudhsm.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHapgRequestRequestTypeDef,
-    CreateHsmRequestRequestTypeDef,
-    CreateLunaClientRequestRequestTypeDef,
-    DeleteHapgRequestRequestTypeDef,
-    DeleteHsmRequestRequestTypeDef,
-    DeleteLunaClientRequestRequestTypeDef,
-    DescribeHapgRequestRequestTypeDef,
-    DescribeHsmRequestRequestTypeDef,
-    DescribeLunaClientRequestRequestTypeDef,
-    GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListHapgsRequestRequestTypeDef,
-    ListHsmsRequestRequestTypeDef,
-    ListLunaClientsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ModifyHapgRequestRequestTypeDef,
-    ModifyHsmRequestRequestTypeDef,
-    ModifyLunaClientRequestRequestTypeDef,
-    RemoveTagsFromResourceRequestRequestTypeDef,
-    AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
-)
+from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsm-2.5.2.post2/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

