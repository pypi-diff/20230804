# Comparing `tmp/types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-servicecatalog-appregistry-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15887 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 14:49:34.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.009460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.066643 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14692 2023-08-04 13:59:26.066643 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13113 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.066643 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2193 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.066643 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1822 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1821 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22851 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22813 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9448 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9446 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7421 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7414 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21686 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21665 2023-08-04 13:53:23.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:22.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.066643 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14692 2023-08-04 13:59:25.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1174 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       45 2023-08-04 13:59:25.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/LICENSE` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,112 +310,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicecatalog_appregistry.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `AppRegistry` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/literals/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.literals import (
-    ListApplicationsPaginatorName,
-    ListAssociatedAttributeGroupsPaginatorName,
-    ListAssociatedResourcesPaginatorName,
-    ListAttributeGroupsForApplicationPaginatorName,
-    ListAttributeGroupsPaginatorName,
-    ResourceGroupStateType,
-    ResourceTypeType,
-    SyncActionType,
-    AppRegistryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicecatalog_appregistry.literals import ListApplicationsPaginatorName
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `AppRegistry` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/type_defs/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationTypeDef,
-    ApplicationSummaryTypeDef,
-    ApplicationTypeDef,
-    AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AssociateResourceRequestRequestTypeDef,
-    AttributeGroupDetailsTypeDef,
-    AttributeGroupSummaryTypeDef,
-    AttributeGroupTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    CreateAttributeGroupRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateResourceRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetAssociatedResourceRequestRequestTypeDef,
-    GetAttributeGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
-    SyncResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    ListAttributeGroupsForApplicationResponseTypeDef,
-    DeleteAttributeGroupResponseTypeDef,
-    ListAttributeGroupsResponseTypeDef,
-    CreateAttributeGroupResponseTypeDef,
-    UpdateAttributeGroupResponseTypeDef,
-    IntegrationsTypeDef,
-    ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
-    ResourceInfoTypeDef,
-    GetConfigurationResponseTypeDef,
-    PutConfigurationRequestRequestTypeDef,
-    GetApplicationResponseTypeDef,
-    ResourceTypeDef,
-    ListAssociatedResourcesResponseTypeDef,
-    GetAssociatedResourceResponseTypeDef,
-)
+from types_aiobotocore_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
 
 def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/README.md` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-servicecatalog-appregistry
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,112 +310,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicecatalog_appregistry.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `AppRegistry` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/literals/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.literals import (
-    ListApplicationsPaginatorName,
-    ListAssociatedAttributeGroupsPaginatorName,
-    ListAssociatedResourcesPaginatorName,
-    ListAttributeGroupsForApplicationPaginatorName,
-    ListAttributeGroupsPaginatorName,
-    ResourceGroupStateType,
-    ResourceTypeType,
-    SyncActionType,
-    AppRegistryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicecatalog_appregistry.literals import ListApplicationsPaginatorName
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `AppRegistry` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/type_defs/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationTypeDef,
-    ApplicationSummaryTypeDef,
-    ApplicationTypeDef,
-    AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AssociateResourceRequestRequestTypeDef,
-    AttributeGroupDetailsTypeDef,
-    AttributeGroupSummaryTypeDef,
-    AttributeGroupTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    CreateAttributeGroupRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateResourceRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetAssociatedResourceRequestRequestTypeDef,
-    GetAttributeGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
-    SyncResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    ListAttributeGroupsForApplicationResponseTypeDef,
-    DeleteAttributeGroupResponseTypeDef,
-    ListAttributeGroupsResponseTypeDef,
-    CreateAttributeGroupResponseTypeDef,
-    UpdateAttributeGroupResponseTypeDef,
-    IntegrationsTypeDef,
-    ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
-    ResourceInfoTypeDef,
-    GetConfigurationResponseTypeDef,
-    PutConfigurationRequestRequestTypeDef,
-    GetApplicationResponseTypeDef,
-    ResourceTypeDef,
-    ListAssociatedResourcesResponseTypeDef,
-    GetAssociatedResourceResponseTypeDef,
-)
+from types_aiobotocore_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
 
 def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog-appregistry",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__main__.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRegistry 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AppRegistry 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/literals.pyi`

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
     "ListApplicationsPaginatorName",
     "ListAssociatedAttributeGroupsPaginatorName",
     "ListAssociatedResourcesPaginatorName",
     "ListAttributeGroupsForApplicationPaginatorName",
     "ListAttributeGroupsPaginatorName",
     "ResourceGroupStateType",
