# Comparing `tmp/types-aiobotocore-ssm-sap-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ssm-sap-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-sap-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-sap-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-ssm-sap-2.5.2.post1.tar` & `types-aiobotocore-ssm-sap-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.369448 types-aiobotocore-ssm-sap-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-08-02 14:53:04.369448 types-aiobotocore-ssm-sap-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13704 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.369448 types-aiobotocore-ssm-sap-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 14:50:12.000000 types-aiobotocore-ssm-sap-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.369448 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-08-02 14:50:16.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:15.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.369448 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:53:04.000000 types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.616643 types-aiobotocore-ssm-sap-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13331 2023-08-04 13:59:27.616643 types-aiobotocore-ssm-sap-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11814 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.616643 types-aiobotocore-ssm-sap-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2071 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.606643 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1242 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1241 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      941 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17144 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17113 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10239 2023-08-04 13:54:28.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10237 2023-08-04 13:54:28.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5387 2023-08-04 13:54:28.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5381 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17040 2023-08-04 13:54:28.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17027 2023-08-04 13:54:28.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.606643 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13331 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      813 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/LICENSE` & `types-aiobotocore-ssm-sap-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ssm-sap-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-sap
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
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
 [types-aiobotocore-ssm-sap docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,100 +298,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ssm_sap.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `SsmSap` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/literals/).
