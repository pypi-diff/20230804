# Comparing `tmp/types-aiobotocore-resource-groups-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-resource-groups-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-groups-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-groups-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-resource-groups-2.5.2.post1.tar` & `types-aiobotocore-resource-groups-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.905481 types-aiobotocore-resource-groups-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-08-02 14:52:52.893481 types-aiobotocore-resource-groups-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.905481 types-aiobotocore-resource-groups-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.889481 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:47:55.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:54.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:52.000000 types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.066643 types-aiobotocore-resource-groups-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13663 2023-08-04 13:59:23.066643 types-aiobotocore-resource-groups-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12114 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.066643 types-aiobotocore-resource-groups-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.056643 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1101 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1100 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16991 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16961 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9536 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9534 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4614 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4609 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15878 2023-08-04 13:50:48.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15863 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:47.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.066643 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13663 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:22.000000 types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/LICENSE` & `types-aiobotocore-resource-groups-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/PKG-INFO` & `types-aiobotocore-resource-groups-2.5.2.post2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-groups
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,107 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_groups.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroups` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/literals/).
+
 ```python
-from types_aiobotocore_resource_groups.literals import (
-    GroupConfigurationStatusType,
-    GroupFilterNameType,
-    GroupLifecycleEventsDesiredStatusType,
-    GroupLifecycleEventsStatusType,
-    ListGroupResourcesPaginatorName,
-    ListGroupsPaginatorName,
-    QueryErrorCodeType,
-    QueryTypeType,
-    ResourceFilterNameType,
-    ResourceStatusValueType,
-    SearchResourcesPaginatorName,
-    ResourceGroupsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_groups.literals import GroupConfigurationStatusType
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ResourceGroups` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/type_defs/).
+
 ```python
-from types_aiobotocore_resource_groups.type_defs import (
-    AccountSettingsTypeDef,
-    ResourceQueryTypeDef,
-    GroupTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteGroupInputRequestTypeDef,
-    FailedResourceTypeDef,
-    GetGroupConfigurationInputRequestTypeDef,
-    GetGroupInputRequestTypeDef,
-    GetGroupQueryInputRequestTypeDef,
-    GetTagsInputRequestTypeDef,
-    GroupConfigurationParameterOutputTypeDef,
-    GroupConfigurationParameterTypeDef,
-    GroupFilterTypeDef,
-    GroupIdentifierTypeDef,
-    GroupResourcesInputRequestTypeDef,
-    PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceFilterTypeDef,
-    ResourceIdentifierTypeDef,
-    ResourceStatusTypeDef,
-    QueryErrorTypeDef,
-    TagInputRequestTypeDef,
-    UngroupResourcesInputRequestTypeDef,
-    UntagInputRequestTypeDef,
-    UpdateAccountSettingsInputRequestTypeDef,
-    UpdateGroupInputRequestTypeDef,
-    GroupQueryTypeDef,
-    SearchResourcesInputRequestTypeDef,
-    UpdateGroupQueryInputRequestTypeDef,
-    DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    UpdateGroupOutputTypeDef,
-    GroupConfigurationItemOutputTypeDef,
-    GroupConfigurationItemTypeDef,
-    ListGroupsInputRequestTypeDef,
-    ListGroupsOutputTypeDef,
-    GroupResourcesOutputTypeDef,
-    UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
-    ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
-    ListGroupResourcesInputRequestTypeDef,
-    ListGroupResourcesItemTypeDef,
-    SearchResourcesOutputTypeDef,
-    GetGroupQueryOutputTypeDef,
-    UpdateGroupQueryOutputTypeDef,
-    GroupConfigurationTypeDef,
-    GroupConfigurationItemUnionTypeDef,
-    ListGroupResourcesOutputTypeDef,
-    CreateGroupOutputTypeDef,
-    GetGroupConfigurationOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
-)
+from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
 
 def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/README.md` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-resource-groups
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,107 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_groups.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroups` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/literals/).
+
 ```python
-from types_aiobotocore_resource_groups.literals import (
-    GroupConfigurationStatusType,
-    GroupFilterNameType,
-    GroupLifecycleEventsDesiredStatusType,
-    GroupLifecycleEventsStatusType,
-    ListGroupResourcesPaginatorName,
-    ListGroupsPaginatorName,
-    QueryErrorCodeType,
-    QueryTypeType,
-    ResourceFilterNameType,
-    ResourceStatusValueType,
-    SearchResourcesPaginatorName,
-    ResourceGroupsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_groups.literals import GroupConfigurationStatusType
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ResourceGroups` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/type_defs/).
+
 ```python
-from types_aiobotocore_resource_groups.type_defs import (
-    AccountSettingsTypeDef,
-    ResourceQueryTypeDef,
-    GroupTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteGroupInputRequestTypeDef,
-    FailedResourceTypeDef,
-    GetGroupConfigurationInputRequestTypeDef,
-    GetGroupInputRequestTypeDef,
-    GetGroupQueryInputRequestTypeDef,
-    GetTagsInputRequestTypeDef,
-    GroupConfigurationParameterOutputTypeDef,
-    GroupConfigurationParameterTypeDef,
-    GroupFilterTypeDef,
-    GroupIdentifierTypeDef,
-    GroupResourcesInputRequestTypeDef,
-    PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceFilterTypeDef,
-    ResourceIdentifierTypeDef,
-    ResourceStatusTypeDef,
-    QueryErrorTypeDef,
-    TagInputRequestTypeDef,
-    UngroupResourcesInputRequestTypeDef,
-    UntagInputRequestTypeDef,
-    UpdateAccountSettingsInputRequestTypeDef,
-    UpdateGroupInputRequestTypeDef,
-    GroupQueryTypeDef,
-    SearchResourcesInputRequestTypeDef,
-    UpdateGroupQueryInputRequestTypeDef,
-    DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    UpdateGroupOutputTypeDef,
-    GroupConfigurationItemOutputTypeDef,
-    GroupConfigurationItemTypeDef,
-    ListGroupsInputRequestTypeDef,
-    ListGroupsOutputTypeDef,
-    GroupResourcesOutputTypeDef,
-    UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
-    ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
-    ListGroupResourcesInputRequestTypeDef,
-    ListGroupResourcesItemTypeDef,
-    SearchResourcesOutputTypeDef,
-    GetGroupQueryOutputTypeDef,
-    UpdateGroupQueryOutputTypeDef,
-    GroupConfigurationTypeDef,
-    GroupConfigurationItemUnionTypeDef,
-    ListGroupResourcesOutputTypeDef,
-    CreateGroupOutputTypeDef,
-    GetGroupConfigurationOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
-)
+from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
 
 def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/setup.py` & `types-aiobotocore-resource-groups-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-groups",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__init__.pyi` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/__main__.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ResourceGroups 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
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

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemUnionTypeDef,
+    GroupConfigurationItemTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -110,15 +110,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -231,15 +231,15 @@
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
 
     async def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/client.pyi` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemUnionTypeDef,
+    GroupConfigurationItemTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -103,15 +103,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -213,15 +213,15 @@
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
     async def put_group_configuration(
-        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -34,15 +33,14 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
@@ -66,14 +64,15 @@
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
@@ -169,14 +168,15 @@
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
@@ -255,26 +255,28 @@
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
@@ -436,14 +438,15 @@
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

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/literals.pyi` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/literals.py`

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
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -33,14 +34,15 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
@@ -64,14 +66,15 @@
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
@@ -167,14 +170,15 @@
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
@@ -253,26 +257,28 @@
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
@@ -434,14 +440,15 @@
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

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/paginator.pyi` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.py` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
     data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -40,15 +40,14 @@
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
     "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
@@ -67,35 +66,33 @@
     "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
     "GetTagsOutputTypeDef",
     "TagOutputTypeDef",
     "UntagOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
-    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
     "ListGroupsInputListGroupsPaginateTypeDef",
     "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
-    "GroupConfigurationItemUnionTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -191,36 +188,14 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
-    "_RequiredGroupConfigurationParameterOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
-    "_OptionalGroupConfigurationParameterOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
-
-class GroupConfigurationParameterOutputTypeDef(
-    _RequiredGroupConfigurationParameterOutputTypeDef,
-    _OptionalGroupConfigurationParameterOutputTypeDef,
-):
-    pass
-
-
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
@@ -472,35 +447,14 @@
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
-    "_RequiredGroupConfigurationItemOutputTypeDef",
-    {
-        "Type": str,
-    },
-)
-_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
-    "_OptionalGroupConfigurationItemOutputTypeDef",
-    {
-        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class GroupConfigurationItemOutputTypeDef(
-    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
-):
-    pass
-
-
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -643,28 +597,58 @@
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGroupInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGroupInputRequestTypeDef",
+    {
+        "Description": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Mapping[str, str],
+        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateGroupInputRequestTypeDef(
+    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
+):
+    pass
+
+
 GroupConfigurationTypeDef = TypedDict(
     "GroupConfigurationTypeDef",
     {
-        "Configuration": List[GroupConfigurationItemOutputTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
+        "Configuration": List[GroupConfigurationItemTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
-GroupConfigurationItemUnionTypeDef = Union[
-    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
-]
+PutGroupConfigurationInputRequestTypeDef = TypedDict(
+    "PutGroupConfigurationInputRequestTypeDef",
+    {
+        "Group": str,
+        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+    },
+    total=False,
+)
+
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
@@ -686,40 +670,7 @@
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGroupInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGroupInputRequestTypeDef",
-    {
-        "Description": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateGroupInputRequestTypeDef(
-    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
-):
-    pass
-
-
-PutGroupConfigurationInputRequestTypeDef = TypedDict(
-    "PutGroupConfigurationInputRequestTypeDef",
-    {
-        "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
-    },
-    total=False,
-)
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups/type_defs.pyi` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
     data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     GroupConfigurationStatusType,
     GroupFilterNameType,
     GroupLifecycleEventsDesiredStatusType,
     GroupLifecycleEventsStatusType,
     QueryErrorCodeType,