@@ -31,15 +30,14 @@
     "AppRegistryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListAssociatedAttributeGroupsPaginatorName = Literal["list_associated_attribute_groups"]
 ListAssociatedResourcesPaginatorName = Literal["list_associated_resources"]
 ListAttributeGroupsForApplicationPaginatorName = Literal["list_attribute_groups_for_application"]
 ListAttributeGroupsPaginatorName = Literal["list_attribute_groups"]
 ResourceGroupStateType = Literal[
     "CREATE_COMPLETE", "CREATE_FAILED", "CREATING", "UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"
@@ -58,14 +56,15 @@
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
@@ -161,14 +160,15 @@
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
@@ -247,26 +247,28 @@
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
@@ -420,21 +422,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/literals.py`

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
     "ListApplicationsPaginatorName",
     "ListAssociatedAttributeGroupsPaginatorName",
     "ListAssociatedResourcesPaginatorName",
     "ListAttributeGroupsForApplicationPaginatorName",
     "ListAttributeGroupsPaginatorName",
     "ResourceGroupStateType",
@@ -30,14 +31,15 @@
     "AppRegistryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListAssociatedAttributeGroupsPaginatorName = Literal["list_associated_attribute_groups"]
 ListAssociatedResourcesPaginatorName = Literal["list_associated_resources"]
 ListAttributeGroupsForApplicationPaginatorName = Literal["list_attribute_groups_for_application"]
 ListAttributeGroupsPaginatorName = Literal["list_attribute_groups"]
 ResourceGroupStateType = Literal[
     "CREATE_COMPLETE", "CREATE_FAILED", "CREATING", "UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"
@@ -56,14 +58,15 @@
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
@@ -159,14 +162,15 @@
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
@@ -245,26 +249,28 @@
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
@@ -418,21 +424,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,112 +278,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicecatalog_appregistry.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `AppRegistry` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/literals/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.literals import (
-    ListApplicationsPaginatorName,
-    ListAssociatedAttributeGroupsPaginatorName,
-    ListAssociatedResourcesPaginatorName,
-    ListAttributeGroupsForApplicationPaginatorName,
-    ListAttributeGroupsPaginatorName,
-    ResourceGroupStateType,
-    ResourceTypeType,
-    SyncActionType,
-    AppRegistryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicecatalog_appregistry.literals import ListApplicationsPaginatorName
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `AppRegistry` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/type_defs/).
+
 ```python
-from types_aiobotocore_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationTypeDef,
-    ApplicationSummaryTypeDef,
-    ApplicationTypeDef,
-    AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AssociateResourceRequestRequestTypeDef,
-    AttributeGroupDetailsTypeDef,
-    AttributeGroupSummaryTypeDef,
-    AttributeGroupTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    CreateAttributeGroupRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateResourceRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetAssociatedResourceRequestRequestTypeDef,
-    GetAttributeGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ResourceDetailsTypeDef,
-    SyncResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    ListAttributeGroupsForApplicationResponseTypeDef,
-    DeleteAttributeGroupResponseTypeDef,
-    ListAttributeGroupsResponseTypeDef,
-    CreateAttributeGroupResponseTypeDef,
-    UpdateAttributeGroupResponseTypeDef,
-    IntegrationsTypeDef,
-    ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
-    ResourceInfoTypeDef,
-    GetConfigurationResponseTypeDef,
-    PutConfigurationRequestRequestTypeDef,
-    GetApplicationResponseTypeDef,
-    ResourceTypeDef,
-    ListAssociatedResourcesResponseTypeDef,
-    GetAssociatedResourceResponseTypeDef,
-)
+from types_aiobotocore_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
 
 def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post2/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