+
 ```python
-from types_aiobotocore_ssm_sap.literals import (
-    ApplicationStatusType,
-    ApplicationTypeType,
-    ComponentStatusType,
-    ComponentTypeType,
-    CredentialTypeType,
-    DatabaseStatusType,
-    DatabaseTypeType,
-    FilterOperatorType,
-    HostRoleType,
-    ListApplicationsPaginatorName,
-    ListComponentsPaginatorName,
-    ListDatabasesPaginatorName,
-    ListOperationsPaginatorName,
-    OperationStatusType,
-    PermissionActionTypeType,
-    SsmSapServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_ssm_sap.literals import ApplicationDiscoveryStatusType
 
 
-def check_value(value: ApplicationStatusType) -> bool:
+def check_value(value: ApplicationDiscoveryStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ssm_sap.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SsmSap` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/type_defs/).
+
 ```python
-from types_aiobotocore_ssm_sap.type_defs import (
-    ApplicationCredentialTypeDef,
-    ApplicationSummaryTypeDef,
-    ApplicationTypeDef,
-    ComponentSummaryTypeDef,
-    HostTypeDef,
-    DatabaseSummaryTypeDef,
-    DeleteResourcePermissionInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeregisterApplicationInputRequestTypeDef,
-    FilterTypeDef,
-    GetApplicationInputRequestTypeDef,
-    GetComponentInputRequestTypeDef,
-    GetDatabaseInputRequestTypeDef,
-    GetOperationInputRequestTypeDef,
-    OperationTypeDef,
-    GetResourcePermissionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsInputRequestTypeDef,
-    ListComponentsInputRequestTypeDef,
-    ListDatabasesInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePermissionInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    DatabaseTypeDef,
-    RegisterApplicationInputRequestTypeDef,
-    UpdateApplicationSettingsInputRequestTypeDef,
-    ComponentTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
-    GetApplicationOutputTypeDef,
-    GetResourcePermissionOutputTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDatabasesOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
-    ListOperationsInputRequestTypeDef,
-    GetOperationOutputTypeDef,
-    ListOperationsOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
-    GetDatabaseOutputTypeDef,
-    GetComponentOutputTypeDef,
-)
+from types_aiobotocore_ssm_sap.type_defs import ApplicationCredentialTypeDef
 
 
 def get_value() -> ApplicationCredentialTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/README.md` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ssm-sap
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ssm-sap type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ssm-sap"></a>
 
 # types-aiobotocore-ssm-sap
 
 [![PyPI - types-aiobotocore-ssm-sap](https://img.shields.io/pypi/v/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-sap.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/)
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
 [types-aiobotocore-ssm-sap docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,100 +298,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ssm_sap.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `SsmSap` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/literals/).
+
 ```python
-from types_aiobotocore_ssm_sap.literals import (
-    ApplicationStatusType,
-    ApplicationTypeType,
-    ComponentStatusType,
-    ComponentTypeType,
-    CredentialTypeType,
-    DatabaseStatusType,
-    DatabaseTypeType,
-    FilterOperatorType,
-    HostRoleType,
-    ListApplicationsPaginatorName,
-    ListComponentsPaginatorName,
-    ListDatabasesPaginatorName,
-    ListOperationsPaginatorName,
-    OperationStatusType,
-    PermissionActionTypeType,
-    SsmSapServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_ssm_sap.literals import ApplicationDiscoveryStatusType
 
 
-def check_value(value: ApplicationStatusType) -> bool:
+def check_value(value: ApplicationDiscoveryStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ssm_sap.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SsmSap` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/type_defs/).
+
 ```python
-from types_aiobotocore_ssm_sap.type_defs import (
-    ApplicationCredentialTypeDef,
-    ApplicationSummaryTypeDef,
-    ApplicationTypeDef,
-    ComponentSummaryTypeDef,
-    HostTypeDef,
-    DatabaseSummaryTypeDef,
-    DeleteResourcePermissionInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeregisterApplicationInputRequestTypeDef,
-    FilterTypeDef,
-    GetApplicationInputRequestTypeDef,
-    GetComponentInputRequestTypeDef,
-    GetDatabaseInputRequestTypeDef,
-    GetOperationInputRequestTypeDef,
-    OperationTypeDef,
-    GetResourcePermissionInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsInputRequestTypeDef,
-    ListComponentsInputRequestTypeDef,
-    ListDatabasesInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePermissionInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    DatabaseTypeDef,
-    RegisterApplicationInputRequestTypeDef,
-    UpdateApplicationSettingsInputRequestTypeDef,
-    ComponentTypeDef,
-    DeleteResourcePermissionOutputTypeDef,
-    GetApplicationOutputTypeDef,
-    GetResourcePermissionOutputTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListComponentsOutputTypeDef,
-    ListDatabasesOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePermissionOutputTypeDef,
-    RegisterApplicationOutputTypeDef,
-    UpdateApplicationSettingsOutputTypeDef,
-    ListOperationsInputRequestTypeDef,
-    GetOperationOutputTypeDef,
-    ListOperationsOutputTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListComponentsInputListComponentsPaginateTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
-    ListOperationsInputListOperationsPaginateTypeDef,
-    GetDatabaseOutputTypeDef,
-    GetComponentOutputTypeDef,
-)
+from types_aiobotocore_ssm_sap.type_defs import ApplicationCredentialTypeDef
 
 
 def get_value() -> ApplicationCredentialTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/setup.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-sap",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SsmSap 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__init__.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__init__.pyi` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/__main__.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SsmSap 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SsmSap 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
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

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/client.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,28 +24,30 @@
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
+    BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
     GetApplicationOutputTypeDef,
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -280,14 +282,24 @@
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#register_application)
         """
 
+    async def start_application_refresh(
+        self, *, ApplicationId: str
+    ) -> StartApplicationRefreshOutputTypeDef:
+        """
+        Refreshes a registered application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#start_application_refresh)
+        """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#tag_resource)
         """
@@ -301,15 +313,16 @@
         """
 
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
-        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...
+        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
+        Backint: BackintConfigTypeDef = ...
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#update_application_settings)
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/client.pyi` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,30 @@
     ListApplicationsPaginator,
     ListComponentsPaginator,
     ListDatabasesPaginator,
     ListOperationsPaginator,
 )
 from .type_defs import (
     ApplicationCredentialTypeDef,
+    BackintConfigTypeDef,
     DeleteResourcePermissionOutputTypeDef,
     FilterTypeDef,
     GetApplicationOutputTypeDef,
     GetComponentOutputTypeDef,
     GetDatabaseOutputTypeDef,
     GetOperationOutputTypeDef,
     GetResourcePermissionOutputTypeDef,
     ListApplicationsOutputTypeDef,
     ListComponentsOutputTypeDef,
     ListDatabasesOutputTypeDef,
     ListOperationsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePermissionOutputTypeDef,
     RegisterApplicationOutputTypeDef,
+    StartApplicationRefreshOutputTypeDef,
     UpdateApplicationSettingsOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -258,14 +260,23 @@
     ) -> RegisterApplicationOutputTypeDef:
         """
         Register an SAP application with AWS Systems Manager for SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.register_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#register_application)
         """
+    async def start_application_refresh(
+        self, *, ApplicationId: str
+    ) -> StartApplicationRefreshOutputTypeDef:
+        """
+        Refreshes a registered application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.start_application_refresh)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#start_application_refresh)
+        """
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Creates tag for a resource by specifying the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#tag_resource)
         """
