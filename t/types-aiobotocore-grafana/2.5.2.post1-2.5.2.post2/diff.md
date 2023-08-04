# Comparing `tmp/types-aiobotocore-grafana-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-grafana-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-grafana-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-grafana-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-grafana-2.5.2.post1.tar` & `types-aiobotocore-grafana-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.553576 types-aiobotocore-grafana-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:37.000000 types-aiobotocore-grafana-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-08-02 14:52:21.553576 types-aiobotocore-grafana-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-08-02 14:39:37.000000 types-aiobotocore-grafana-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.553576 types-aiobotocore-grafana-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:39:37.000000 types-aiobotocore-grafana-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.553576 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-02 14:39:37.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21485 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-08-02 14:39:38.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:37.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.553576 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:21.000000 types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.468365 types-aiobotocore-grafana-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-08-04 12:00:58.468365 types-aiobotocore-grafana-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.468365 types-aiobotocore-grafana-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:47:08.000000 types-aiobotocore-grafana-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.460364 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-04 11:47:10.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-08-04 11:47:10.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-08-04 11:47:10.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:47:09.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.468365 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:58.000000 types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/LICENSE` & `types-aiobotocore-grafana-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/PKG-INFO` & `types-aiobotocore-grafana-2.5.2.post2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-grafana
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
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
 [types-aiobotocore-grafana docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,113 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_grafana.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ManagedGrafana` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/literals/).
+
 ```python
-from types_aiobotocore_grafana.literals import (
-    AccountAccessTypeType,
-    AuthenticationProviderTypesType,
-    DataSourceTypeType,
-    LicenseTypeType,
-    ListPermissionsPaginatorName,
-    ListWorkspacesPaginatorName,
-    NotificationDestinationTypeType,
-    PermissionTypeType,
-    RoleType,
-    SamlConfigurationStatusType,
-    UpdateActionType,
-    UserTypeType,
-    WorkspaceStatusType,
-    ManagedGrafanaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_grafana.literals import AccountAccessTypeType
 
 
 def check_value(value: AccountAccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_grafana.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ManagedGrafana` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/type_defs/).
+
 ```python
-from types_aiobotocore_grafana.type_defs import (
-    AssertionAttributesTypeDef,
-    AssociateLicenseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AwsSsoAuthenticationTypeDef,
-    AuthenticationSummaryTypeDef,
-    CreateWorkspaceApiKeyRequestRequestTypeDef,
-    NetworkAccessConfigurationTypeDef,
-    VpcConfigurationTypeDef,
-    DeleteWorkspaceApiKeyRequestRequestTypeDef,
-    DeleteWorkspaceRequestRequestTypeDef,
-    DescribeWorkspaceAuthenticationRequestRequestTypeDef,
-    DescribeWorkspaceConfigurationRequestRequestTypeDef,
-    DescribeWorkspaceRequestRequestTypeDef,
-    DisassociateLicenseRequestRequestTypeDef,
-    IdpMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ListPermissionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListWorkspacesRequestRequestTypeDef,
-    NetworkAccessConfigurationOutputTypeDef,
-    UserTypeDef,
-    RoleValuesOutputTypeDef,
-    RoleValuesTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateWorkspaceConfigurationRequestRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
-    CreateWorkspaceApiKeyResponseTypeDef,
-    DeleteWorkspaceApiKeyResponseTypeDef,
-    DescribeWorkspaceConfigurationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    WorkspaceSummaryTypeDef,
-    CreateWorkspaceRequestRequestTypeDef,
-    UpdateWorkspaceRequestRequestTypeDef,
-    ListPermissionsRequestListPermissionsPaginateTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    PermissionEntryTypeDef,
-    UpdateInstructionOutputTypeDef,
-    UpdateInstructionTypeDef,
-    SamlConfigurationOutputTypeDef,
-    SamlConfigurationTypeDef,
-    VpcConfigurationUnionTypeDef,
-    WorkspaceDescriptionTypeDef,
-    ListWorkspacesResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    UpdateErrorTypeDef,
-    UpdateInstructionUnionTypeDef,
-    SamlAuthenticationTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    AssociateLicenseResponseTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    DeleteWorkspaceResponseTypeDef,
-    DescribeWorkspaceResponseTypeDef,
-    DisassociateLicenseResponseTypeDef,
-    UpdateWorkspaceResponseTypeDef,
-    UpdatePermissionsResponseTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
-    AuthenticationDescriptionTypeDef,
-    DescribeWorkspaceAuthenticationResponseTypeDef,
-    UpdateWorkspaceAuthenticationResponseTypeDef,
-)
+from types_aiobotocore_grafana.type_defs import AssertionAttributesTypeDef
 
 
 def get_value() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/README.md` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-grafana
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore grafana type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-grafana"></a>
 
 # types-aiobotocore-grafana
 
 [![PyPI - types-aiobotocore-grafana](https://img.shields.io/pypi/v/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
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
 [types-aiobotocore-grafana docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -258,113 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_grafana.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ManagedGrafana` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/literals/).
+
 ```python
-from types_aiobotocore_grafana.literals import (
-    AccountAccessTypeType,
-    AuthenticationProviderTypesType,
-    DataSourceTypeType,
-    LicenseTypeType,
-    ListPermissionsPaginatorName,
-    ListWorkspacesPaginatorName,
-    NotificationDestinationTypeType,
-    PermissionTypeType,
-    RoleType,
-    SamlConfigurationStatusType,
-    UpdateActionType,
-    UserTypeType,
-    WorkspaceStatusType,
-    ManagedGrafanaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_grafana.literals import AccountAccessTypeType
 
 
 def check_value(value: AccountAccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_grafana.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ManagedGrafana` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/type_defs/).
+
 ```python
-from types_aiobotocore_grafana.type_defs import (
-    AssertionAttributesTypeDef,
-    AssociateLicenseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AwsSsoAuthenticationTypeDef,
-    AuthenticationSummaryTypeDef,
-    CreateWorkspaceApiKeyRequestRequestTypeDef,
-    NetworkAccessConfigurationTypeDef,
-    VpcConfigurationTypeDef,
-    DeleteWorkspaceApiKeyRequestRequestTypeDef,
-    DeleteWorkspaceRequestRequestTypeDef,
-    DescribeWorkspaceAuthenticationRequestRequestTypeDef,
-    DescribeWorkspaceConfigurationRequestRequestTypeDef,
-    DescribeWorkspaceRequestRequestTypeDef,
-    DisassociateLicenseRequestRequestTypeDef,
-    IdpMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ListPermissionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListWorkspacesRequestRequestTypeDef,
-    NetworkAccessConfigurationOutputTypeDef,
-    UserTypeDef,
-    RoleValuesOutputTypeDef,
-    RoleValuesTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateWorkspaceConfigurationRequestRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
-    CreateWorkspaceApiKeyResponseTypeDef,
-    DeleteWorkspaceApiKeyResponseTypeDef,
-    DescribeWorkspaceConfigurationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    WorkspaceSummaryTypeDef,
-    CreateWorkspaceRequestRequestTypeDef,
-    UpdateWorkspaceRequestRequestTypeDef,
-    ListPermissionsRequestListPermissionsPaginateTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    PermissionEntryTypeDef,
-    UpdateInstructionOutputTypeDef,
-    UpdateInstructionTypeDef,
-    SamlConfigurationOutputTypeDef,
-    SamlConfigurationTypeDef,
-    VpcConfigurationUnionTypeDef,
-    WorkspaceDescriptionTypeDef,
-    ListWorkspacesResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    UpdateErrorTypeDef,
-    UpdateInstructionUnionTypeDef,
-    SamlAuthenticationTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    AssociateLicenseResponseTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    DeleteWorkspaceResponseTypeDef,
-    DescribeWorkspaceResponseTypeDef,
-    DisassociateLicenseResponseTypeDef,
-    UpdateWorkspaceResponseTypeDef,
-    UpdatePermissionsResponseTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
-    AuthenticationDescriptionTypeDef,
-    DescribeWorkspaceAuthenticationResponseTypeDef,
-    UpdateWorkspaceAuthenticationResponseTypeDef,
-)
+from types_aiobotocore_grafana.type_defs import AssertionAttributesTypeDef
 
 
 def get_value() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/setup.py` & `types-aiobotocore-grafana-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-grafana",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__init__.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__init__.pyi` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/__main__.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ManagedGrafana 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/client.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateInstructionUnionTypeDef,
+    NetworkAccessConfigurationTypeDef,
+    SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -127,19 +127,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -286,35 +286,35 @@
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#untag_resource)
         """
 
     async def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_permissions)
         """
 
     async def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -326,15 +326,15 @@
         """
 
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationUnionTypeDef = ...
+        samlConfiguration: SamlConfigurationTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_authentication)
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/client.pyi` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
-    NetworkAccessConfigurationUnionTypeDef,
-    SamlConfigurationUnionTypeDef,
-    UpdateInstructionUnionTypeDef,
+    NetworkAccessConfigurationTypeDef,
+    SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -119,19 +119,19 @@
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
         configuration: str = ...,
         grafanaVersion: str = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         stackSetName: str = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> CreateWorkspaceResponseTypeDef:
@@ -264,34 +264,34 @@
         The `UntagResource` operation removes the association of the tag with the Amazon
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#untag_resource)
         """
     async def update_permissions(
-        self, *, updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef], workspaceId: str
+        self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_permissions)
         """
     async def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
-        networkAccessControl: NetworkAccessConfigurationUnionTypeDef = ...,
+        networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
         permissionType: PermissionTypeType = ...,
         removeNetworkAccessConfiguration: bool = ...,
         removeVpcConfiguration: bool = ...,
         stackSetName: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         workspaceDataSources: Sequence[DataSourceTypeType] = ...,
         workspaceDescription: str = ...,
         workspaceName: str = ...,
         workspaceNotificationDestinations: Sequence[Literal["SNS"]] = ...,
         workspaceOrganizationalUnits: Sequence[str] = ...,
         workspaceRoleArn: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
@@ -302,15 +302,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace)
         """
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
-        samlConfiguration: SamlConfigurationUnionTypeDef = ...
+        samlConfiguration: SamlConfigurationTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_authentication)
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/literals.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/literals.pyi` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/paginator.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/paginator.pyi` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/type_defs.py` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_grafana.type_defs import AssertionAttributesTypeDef
 
     data: AssertionAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -54,54 +54,45 @@
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "NetworkAccessConfigurationOutputTypeDef",
     "UserTypeDef",
-    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
-    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdateInstructionUnionTypeDef",
-    "SamlAuthenticationTypeDef",
-    "SamlConfigurationUnionTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "UpdatePermissionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
     "UpdatePermissionsRequestRequestTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -173,24 +164,24 @@
         "workspaceId": str,
     },
 )
 
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": Sequence[str],
-        "vpceIds": Sequence[str],
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "subnetIds": Sequence[str],
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
     },
 )
 
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
@@ -290,44 +281,27 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-NetworkAccessConfigurationOutputTypeDef = TypedDict(
-    "NetworkAccessConfigurationOutputTypeDef",
-    {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
-    },
-)
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
 
-RoleValuesOutputTypeDef = TypedDict(
-    "RoleValuesOutputTypeDef",
-    {
-        "admin": List[str],
-        "editor": List[str],
-    },
-    total=False,
-)
-
 RoleValuesTypeDef = TypedDict(
     "RoleValuesTypeDef",
     {
-        "admin": Sequence[str],
-        "editor": Sequence[str],
+        "admin": List[str],
+        "editor": List[str],
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -348,22 +322,14 @@
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
-
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -489,14 +455,57 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredWorkspaceDescriptionTypeDef = TypedDict(
+    "_RequiredWorkspaceDescriptionTypeDef",
+    {
+        "authentication": AuthenticationSummaryTypeDef,
+        "created": datetime,
+        "dataSources": List[DataSourceTypeType],
+        "endpoint": str,
+        "grafanaVersion": str,
+        "id": str,
+        "modified": datetime,
+        "status": WorkspaceStatusType,
+    },
+)
+_OptionalWorkspaceDescriptionTypeDef = TypedDict(
+    "_OptionalWorkspaceDescriptionTypeDef",
+    {
+        "accountAccessType": AccountAccessTypeType,
+        "description": str,
+        "freeTrialConsumed": bool,
+        "freeTrialExpiration": datetime,
+        "licenseExpiration": datetime,
+        "licenseType": LicenseTypeType,
+        "name": str,
+        "networkAccessControl": NetworkAccessConfigurationTypeDef,
+        "notificationDestinations": List[Literal["SNS"]],
+        "organizationRoleName": str,
+        "organizationalUnits": List[str],
+        "permissionType": PermissionTypeType,
+        "stackSetName": str,
+        "tags": Dict[str, str],
+        "vpcConfiguration": VpcConfigurationTypeDef,
+        "workspaceRoleArn": str,
+    },
+    total=False,
+)
+
+
+class WorkspaceDescriptionTypeDef(
+    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
+):
+    pass
+
+
 _RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
@@ -522,140 +531,108 @@
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-NetworkAccessConfigurationUnionTypeDef = Union[
-    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
 
-UpdateInstructionOutputTypeDef = TypedDict(
-    "UpdateInstructionOutputTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": List[UserTypeDef],
-    },
-)
-
 UpdateInstructionTypeDef = TypedDict(
     "UpdateInstructionTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
         "users": Sequence[UserTypeDef],
     },
 )
 
-_RequiredSamlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSamlConfigurationOutputTypeDef",
-    {
-        "idpMetadata": IdpMetadataTypeDef,
-    },
-)
-_OptionalSamlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSamlConfigurationOutputTypeDef",
-    {
-        "allowedOrganizations": List[str],
-        "assertionAttributes": AssertionAttributesTypeDef,
-        "loginValidityDuration": int,
-        "roleValues": RoleValuesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SamlConfigurationOutputTypeDef(
-    _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSamlConfigurationTypeDef = TypedDict(
     "_RequiredSamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationTypeDef = TypedDict(
     "_OptionalSamlConfigurationTypeDef",
     {
-        "allowedOrganizations": Sequence[str],
+        "allowedOrganizations": List[str],
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesTypeDef,
     },
     total=False,
 )
 
 
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-_RequiredWorkspaceDescriptionTypeDef = TypedDict(
-    "_RequiredWorkspaceDescriptionTypeDef",
+ListWorkspacesResponseTypeDef = TypedDict(
+    "ListWorkspacesResponseTypeDef",
     {
-        "authentication": AuthenticationSummaryTypeDef,
-        "created": datetime,
-        "dataSources": List[DataSourceTypeType],
-        "endpoint": str,
-        "grafanaVersion": str,
-        "id": str,
-        "modified": datetime,
-        "status": WorkspaceStatusType,
+        "nextToken": str,
+        "workspaces": List[WorkspaceSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWorkspaceDescriptionTypeDef = TypedDict(
-    "_OptionalWorkspaceDescriptionTypeDef",
+
+AssociateLicenseResponseTypeDef = TypedDict(
+    "AssociateLicenseResponseTypeDef",
     {
-        "accountAccessType": AccountAccessTypeType,
-        "description": str,
-        "freeTrialConsumed": bool,
-        "freeTrialExpiration": datetime,
-        "licenseExpiration": datetime,
-        "licenseType": LicenseTypeType,
-        "name": str,
-        "networkAccessControl": NetworkAccessConfigurationOutputTypeDef,
-        "notificationDestinations": List[Literal["SNS"]],
-        "organizationRoleName": str,
-        "organizationalUnits": List[str],
-        "permissionType": PermissionTypeType,
-        "stackSetName": str,
-        "tags": Dict[str, str],
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
-        "workspaceRoleArn": str,
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class WorkspaceDescriptionTypeDef(
-    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
-):
-    pass
+DeleteWorkspaceResponseTypeDef = TypedDict(
+    "DeleteWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DescribeWorkspaceResponseTypeDef = TypedDict(
+    "DescribeWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListWorkspacesResponseTypeDef = TypedDict(
-    "ListWorkspacesResponseTypeDef",
+DisassociateLicenseResponseTypeDef = TypedDict(
+    "DisassociateLicenseResponseTypeDef",
     {
-        "nextToken": str,
-        "workspaces": List[WorkspaceSummaryTypeDef],
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkspaceResponseTypeDef = TypedDict(
+    "UpdateWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
@@ -664,43 +641,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateErrorTypeDef = TypedDict(
     "UpdateErrorTypeDef",
     {
-        "causedBy": UpdateInstructionOutputTypeDef,
+        "causedBy": UpdateInstructionTypeDef,
         "code": int,
         "message": str,
     },
 )
 
-UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
     "_OptionalSamlAuthenticationTypeDef",
     {
-        "configuration": SamlConfigurationOutputTypeDef,
+        "configuration": SamlConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class SamlAuthenticationTypeDef(
     _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
 ):
     pass
 
 
-SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
 _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
     },
 )
@@ -716,78 +699,22 @@
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateLicenseResponseTypeDef = TypedDict(
-    "AssociateLicenseResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteWorkspaceResponseTypeDef = TypedDict(
-    "DeleteWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorkspaceResponseTypeDef = TypedDict(
-    "DescribeWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateLicenseResponseTypeDef = TypedDict(
-    "DisassociateLicenseResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkspaceResponseTypeDef = TypedDict(
-    "UpdateWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
-        "workspaceId": str,
-    },
-)
-
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
     },
 )
 _OptionalAuthenticationDescriptionTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana/type_defs.pyi` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_grafana.type_defs import AssertionAttributesTypeDef
 
     data: AssertionAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
