# Comparing `tmp/types-aiobotocore-amp-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-amp-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amp-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-amp-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-amp-2.5.2.post1.tar` & `types-aiobotocore-amp-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.837667 types-aiobotocore-amp-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16341 2023-08-02 14:51:47.837667 types-aiobotocore-amp-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.837667 types-aiobotocore-amp-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18387 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-02 14:32:48.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.837667 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16341 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:51:47.000000 types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.726886 types-aiobotocore-amp-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-08-04 12:00:19.726886 types-aiobotocore-amp-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.730886 types-aiobotocore-amp-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.714886 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18387 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-04 11:39:54.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-08-04 11:39:54.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-04 11:39:53.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.726886 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:19.000000 types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amp-2.5.2.post1/LICENSE` & `types-aiobotocore-amp-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/PKG-INFO` & `types-aiobotocore-amp-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
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
 [types-aiobotocore-amp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,101 +318,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_amp.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `PrometheusService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/literals/).
+
 ```python
-from types_aiobotocore_amp.literals import (
-    AlertManagerDefinitionStatusCodeType,
-    ListRuleGroupsNamespacesPaginatorName,
-    ListWorkspacesPaginatorName,
-    LoggingConfigurationStatusCodeType,
-    RuleGroupsNamespaceStatusCodeType,
-    WorkspaceActiveWaiterName,
-    WorkspaceDeletedWaiterName,
-    WorkspaceStatusCodeType,
-    PrometheusServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_amp.literals import AlertManagerDefinitionStatusCodeType
 
 
 def check_value(value: AlertManagerDefinitionStatusCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_amp.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PrometheusService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/type_defs/).
+
 ```python
-from types_aiobotocore_amp.type_defs import (
-    AlertManagerDefinitionStatusTypeDef,
-    BlobTypeDef,
-    ResponseMetadataTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationStatusTypeDef,
-    RuleGroupsNamespaceStatusTypeDef,
-    CreateWorkspaceRequestRequestTypeDef,
-    WorkspaceStatusTypeDef,
-    DeleteAlertManagerDefinitionRequestRequestTypeDef,
-    DeleteLoggingConfigurationRequestRequestTypeDef,
-    DeleteRuleGroupsNamespaceRequestRequestTypeDef,
-    DeleteWorkspaceRequestRequestTypeDef,
-    DescribeAlertManagerDefinitionRequestRequestTypeDef,
-    DescribeLoggingConfigurationRequestRequestTypeDef,
-    DescribeRuleGroupsNamespaceRequestRequestTypeDef,
-    DescribeWorkspaceRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ListRuleGroupsNamespacesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListWorkspacesRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
-    UpdateWorkspaceAliasRequestRequestTypeDef,
-    AlertManagerDefinitionDescriptionTypeDef,
-    CreateAlertManagerDefinitionRequestRequestTypeDef,
-    CreateRuleGroupsNamespaceRequestRequestTypeDef,
-    PutAlertManagerDefinitionRequestRequestTypeDef,
-    PutRuleGroupsNamespaceRequestRequestTypeDef,
-    CreateAlertManagerDefinitionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutAlertManagerDefinitionResponseTypeDef,
-    CreateLoggingConfigurationResponseTypeDef,
-    LoggingConfigurationMetadataTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    CreateRuleGroupsNamespaceResponseTypeDef,
-    PutRuleGroupsNamespaceResponseTypeDef,
-    RuleGroupsNamespaceDescriptionTypeDef,
-    RuleGroupsNamespaceSummaryTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    WorkspaceDescriptionTypeDef,
-    WorkspaceSummaryTypeDef,
-    DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef,
-    DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef,
-    ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
-    DescribeAlertManagerDefinitionResponseTypeDef,
-    DescribeLoggingConfigurationResponseTypeDef,
-    DescribeRuleGroupsNamespaceResponseTypeDef,
-    ListRuleGroupsNamespacesResponseTypeDef,
-    DescribeWorkspaceResponseTypeDef,
-    ListWorkspacesResponseTypeDef,
-)
+from types_aiobotocore_amp.type_defs import AlertManagerDefinitionStatusTypeDef
 
 
 def get_value() -> AlertManagerDefinitionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-amp-2.5.2.post1/README.md` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-amp
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore amp type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amp"></a>
 
 # types-aiobotocore-amp
 
 [![PyPI - types-aiobotocore-amp](https://img.shields.io/pypi/v/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
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
 [types-aiobotocore-amp docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,101 +318,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_amp.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `PrometheusService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/literals/).
+
 ```python
-from types_aiobotocore_amp.literals import (
-    AlertManagerDefinitionStatusCodeType,
-    ListRuleGroupsNamespacesPaginatorName,
-    ListWorkspacesPaginatorName,
-    LoggingConfigurationStatusCodeType,
-    RuleGroupsNamespaceStatusCodeType,
-    WorkspaceActiveWaiterName,
-    WorkspaceDeletedWaiterName,
-    WorkspaceStatusCodeType,
-    PrometheusServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_amp.literals import AlertManagerDefinitionStatusCodeType
 
 
 def check_value(value: AlertManagerDefinitionStatusCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_amp.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PrometheusService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/type_defs/).
+
 ```python
-from types_aiobotocore_amp.type_defs import (
-    AlertManagerDefinitionStatusTypeDef,
-    BlobTypeDef,
-    ResponseMetadataTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
-    LoggingConfigurationStatusTypeDef,
-    RuleGroupsNamespaceStatusTypeDef,
-    CreateWorkspaceRequestRequestTypeDef,
-    WorkspaceStatusTypeDef,
-    DeleteAlertManagerDefinitionRequestRequestTypeDef,
-    DeleteLoggingConfigurationRequestRequestTypeDef,
-    DeleteRuleGroupsNamespaceRequestRequestTypeDef,
-    DeleteWorkspaceRequestRequestTypeDef,
-    DescribeAlertManagerDefinitionRequestRequestTypeDef,
-    DescribeLoggingConfigurationRequestRequestTypeDef,
-    DescribeRuleGroupsNamespaceRequestRequestTypeDef,
-    DescribeWorkspaceRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ListRuleGroupsNamespacesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListWorkspacesRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
-    UpdateWorkspaceAliasRequestRequestTypeDef,
-    AlertManagerDefinitionDescriptionTypeDef,
-    CreateAlertManagerDefinitionRequestRequestTypeDef,
-    CreateRuleGroupsNamespaceRequestRequestTypeDef,
-    PutAlertManagerDefinitionRequestRequestTypeDef,
-    PutRuleGroupsNamespaceRequestRequestTypeDef,
-    CreateAlertManagerDefinitionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutAlertManagerDefinitionResponseTypeDef,
-    CreateLoggingConfigurationResponseTypeDef,
-    LoggingConfigurationMetadataTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    CreateRuleGroupsNamespaceResponseTypeDef,
-    PutRuleGroupsNamespaceResponseTypeDef,
-    RuleGroupsNamespaceDescriptionTypeDef,
-    RuleGroupsNamespaceSummaryTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    WorkspaceDescriptionTypeDef,
-    WorkspaceSummaryTypeDef,
-    DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef,
-    DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef,
-    ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
-    DescribeAlertManagerDefinitionResponseTypeDef,
-    DescribeLoggingConfigurationResponseTypeDef,
-    DescribeRuleGroupsNamespaceResponseTypeDef,
-    ListRuleGroupsNamespacesResponseTypeDef,
-    DescribeWorkspaceResponseTypeDef,
-    ListWorkspacesResponseTypeDef,
-)
+from types_aiobotocore_amp.type_defs import AlertManagerDefinitionStatusTypeDef
 
 
 def get_value() -> AlertManagerDefinitionStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-amp-2.5.2.post1/setup.py` & `types-aiobotocore-amp-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amp",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__init__.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__init__.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/__main__.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PrometheusService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
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

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/client.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/client.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/literals.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/literals.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/paginator.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/paginator.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/type_defs.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/type_defs.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/waiter.py` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp/waiter.pyi` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post1/types_aiobotocore_amp.egg-info/SOURCES.txt` & `types-aiobotocore-amp-2.5.2.post2/types_aiobotocore_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