@@ -277,15 +288,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#untag_resource)
         """
     async def update_application_settings(
         self,
         *,
         ApplicationId: str,
         CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,
-        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...
+        CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,
+        Backint: BackintConfigTypeDef = ...
     ) -> UpdateApplicationSettingsOutputTypeDef:
         """
         Updates the settings of an application registered with AWS Systems Manager for
         SAP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client.update_application_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/client/#update_application_settings)
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/literals.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,68 +2,82 @@
 Type annotations for ssm-sap service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_ssm_sap.literals import ApplicationStatusType
+    from types_aiobotocore_ssm_sap.literals import ApplicationDiscoveryStatusType
 
-    data: ApplicationStatusType = "ACTIVATED"
+    data: ApplicationDiscoveryStatusType = "DELETING"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
+    "BackintModeType",
+    "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
     "CredentialTypeType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
+    "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
+ApplicationDiscoveryStatusType = Literal[
+    "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
+]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 ApplicationTypeType = Literal["HANA"]
-ComponentStatusType = Literal["ACTIVATED"]
-ComponentTypeType = Literal["HANA"]
+BackintModeType = Literal["AWSBackup"]
+ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
+ComponentStatusType = Literal[
+    "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
+]
+ComponentTypeType = Literal["HANA", "HANA_NODE"]
 CredentialTypeType = Literal["ADMIN"]