@@ -39,15 +39,14 @@
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
     "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
@@ -66,35 +65,33 @@
     "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
     "GetTagsOutputTypeDef",
     "TagOutputTypeDef",
     "UntagOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
-    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
     "ListGroupsInputListGroupsPaginateTypeDef",
     "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
-    "GroupConfigurationItemUnionTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -188,34 +185,14 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
-    "_RequiredGroupConfigurationParameterOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
-    "_OptionalGroupConfigurationParameterOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
-class GroupConfigurationParameterOutputTypeDef(
-    _RequiredGroupConfigurationParameterOutputTypeDef,
-    _OptionalGroupConfigurationParameterOutputTypeDef,
-):
-    pass
-
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
@@ -461,33 +438,14 @@
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
-    "_RequiredGroupConfigurationItemOutputTypeDef",
-    {
-        "Type": str,
-    },
-)
-_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
-    "_OptionalGroupConfigurationItemOutputTypeDef",
-    {
-        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-class GroupConfigurationItemOutputTypeDef(
-    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
-):
-    pass
-
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -626,28 +584,56 @@
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGroupInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGroupInputRequestTypeDef",
+    {
+        "Description": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Mapping[str, str],
+        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+    },
+    total=False,
+)
+
+class CreateGroupInputRequestTypeDef(
+    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
+):
+    pass
+
 GroupConfigurationTypeDef = TypedDict(
     "GroupConfigurationTypeDef",
     {
-        "Configuration": List[GroupConfigurationItemOutputTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
+        "Configuration": List[GroupConfigurationItemTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
-GroupConfigurationItemUnionTypeDef = Union[
-    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
-]
+PutGroupConfigurationInputRequestTypeDef = TypedDict(
+    "PutGroupConfigurationInputRequestTypeDef",
+    {
+        "Group": str,
+        "Configuration": Sequence[GroupConfigurationItemTypeDef],
+    },
+    total=False,
+)
+
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
@@ -669,38 +655,7 @@
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGroupInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGroupInputRequestTypeDef",
-    {
-        "Description": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Mapping[str, str],
-        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateGroupInputRequestTypeDef(
-    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
-):
-    pass
-
-PutGroupConfigurationInputRequestTypeDef = TypedDict(
-    "PutGroupConfigurationInputRequestTypeDef",
-    {
-        "Group": str,
-        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
-    },
-    total=False,
-)
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/PKG-INFO` & `types-aiobotocore-resource-groups-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-resource-groups
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceGroups 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
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
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,107 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resource_groups.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroups` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/literals/).
+
 ```python
-from types_aiobotocore_resource_groups.literals import (
-    GroupConfigurationStatusType,
-    GroupFilterNameType,
-    GroupLifecycleEventsDesiredStatusType,
-    GroupLifecycleEventsStatusType,
-    ListGroupResourcesPaginatorName,
-    ListGroupsPaginatorName,
-    QueryErrorCodeType,
-    QueryTypeType,
-    ResourceFilterNameType,
-    ResourceStatusValueType,
-    SearchResourcesPaginatorName,
-    ResourceGroupsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resource_groups.literals import GroupConfigurationStatusType
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resource_groups.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ResourceGroups` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/type_defs/).
+
 ```python
-from types_aiobotocore_resource_groups.type_defs import (
-    AccountSettingsTypeDef,
-    ResourceQueryTypeDef,
-    GroupTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteGroupInputRequestTypeDef,
-    FailedResourceTypeDef,
-    GetGroupConfigurationInputRequestTypeDef,
-    GetGroupInputRequestTypeDef,
-    GetGroupQueryInputRequestTypeDef,
-    GetTagsInputRequestTypeDef,
-    GroupConfigurationParameterOutputTypeDef,
-    GroupConfigurationParameterTypeDef,
-    GroupFilterTypeDef,
-    GroupIdentifierTypeDef,
-    GroupResourcesInputRequestTypeDef,
-    PendingResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceFilterTypeDef,
-    ResourceIdentifierTypeDef,
-    ResourceStatusTypeDef,
-    QueryErrorTypeDef,
-    TagInputRequestTypeDef,
-    UngroupResourcesInputRequestTypeDef,
-    UntagInputRequestTypeDef,
-    UpdateAccountSettingsInputRequestTypeDef,
-    UpdateGroupInputRequestTypeDef,
-    GroupQueryTypeDef,
-    SearchResourcesInputRequestTypeDef,
-    UpdateGroupQueryInputRequestTypeDef,
-    DeleteGroupOutputTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    GetGroupOutputTypeDef,
-    GetTagsOutputTypeDef,
-    TagOutputTypeDef,
-    UntagOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    UpdateGroupOutputTypeDef,
-    GroupConfigurationItemOutputTypeDef,
-    GroupConfigurationItemTypeDef,
-    ListGroupsInputRequestTypeDef,
-    ListGroupsOutputTypeDef,
-    GroupResourcesOutputTypeDef,
-    UngroupResourcesOutputTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
-    ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
-    ListGroupResourcesInputRequestTypeDef,
-    ListGroupResourcesItemTypeDef,
-    SearchResourcesOutputTypeDef,
-    GetGroupQueryOutputTypeDef,
-    UpdateGroupQueryOutputTypeDef,
-    GroupConfigurationTypeDef,
-    GroupConfigurationItemUnionTypeDef,
-    ListGroupResourcesOutputTypeDef,
-    CreateGroupOutputTypeDef,
-    GetGroupConfigurationOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
-)
+from types_aiobotocore_resource_groups.type_defs import AccountSettingsTypeDef
 
 
 def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resource-groups-2.5.2.post1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt` & `types-aiobotocore-resource-groups-2.5.2.post2/types_aiobotocore_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

