# Comparing `tmp/types-aiobotocore-resource-explorer-2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-resource-explorer-2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1.tar` & `types-aiobotocore-resource-explorer-2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-02 14:47:53.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.066643 types-aiobotocore-resource-explorer-2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13991 2023-08-04 13:59:23.066643 types-aiobotocore-resource-explorer-2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12428 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.066643 types-aiobotocore-resource-explorer-2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2129 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.056643 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1300 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1299 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      985 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18703 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18671 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8763 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8761 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5657 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5651 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13070 2023-08-04 13:50:46.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13059 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:45.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.066643 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13991 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.000000 types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/LICENSE` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-explorer-2
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,93 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_explorer_2.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceExplorer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/literals/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.literals import (
-    IndexStateType,
-    IndexTypeType,
-    ListIndexesPaginatorName,
-    ListSupportedResourceTypesPaginatorName,
-    ListViewsPaginatorName,
-    SearchPaginatorName,
-    ResourceExplorerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_explorer_2.literals import IndexStateType
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `ResourceExplorer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/type_defs/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.type_defs import (
-    AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    BatchGetViewErrorTypeDef,
-    BatchGetViewInputRequestTypeDef,
-    CreateIndexInputRequestTypeDef,
-    IncludedPropertyTypeDef,
-    SearchFilterTypeDef,
-    DeleteIndexInputRequestTypeDef,
-    DeleteViewInputRequestTypeDef,
-    GetViewInputRequestTypeDef,
-    IndexTypeDef,
-    PaginatorConfigTypeDef,
-    ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputRequestTypeDef,
-    SupportedResourceTypeTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListViewsInputRequestTypeDef,
-    ResourceCountTypeDef,
-    ResourcePropertyTypeDef,
-    SearchInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
-    UpdateIndexTypeOutputTypeDef,
-    CreateViewInputRequestTypeDef,
-    UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
-    ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
-    ListSupportedResourceTypesOutputTypeDef,
-    ResourceTypeDef,
-    BatchGetViewOutputTypeDef,
-    CreateViewOutputTypeDef,
-    GetViewOutputTypeDef,
-    UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
-)
+from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef
 
 
 def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/README.md` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-resource-explorer-2
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,93 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_explorer_2.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceExplorer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/literals/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.literals import (
-    IndexStateType,
-    IndexTypeType,
-    ListIndexesPaginatorName,
-    ListSupportedResourceTypesPaginatorName,
-    ListViewsPaginatorName,
-    SearchPaginatorName,
-    ResourceExplorerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_explorer_2.literals import IndexStateType
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `ResourceExplorer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/type_defs/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.type_defs import (
-    AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    BatchGetViewErrorTypeDef,
-    BatchGetViewInputRequestTypeDef,
-    CreateIndexInputRequestTypeDef,
-    IncludedPropertyTypeDef,
-    SearchFilterTypeDef,
-    DeleteIndexInputRequestTypeDef,
-    DeleteViewInputRequestTypeDef,
-    GetViewInputRequestTypeDef,
-    IndexTypeDef,
-    PaginatorConfigTypeDef,
-    ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputRequestTypeDef,
-    SupportedResourceTypeTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListViewsInputRequestTypeDef,
-    ResourceCountTypeDef,
-    ResourcePropertyTypeDef,
-    SearchInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
-    UpdateIndexTypeOutputTypeDef,
-    CreateViewInputRequestTypeDef,
-    UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
-    ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
-    ListSupportedResourceTypesOutputTypeDef,
-    ResourceTypeDef,
-    BatchGetViewOutputTypeDef,
-    CreateViewOutputTypeDef,
-    GetViewOutputTypeDef,
-    UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
-)
+from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef
 
 
 def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-explorer-2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__main__.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ResourceExplorer 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
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

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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
@@ -417,13 +421,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/literals.pyi`

 * *Files 1% similar despite different names*

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
@@ -415,13 +419,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-resource-explorer-2
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,93 +267,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_explorer_2.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceExplorer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/literals/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.literals import (
-    IndexStateType,
-    IndexTypeType,
-    ListIndexesPaginatorName,
-    ListSupportedResourceTypesPaginatorName,
-    ListViewsPaginatorName,
-    SearchPaginatorName,
-    ResourceExplorerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_explorer_2.literals import IndexStateType
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `ResourceExplorer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/type_defs/).
+
 ```python
-from types_aiobotocore_resource_explorer_2.type_defs import (
-    AssociateDefaultViewInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    BatchGetViewErrorTypeDef,
-    BatchGetViewInputRequestTypeDef,
-    CreateIndexInputRequestTypeDef,
-    IncludedPropertyTypeDef,
-    SearchFilterTypeDef,
-    DeleteIndexInputRequestTypeDef,
-    DeleteViewInputRequestTypeDef,
-    GetViewInputRequestTypeDef,
-    IndexTypeDef,
-    PaginatorConfigTypeDef,
-    ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputRequestTypeDef,
-    SupportedResourceTypeTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListViewsInputRequestTypeDef,
-    ResourceCountTypeDef,
-    ResourcePropertyTypeDef,
-    SearchInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateIndexTypeInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
-    CreateIndexOutputTypeDef,
-    DeleteIndexOutputTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsOutputTypeDef,
-    UpdateIndexTypeOutputTypeDef,
-    CreateViewInputRequestTypeDef,
-    UpdateViewInputRequestTypeDef,
-    ViewTypeDef,
-    ListIndexesOutputTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
-    SearchInputSearchPaginateTypeDef,
-    ListSupportedResourceTypesOutputTypeDef,
-    ResourceTypeDef,
-    BatchGetViewOutputTypeDef,
-    CreateViewOutputTypeDef,
-    GetViewOutputTypeDef,
-    UpdateViewOutputTypeDef,
-    SearchOutputTypeDef,
-)
+from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef
 
 
 def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt` & `types-aiobotocore-resource-explorer-2-2.5.2.post2/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