@@ -53,54 +53,45 @@
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
-    "NetworkAccessConfigurationOutputTypeDef",
     "UserTypeDef",
-    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    "NetworkAccessConfigurationUnionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionOutputTypeDef",
     "UpdateInstructionTypeDef",
-    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdateInstructionUnionTypeDef",
-    "SamlAuthenticationTypeDef",
-    "SamlConfigurationUnionTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "UpdatePermissionsResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
     "UpdatePermissionsRequestRequestTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
@@ -170,24 +161,24 @@
         "workspaceId": str,
     },
 )
 
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": Sequence[str],
-        "vpceIds": Sequence[str],
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "subnetIds": Sequence[str],
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
     },
 )
 
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
@@ -285,44 +276,27 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-NetworkAccessConfigurationOutputTypeDef = TypedDict(
-    "NetworkAccessConfigurationOutputTypeDef",
-    {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
-    },
-)
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
 
-RoleValuesOutputTypeDef = TypedDict(
-    "RoleValuesOutputTypeDef",
-    {
-        "admin": List[str],
-        "editor": List[str],
-    },
-    total=False,
-)
-
 RoleValuesTypeDef = TypedDict(
     "RoleValuesTypeDef",
     {
-        "admin": Sequence[str],
-        "editor": Sequence[str],
+        "admin": List[str],
+        "editor": List[str],
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -343,22 +317,14 @@
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
-
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -478,14 +444,55 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+_RequiredWorkspaceDescriptionTypeDef = TypedDict(
+    "_RequiredWorkspaceDescriptionTypeDef",
+    {
+        "authentication": AuthenticationSummaryTypeDef,
+        "created": datetime,
+        "dataSources": List[DataSourceTypeType],
+        "endpoint": str,
+        "grafanaVersion": str,
+        "id": str,
+        "modified": datetime,
+        "status": WorkspaceStatusType,
+    },
+)
+_OptionalWorkspaceDescriptionTypeDef = TypedDict(
+    "_OptionalWorkspaceDescriptionTypeDef",
+    {
+        "accountAccessType": AccountAccessTypeType,
+        "description": str,
+        "freeTrialConsumed": bool,
+        "freeTrialExpiration": datetime,
+        "licenseExpiration": datetime,
+        "licenseType": LicenseTypeType,
+        "name": str,
+        "networkAccessControl": NetworkAccessConfigurationTypeDef,
+        "notificationDestinations": List[Literal["SNS"]],
+        "organizationRoleName": str,
+        "organizationalUnits": List[str],
+        "permissionType": PermissionTypeType,
+        "stackSetName": str,
+        "tags": Dict[str, str],
+        "vpcConfiguration": VpcConfigurationTypeDef,
+        "workspaceRoleArn": str,
+    },
+    total=False,
+)
+
+class WorkspaceDescriptionTypeDef(
+    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
+):
+    pass
+
 _RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
@@ -509,134 +516,106 @@
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-NetworkAccessConfigurationUnionTypeDef = Union[
-    NetworkAccessConfigurationTypeDef, NetworkAccessConfigurationOutputTypeDef
-]
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
         "user": UserTypeDef,
     },
 )
 