-DatabaseStatusType = Literal["RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
+DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationModeType = Literal[
+    "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
+]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
+ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -72,14 +86,15 @@
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
@@ -175,14 +190,15 @@
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
@@ -261,26 +277,28 @@
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

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/literals.pyi` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/literals.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,66 +2,84 @@
 Type annotations for ssm-sap service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_sap/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_ssm_sap.literals import ApplicationStatusType
+    from types_aiobotocore_ssm_sap.literals import ApplicationDiscoveryStatusType
 
-    data: ApplicationStatusType = "ACTIVATED"
+    data: ApplicationDiscoveryStatusType = "DELETING"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "ApplicationDiscoveryStatusType",
     "ApplicationStatusType",
     "ApplicationTypeType",
+    "BackintModeType",
+    "ClusterStatusType",
     "ComponentStatusType",
     "ComponentTypeType",
     "CredentialTypeType",
     "DatabaseStatusType",
     "DatabaseTypeType",
     "FilterOperatorType",
     "HostRoleType",
     "ListApplicationsPaginatorName",
     "ListComponentsPaginatorName",
     "ListDatabasesPaginatorName",
     "ListOperationsPaginatorName",
+    "OperationModeType",
     "OperationStatusType",
     "PermissionActionTypeType",
+    "ReplicationModeType",
     "SsmSapServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
+ApplicationDiscoveryStatusType = Literal[
+    "DELETING", "REFRESH_FAILED", "REGISTERING", "REGISTRATION_FAILED", "SUCCESS"
+]
 ApplicationStatusType = Literal[
     "ACTIVATED", "DELETING", "FAILED", "REGISTERING", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
 ]
 ApplicationTypeType = Literal["HANA"]
-ComponentStatusType = Literal["ACTIVATED"]
-ComponentTypeType = Literal["HANA"]
+BackintModeType = Literal["AWSBackup"]
+ClusterStatusType = Literal["MAINTENANCE", "NONE", "OFFLINE", "ONLINE", "STANDBY"]
+ComponentStatusType = Literal[
+    "ACTIVATED", "RUNNING", "RUNNING_WITH_ERROR", "STARTING", "STOPPED", "STOPPING", "UNDEFINED"
+]
+ComponentTypeType = Literal["HANA", "HANA_NODE"]
 CredentialTypeType = Literal["ADMIN"]
-DatabaseStatusType = Literal["RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
+DatabaseStatusType = Literal["ERROR", "RUNNING", "STARTING", "STOPPED", "UNKNOWN", "WARNING"]
 DatabaseTypeType = Literal["SYSTEM", "TENANT"]
 FilterOperatorType = Literal["Equals", "GreaterThanOrEquals", "LessThanOrEquals"]
 HostRoleType = Literal["LEADER", "STANDBY", "UNKNOWN", "WORKER"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListDatabasesPaginatorName = Literal["list_databases"]
 ListOperationsPaginatorName = Literal["list_operations"]
+OperationModeType = Literal[
+    "DELTA_DATASHIPPING", "LOGREPLAY", "LOGREPLAY_READACCESS", "NONE", "PRIMARY"
+]
 OperationStatusType = Literal["ERROR", "INPROGRESS", "SUCCESS"]
 PermissionActionTypeType = Literal["RESTORE"]
+ReplicationModeType = Literal["ASYNC", "NONE", "PRIMARY", "SYNC", "SYNCMEM"]
 SsmSapServiceName = Literal["ssm-sap"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -70,14 +88,15 @@
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
@@ -173,14 +192,15 @@
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
@@ -259,26 +279,28 @@
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

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/paginator.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/paginator.pyi` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/type_defs.py` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,26 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
+    ClusterStatusType,
+    ComponentStatusType,
+    ComponentTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationModeType,
     OperationStatusType,
+    ReplicationModeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -34,16 +40,19 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
+    "AssociatedHostTypeDef",
+    "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
+    "ResilienceTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
@@ -53,14 +62,15 @@
     "GetResourcePermissionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "StartApplicationRefreshInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
     "ComponentTypeDef",
     "DeleteResourcePermissionOutputTypeDef",
@@ -68,14 +78,15 @@
     "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePermissionOutputTypeDef",
     "RegisterApplicationOutputTypeDef",
+    "StartApplicationRefreshOutputTypeDef",
     "UpdateApplicationSettingsOutputTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
@@ -108,39 +119,72 @@
     "ApplicationTypeDef",
     {
         "Id": str,
         "Type": Literal["HANA"],
         "Arn": str,
         "AppRegistryArn": str,
         "Status": ApplicationStatusType,
+        "DiscoveryStatus": ApplicationDiscoveryStatusType,
         "Components": List[str],
         "LastUpdated": datetime,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AssociatedHostTypeDef = TypedDict(
+    "AssociatedHostTypeDef",
+    {
+        "Hostname": str,
+        "Ec2InstanceId": str,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+BackintConfigTypeDef = TypedDict(
+    "BackintConfigTypeDef",
+    {
+        "BackintMode": Literal["AWSBackup"],
+        "EnsureNoBackupInProcess": bool,
+    },
+)
+
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "ComponentType": Literal["HANA"],
+        "ComponentType": ComponentTypeType,
         "Tags": Dict[str, str],
+        "Arn": str,
     },
     total=False,
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "HostName": str,
-        "HostRole": HostRoleType,
         "HostIp": str,
+        "EC2InstanceId": str,
         "InstanceId": str,
+        "HostRole": HostRoleType,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+ResilienceTypeDef = TypedDict(
+    "ResilienceTypeDef",
+    {
+        "HsrTier": str,
+        "HsrReplicationMode": ReplicationModeType,
+        "HsrOperationMode": OperationModeType,
+        "ClusterStatus": ClusterStatusType,
     },
     total=False,
 )
 
 DatabaseSummaryTypeDef = TypedDict(
     "DatabaseSummaryTypeDef",
     {
@@ -332,14 +376,21 @@
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
+StartApplicationRefreshInputRequestTypeDef = TypedDict(
+    "StartApplicationRefreshInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -403,14 +454,15 @@
     },
 )
 _OptionalUpdateApplicationSettingsInputRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationSettingsInputRequestTypeDef",
     {
         "CredentialsToAddOrUpdate": Sequence[ApplicationCredentialTypeDef],
         "CredentialsToRemove": Sequence[ApplicationCredentialTypeDef],
+        "Backint": BackintConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
@@ -419,21 +471,29 @@
     pass
 
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "ComponentId": str,
+        "ParentComponent": str,
+        "ChildComponents": List[str],
         "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
+        "ComponentType": ComponentTypeType,
+        "Status": ComponentStatusType,
+        "SapHostname": str,
+        "SapKernelVersion": str,
+        "HdbVersion": str,
+        "Resilience": ResilienceTypeDef,
+        "AssociatedHost": AssociatedHostTypeDef,
         "Databases": List[str],
         "Hosts": List[HostTypeDef],
         "PrimaryHost": str,
         "LastUpdated": datetime,
+        "Arn": str,
     },
     total=False,
 )
 
 DeleteResourcePermissionOutputTypeDef = TypedDict(
     "DeleteResourcePermissionOutputTypeDef",
     {
@@ -507,14 +567,22 @@
     {
         "Application": ApplicationTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartApplicationRefreshOutputTypeDef = TypedDict(
+    "StartApplicationRefreshOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateApplicationSettingsOutputTypeDef = TypedDict(
     "UpdateApplicationSettingsOutputTypeDef",
     {
         "Message": str,
         "OperationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -619,10 +687,11 @@
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
+        "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap/type_defs.pyi` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,26 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
+    ApplicationDiscoveryStatusType,
     ApplicationStatusType,
+    ClusterStatusType,
+    ComponentStatusType,
+    ComponentTypeType,
     DatabaseStatusType,
     DatabaseTypeType,
     FilterOperatorType,
     HostRoleType,
+    OperationModeType,
     OperationStatusType,
+    ReplicationModeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -33,16 +39,19 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
+    "AssociatedHostTypeDef",
+    "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
+    "ResilienceTypeDef",
     "DatabaseSummaryTypeDef",
     "DeleteResourcePermissionInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeregisterApplicationInputRequestTypeDef",
     "FilterTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetComponentInputRequestTypeDef",
@@ -52,14 +61,15 @@
     "GetResourcePermissionInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsInputRequestTypeDef",
     "ListComponentsInputRequestTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutResourcePermissionInputRequestTypeDef",
+    "StartApplicationRefreshInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "DatabaseTypeDef",
     "RegisterApplicationInputRequestTypeDef",
     "UpdateApplicationSettingsInputRequestTypeDef",
     "ComponentTypeDef",
     "DeleteResourcePermissionOutputTypeDef",
@@ -67,14 +77,15 @@
     "GetResourcePermissionOutputTypeDef",
     "ListApplicationsOutputTypeDef",
     "ListComponentsOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePermissionOutputTypeDef",
     "RegisterApplicationOutputTypeDef",
+    "StartApplicationRefreshOutputTypeDef",
     "UpdateApplicationSettingsOutputTypeDef",
     "ListOperationsInputRequestTypeDef",
     "GetOperationOutputTypeDef",
     "ListOperationsOutputTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
@@ -107,39 +118,72 @@
     "ApplicationTypeDef",
     {
         "Id": str,
         "Type": Literal["HANA"],
         "Arn": str,
         "AppRegistryArn": str,
         "Status": ApplicationStatusType,
+        "DiscoveryStatus": ApplicationDiscoveryStatusType,
         "Components": List[str],
         "LastUpdated": datetime,
         "StatusMessage": str,
     },
     total=False,
 )
 
