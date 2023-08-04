# Comparing `tmp/types-aiobotocore-marketplace-catalog-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-marketplace-catalog-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1.tar` & `types-aiobotocore-marketplace-catalog-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.013527 types-aiobotocore-marketplace-catalog-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.013527 types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-02 14:42:50.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13751 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12186 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      910 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      909 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13997 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13974 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8331 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8329 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3648 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3644 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11091 2023-08-04 13:43:53.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11077 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13751 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/LICENSE` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,78 +293,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_marketplace_catalog.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceCatalog` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/literals/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.literals import (
-    ChangeStatusType,
-    FailureCodeType,
-    ListChangeSetsPaginatorName,
-    ListEntitiesPaginatorName,
-    OwnershipTypeType,
-    SortOrderType,
-    MarketplaceCatalogServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_marketplace_catalog.literals import ChangeStatusType
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceCatalog` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/type_defs/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.type_defs import (
-    CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
-    ErrorDetailTypeDef,
-    TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DescribeChangeSetRequestRequestTypeDef,
-    DescribeEntityRequestRequestTypeDef,
-    EntitySummaryTypeDef,
-    FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    SortTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    StartChangeSetResponseTypeDef,
-    ListChangeSetsResponseTypeDef,
-    ChangeSummaryTypeDef,
-    ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListEntitiesResponseTypeDef,
-    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
-    ListChangeSetsRequestRequestTypeDef,
-    ListEntitiesRequestListEntitiesPaginateTypeDef,
-    ListEntitiesRequestRequestTypeDef,
-    DescribeChangeSetResponseTypeDef,
-    StartChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
 
 def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/README.md` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-marketplace-catalog
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -261,78 +293,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_marketplace_catalog.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceCatalog` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/literals/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.literals import (
-    ChangeStatusType,
-    FailureCodeType,
-    ListChangeSetsPaginatorName,
-    ListEntitiesPaginatorName,
-    OwnershipTypeType,
-    SortOrderType,
-    MarketplaceCatalogServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_marketplace_catalog.literals import ChangeStatusType
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceCatalog` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/type_defs/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.type_defs import (
-    CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
-    ErrorDetailTypeDef,
-    TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DescribeChangeSetRequestRequestTypeDef,
-    DescribeEntityRequestRequestTypeDef,
-    EntitySummaryTypeDef,
-    FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    SortTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    StartChangeSetResponseTypeDef,
-    ListChangeSetsResponseTypeDef,
-    ChangeSummaryTypeDef,
-    ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListEntitiesResponseTypeDef,
-    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
-    ListChangeSetsRequestRequestTypeDef,
-    ListEntitiesRequestListEntitiesPaginateTypeDef,
-    ListEntitiesRequestRequestTypeDef,
-    DescribeChangeSetResponseTypeDef,
-    StartChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
 
 def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-catalog",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__main__.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
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

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.py`

 * *Files 0% similar despite different names*

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
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.pyi`

 * *Files 0% similar despite different names*

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
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,78 +261,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_marketplace_catalog.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceCatalog` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/literals/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.literals import (
-    ChangeStatusType,
-    FailureCodeType,
-    ListChangeSetsPaginatorName,
-    ListEntitiesPaginatorName,
-    OwnershipTypeType,
-    SortOrderType,
-    MarketplaceCatalogServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_marketplace_catalog.literals import ChangeStatusType
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceCatalog` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/type_defs/).
+
 ```python
-from types_aiobotocore_marketplace_catalog.type_defs import (
-    CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ChangeSetSummaryListItemTypeDef,
-    EntityTypeDef,
-    ErrorDetailTypeDef,
-    TagTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DescribeChangeSetRequestRequestTypeDef,
-    DescribeEntityRequestRequestTypeDef,
-    EntitySummaryTypeDef,
-    FilterTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    SortTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    StartChangeSetResponseTypeDef,
-    ListChangeSetsResponseTypeDef,
-    ChangeSummaryTypeDef,
-    ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListEntitiesResponseTypeDef,
-    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
-    ListChangeSetsRequestRequestTypeDef,
-    ListEntitiesRequestListEntitiesPaginateTypeDef,
-    ListEntitiesRequestRequestTypeDef,
-    DescribeChangeSetResponseTypeDef,
-    StartChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
 
 def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