-UpdateInstructionOutputTypeDef = TypedDict(
-    "UpdateInstructionOutputTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": List[UserTypeDef],
-    },
-)
-
 UpdateInstructionTypeDef = TypedDict(
     "UpdateInstructionTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
         "users": Sequence[UserTypeDef],
     },
 )
 
-_RequiredSamlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSamlConfigurationOutputTypeDef",
+_RequiredSamlConfigurationTypeDef = TypedDict(
+    "_RequiredSamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
     },
 )
-_OptionalSamlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSamlConfigurationOutputTypeDef",
+_OptionalSamlConfigurationTypeDef = TypedDict(
+    "_OptionalSamlConfigurationTypeDef",
     {
         "allowedOrganizations": List[str],
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
-        "roleValues": RoleValuesOutputTypeDef,
+        "roleValues": RoleValuesTypeDef,
     },
     total=False,
 )
 
-class SamlConfigurationOutputTypeDef(
-    _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
+class SamlConfigurationTypeDef(
+    _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
-_RequiredSamlConfigurationTypeDef = TypedDict(
-    "_RequiredSamlConfigurationTypeDef",
+ListWorkspacesResponseTypeDef = TypedDict(
+    "ListWorkspacesResponseTypeDef",
     {
-        "idpMetadata": IdpMetadataTypeDef,
+        "nextToken": str,
+        "workspaces": List[WorkspaceSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSamlConfigurationTypeDef = TypedDict(
-    "_OptionalSamlConfigurationTypeDef",
+
+AssociateLicenseResponseTypeDef = TypedDict(
+    "AssociateLicenseResponseTypeDef",
     {
-        "allowedOrganizations": Sequence[str],
-        "assertionAttributes": AssertionAttributesTypeDef,
-        "loginValidityDuration": int,
-        "roleValues": RoleValuesTypeDef,
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SamlConfigurationTypeDef(
-    _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
-):
-    pass
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-_RequiredWorkspaceDescriptionTypeDef = TypedDict(
-    "_RequiredWorkspaceDescriptionTypeDef",
+DeleteWorkspaceResponseTypeDef = TypedDict(
+    "DeleteWorkspaceResponseTypeDef",
     {
-        "authentication": AuthenticationSummaryTypeDef,
-        "created": datetime,
-        "dataSources": List[DataSourceTypeType],
-        "endpoint": str,
-        "grafanaVersion": str,
-        "id": str,
-        "modified": datetime,
-        "status": WorkspaceStatusType,
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalWorkspaceDescriptionTypeDef = TypedDict(
-    "_OptionalWorkspaceDescriptionTypeDef",
+
+DescribeWorkspaceResponseTypeDef = TypedDict(
+    "DescribeWorkspaceResponseTypeDef",
     {
-        "accountAccessType": AccountAccessTypeType,
-        "description": str,
-        "freeTrialConsumed": bool,
-        "freeTrialExpiration": datetime,
-        "licenseExpiration": datetime,
-        "licenseType": LicenseTypeType,
-        "name": str,
-        "networkAccessControl": NetworkAccessConfigurationOutputTypeDef,
-        "notificationDestinations": List[Literal["SNS"]],
-        "organizationRoleName": str,
-        "organizationalUnits": List[str],
-        "permissionType": PermissionTypeType,
-        "stackSetName": str,
-        "tags": Dict[str, str],
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
-        "workspaceRoleArn": str,
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class WorkspaceDescriptionTypeDef(
-    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
-):
-    pass
+DisassociateLicenseResponseTypeDef = TypedDict(
+    "DisassociateLicenseResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListWorkspacesResponseTypeDef = TypedDict(
-    "ListWorkspacesResponseTypeDef",
+UpdateWorkspaceResponseTypeDef = TypedDict(
+    "UpdateWorkspaceResponseTypeDef",
     {
-        "nextToken": str,
-        "workspaces": List[WorkspaceSummaryTypeDef],
+        "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
@@ -645,41 +624,47 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateErrorTypeDef = TypedDict(
     "UpdateErrorTypeDef",
     {
-        "causedBy": UpdateInstructionOutputTypeDef,
+        "causedBy": UpdateInstructionTypeDef,
         "code": int,
         "message": str,
     },
 )
 
-UpdateInstructionUnionTypeDef = Union[UpdateInstructionTypeDef, UpdateInstructionOutputTypeDef]
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
     "_OptionalSamlAuthenticationTypeDef",
     {
-        "configuration": SamlConfigurationOutputTypeDef,
+        "configuration": SamlConfigurationTypeDef,
     },
     total=False,
 )
 
 class SamlAuthenticationTypeDef(
     _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
 ):
     pass
 
-SamlConfigurationUnionTypeDef = Union[SamlConfigurationTypeDef, SamlConfigurationOutputTypeDef]
 _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
         "authenticationProviders": Sequence[AuthenticationProviderTypesType],
         "workspaceId": str,
     },
 )
@@ -693,78 +678,22 @@
 
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
-AssociateLicenseResponseTypeDef = TypedDict(
-    "AssociateLicenseResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteWorkspaceResponseTypeDef = TypedDict(
-    "DeleteWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorkspaceResponseTypeDef = TypedDict(
-    "DescribeWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateLicenseResponseTypeDef = TypedDict(
-    "DisassociateLicenseResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkspaceResponseTypeDef = TypedDict(
-    "UpdateWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionUnionTypeDef],
-        "workspaceId": str,
-    },
-)
-
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
     },
 )
 _OptionalAuthenticationDescriptionTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-grafana-2.5.2.post1/types_aiobotocore_grafana.egg-info/SOURCES.txt` & `types-aiobotocore-grafana-2.5.2.post2/types_aiobotocore_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