+AssociatedHostTypeDef = TypedDict(
+    "AssociatedHostTypeDef",
+    {
+        "Hostname": str,
+        "Ec2InstanceId": str,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+BackintConfigTypeDef = TypedDict(
+    "BackintConfigTypeDef",
+    {
+        "BackintMode": Literal["AWSBackup"],
+        "EnsureNoBackupInProcess": bool,
+    },
+)
+
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "ComponentType": Literal["HANA"],
+        "ComponentType": ComponentTypeType,
         "Tags": Dict[str, str],
+        "Arn": str,
     },
     total=False,
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "HostName": str,
-        "HostRole": HostRoleType,
         "HostIp": str,
+        "EC2InstanceId": str,
         "InstanceId": str,
+        "HostRole": HostRoleType,
+        "OsVersion": str,
+    },
+    total=False,
+)
+
+ResilienceTypeDef = TypedDict(
+    "ResilienceTypeDef",
+    {
+        "HsrTier": str,
+        "HsrReplicationMode": ReplicationModeType,
+        "HsrOperationMode": OperationModeType,
+        "ClusterStatus": ClusterStatusType,
     },
     total=False,
 )
 
 DatabaseSummaryTypeDef = TypedDict(
     "DatabaseSummaryTypeDef",
     {
@@ -327,14 +371,21 @@
     {
         "ActionType": Literal["RESTORE"],
         "SourceResourceArn": str,
         "ResourceArn": str,
     },
 )
 
+StartApplicationRefreshInputRequestTypeDef = TypedDict(
+    "StartApplicationRefreshInputRequestTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -396,35 +447,44 @@
     },
 )
 _OptionalUpdateApplicationSettingsInputRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationSettingsInputRequestTypeDef",
     {
         "CredentialsToAddOrUpdate": Sequence[ApplicationCredentialTypeDef],
         "CredentialsToRemove": Sequence[ApplicationCredentialTypeDef],
+        "Backint": BackintConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateApplicationSettingsInputRequestTypeDef(
     _RequiredUpdateApplicationSettingsInputRequestTypeDef,
     _OptionalUpdateApplicationSettingsInputRequestTypeDef,
 ):
     pass
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "ComponentId": str,
+        "ParentComponent": str,
+        "ChildComponents": List[str],
         "ApplicationId": str,
-        "ComponentType": Literal["HANA"],
-        "Status": Literal["ACTIVATED"],
+        "ComponentType": ComponentTypeType,
+        "Status": ComponentStatusType,
+        "SapHostname": str,
+        "SapKernelVersion": str,
+        "HdbVersion": str,
+        "Resilience": ResilienceTypeDef,
+        "AssociatedHost": AssociatedHostTypeDef,
         "Databases": List[str],
         "Hosts": List[HostTypeDef],
         "PrimaryHost": str,
         "LastUpdated": datetime,
+        "Arn": str,
     },
     total=False,
 )
 
 DeleteResourcePermissionOutputTypeDef = TypedDict(
     "DeleteResourcePermissionOutputTypeDef",
     {
@@ -498,14 +558,22 @@
     {
         "Application": ApplicationTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartApplicationRefreshOutputTypeDef = TypedDict(
+    "StartApplicationRefreshOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateApplicationSettingsOutputTypeDef = TypedDict(
     "UpdateApplicationSettingsOutputTypeDef",
     {
         "Message": str,
         "OperationIds": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -606,10 +674,11 @@
     },
 )
 
 GetComponentOutputTypeDef = TypedDict(
     "GetComponentOutputTypeDef",
     {
         "Component": ComponentTypeDef,
+        "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ssm-sap-2.5.2.post1/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-sap-2.5.2.post2/types_aiobotocore_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

