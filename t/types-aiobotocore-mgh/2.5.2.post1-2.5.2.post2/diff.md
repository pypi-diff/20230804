# Comparing `tmp/types-aiobotocore-mgh-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mgh-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgh-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgh-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-mgh-2.5.2.post1.tar` & `types-aiobotocore-mgh-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.909520 types-aiobotocore-mgh-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-08-02 14:52:40.909520 types-aiobotocore-mgh-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.909520 types-aiobotocore-mgh-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.909520 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-08-02 14:43:35.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:34.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.909520 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:40.000000 types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13515 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12004 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2029 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1678 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1677 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      934 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18634 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18603 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9047 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9045 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6864 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6857 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17738 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17703 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13515 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgh-2.5.2.post1/LICENSE` & `types-aiobotocore-mgh-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/PKG-INFO` & `types-aiobotocore-mgh-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
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
 [types-aiobotocore-mgh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,86 +307,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mgh.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `MigrationHub` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/literals/).
+
 ```python
-from types_aiobotocore_mgh.literals import (
-    ApplicationStatusType,
-    ListApplicationStatesPaginatorName,
-    ListCreatedArtifactsPaginatorName,
-    ListDiscoveredResourcesPaginatorName,
-    ListMigrationTasksPaginatorName,
-    ListProgressUpdateStreamsPaginatorName,
-    ResourceAttributeTypeType,
-    StatusType,
-    MigrationHubServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mgh.literals import ApplicationStatusType
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mgh.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MigrationHub` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/type_defs/).
+
 ```python
-from types_aiobotocore_mgh.type_defs import (
-    ApplicationStateTypeDef,
-    CreatedArtifactTypeDef,
-    DiscoveredResourceTypeDef,
-    CreateProgressUpdateStreamRequestRequestTypeDef,
-    DeleteProgressUpdateStreamRequestRequestTypeDef,
-    DescribeApplicationStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeMigrationTaskRequestRequestTypeDef,
-    DisassociateCreatedArtifactRequestRequestTypeDef,
-    DisassociateDiscoveredResourceRequestRequestTypeDef,
-    ImportMigrationTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationStatesRequestRequestTypeDef,
-    ListCreatedArtifactsRequestRequestTypeDef,
-    ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMigrationTasksRequestRequestTypeDef,
-    MigrationTaskSummaryTypeDef,
-    ListProgressUpdateStreamsRequestRequestTypeDef,
-    ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeTypeDef,
-    TaskTypeDef,
-    TimestampTypeDef,
-    AssociateCreatedArtifactRequestRequestTypeDef,
-    AssociateDiscoveredResourceRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
-    ListApplicationStatesResultTypeDef,
-    ListCreatedArtifactsResultTypeDef,
-    ListDiscoveredResourcesResultTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
-    ListMigrationTasksResultTypeDef,
-    ListProgressUpdateStreamsResultTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
-    MigrationTaskTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
-    NotifyMigrationTaskStateRequestRequestTypeDef,
-    DescribeMigrationTaskResultTypeDef,
-)
+from types_aiobotocore_mgh.type_defs import ApplicationStateTypeDef
 
 
 def get_value() -> ApplicationStateTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mgh-2.5.2.post1/README.md` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mgh
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mgh type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mgh"></a>
 
 # types-aiobotocore-mgh
 
 [![PyPI - types-aiobotocore-mgh](https://img.shields.io/pypi/v/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
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
 [types-aiobotocore-mgh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -275,86 +307,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mgh.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `MigrationHub` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/literals/).
+
 ```python
-from types_aiobotocore_mgh.literals import (
-    ApplicationStatusType,
-    ListApplicationStatesPaginatorName,
-    ListCreatedArtifactsPaginatorName,
-    ListDiscoveredResourcesPaginatorName,
-    ListMigrationTasksPaginatorName,
-    ListProgressUpdateStreamsPaginatorName,
-    ResourceAttributeTypeType,
-    StatusType,
-    MigrationHubServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mgh.literals import ApplicationStatusType
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mgh.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MigrationHub` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/type_defs/).
+
 ```python
-from types_aiobotocore_mgh.type_defs import (
-    ApplicationStateTypeDef,
-    CreatedArtifactTypeDef,
-    DiscoveredResourceTypeDef,
-    CreateProgressUpdateStreamRequestRequestTypeDef,
-    DeleteProgressUpdateStreamRequestRequestTypeDef,
-    DescribeApplicationStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeMigrationTaskRequestRequestTypeDef,
-    DisassociateCreatedArtifactRequestRequestTypeDef,
-    DisassociateDiscoveredResourceRequestRequestTypeDef,
-    ImportMigrationTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationStatesRequestRequestTypeDef,
-    ListCreatedArtifactsRequestRequestTypeDef,
-    ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMigrationTasksRequestRequestTypeDef,
-    MigrationTaskSummaryTypeDef,
-    ListProgressUpdateStreamsRequestRequestTypeDef,
-    ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeTypeDef,
-    TaskTypeDef,
-    TimestampTypeDef,
-    AssociateCreatedArtifactRequestRequestTypeDef,
-    AssociateDiscoveredResourceRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
-    ListApplicationStatesResultTypeDef,
-    ListCreatedArtifactsResultTypeDef,
-    ListDiscoveredResourcesResultTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
-    ListMigrationTasksResultTypeDef,
-    ListProgressUpdateStreamsResultTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
-    MigrationTaskTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
-    NotifyMigrationTaskStateRequestRequestTypeDef,
-    DescribeMigrationTaskResultTypeDef,
-)
+from types_aiobotocore_mgh.type_defs import ApplicationStateTypeDef
 
 
 def get_value() -> ApplicationStateTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mgh-2.5.2.post1/setup.py` & `types-aiobotocore-mgh-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgh",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__init__.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__init__.pyi` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/__main__.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHub 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHub 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/client.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/client.pyi` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/literals.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
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
@@ -170,14 +171,15 @@
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
@@ -256,26 +258,28 @@
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

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/literals.pyi` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
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
@@ -168,14 +169,15 @@
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
@@ -254,26 +256,28 @@
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

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/paginator.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/paginator.pyi` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/type_defs.py` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh/type_defs.pyi` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post1/types_aiobotocore_mgh.egg-info/SOURCES.txt` & `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

