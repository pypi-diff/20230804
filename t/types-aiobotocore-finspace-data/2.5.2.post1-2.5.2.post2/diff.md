# Comparing `tmp/types-aiobotocore-finspace-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-finspace-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-data-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-finspace-data-2.5.2.post1.tar` & `types-aiobotocore-finspace-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.225587 types-aiobotocore-finspace-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-08-02 14:52:17.217588 types-aiobotocore-finspace-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16124 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:17.225587 types-aiobotocore-finspace-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.217588 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35921 2023-08-02 14:38:46.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35866 2023-08-02 14:38:44.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.217588 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:17.000000 types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.264173 types-aiobotocore-finspace-data-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-08-04 12:00:53.260173 types-aiobotocore-finspace-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:53.264173 types-aiobotocore-finspace-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.256173 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27152 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34473 2023-08-04 11:46:14.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-08-04 11:46:14.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:13.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.260173 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/LICENSE` & `types-aiobotocore-finspace-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/README.md` & `types-aiobotocore-finspace-data-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-finspace-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.FinSpaceData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore finspace-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-finspace-data"></a>
 
 # types-aiobotocore-finspace-data
 
 [![PyPI - types-aiobotocore-finspace-data](https://img.shields.io/pypi/v/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
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
 [types-aiobotocore-finspace-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,149 +301,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_finspace_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `FinSpaceData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/literals/).
+
 ```python
-from types_aiobotocore_finspace_data.literals import (
-    ApiAccessType,
-    ApplicationPermissionType,
-    ChangeTypeType,
-    ColumnDataTypeType,
-    DataViewStatusType,
-    DatasetKindType,
-    DatasetStatusType,
-    ErrorCategoryType,
-    ExportFileFormatType,
-    IngestionStatusType,
-    ListChangesetsPaginatorName,
-    ListDataViewsPaginatorName,
-    ListDatasetsPaginatorName,
-    ListPermissionGroupsPaginatorName,
-    ListUsersPaginatorName,
-    PermissionGroupMembershipStatusType,
-    UserStatusType,
-    UserTypeType,
-    locationTypeType,
-    FinSpaceDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_finspace_data.literals import ApiAccessType
 
 
 def check_value(value: ApiAccessType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_finspace_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `FinSpaceData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/type_defs/).
+
 ```python
 from types_aiobotocore_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    AwsCredentialsTypeDef,
-    ChangesetErrorInfoTypeDef,
-    ColumnDefinitionTypeDef,
-    CreateChangesetRequestRequestTypeDef,
-    DataViewDestinationTypeParamsTypeDef,
-    DatasetOwnerInfoTypeDef,
-    CreatePermissionGroupRequestRequestTypeDef,
-    CreateUserRequestRequestTypeDef,
-    CredentialsTypeDef,
-    DataViewDestinationTypeParamsOutputTypeDef,
-    DataViewErrorInfoTypeDef,
-    DeleteDatasetRequestRequestTypeDef,
-    DeletePermissionGroupRequestRequestTypeDef,
-    DisableUserRequestRequestTypeDef,
-    DisassociateUserFromPermissionGroupRequestRequestTypeDef,
-    EnableUserRequestRequestTypeDef,
-    GetChangesetRequestRequestTypeDef,
-    GetDataViewRequestRequestTypeDef,
-    GetDatasetRequestRequestTypeDef,
-    GetExternalDataViewAccessDetailsRequestRequestTypeDef,
-    S3LocationTypeDef,
-    GetPermissionGroupRequestRequestTypeDef,
-    PermissionGroupTypeDef,
-    GetProgrammaticAccessCredentialsRequestRequestTypeDef,
-    GetUserRequestRequestTypeDef,
-    GetWorkingLocationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListChangesetsRequestRequestTypeDef,
-    ListDataViewsRequestRequestTypeDef,
-    ListDatasetsRequestRequestTypeDef,
-    ListPermissionGroupsByUserRequestRequestTypeDef,
-    PermissionGroupByUserTypeDef,
-    ListPermissionGroupsRequestRequestTypeDef,
-    ListUsersByPermissionGroupRequestRequestTypeDef,
-    UserByPermissionGroupTypeDef,
-    ListUsersRequestRequestTypeDef,
-    UserTypeDef,
-    ResourcePermissionTypeDef,
-    ResetUserPasswordRequestRequestTypeDef,
-    UpdateChangesetRequestRequestTypeDef,
-    UpdatePermissionGroupRequestRequestTypeDef,
-    UpdateUserRequestRequestTypeDef,
-    AssociateUserToPermissionGroupResponseTypeDef,
-    CreateChangesetResponseTypeDef,
-    CreateDataViewResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreatePermissionGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DeletePermissionGroupResponseTypeDef,
-    DisableUserResponseTypeDef,
-    DisassociateUserFromPermissionGroupResponseTypeDef,
-    EnableUserResponseTypeDef,
-    GetUserResponseTypeDef,
-    GetWorkingLocationResponseTypeDef,
-    ResetUserPasswordResponseTypeDef,
-    UpdateChangesetResponseTypeDef,
-    UpdateDatasetResponseTypeDef,
-    UpdatePermissionGroupResponseTypeDef,
-    UpdateUserResponseTypeDef,
-    ChangesetSummaryTypeDef,
-    GetChangesetResponseTypeDef,
-    SchemaDefinitionOutputTypeDef,
-    SchemaDefinitionTypeDef,
-    CreateDataViewRequestRequestTypeDef,
-    GetProgrammaticAccessCredentialsResponseTypeDef,
-    DataViewDestinationTypeParamsUnionTypeDef,
-    DataViewSummaryTypeDef,
-    GetDataViewResponseTypeDef,
-    GetExternalDataViewAccessDetailsResponseTypeDef,
-    GetPermissionGroupResponseTypeDef,
-    ListPermissionGroupsResponseTypeDef,
-    ListChangesetsRequestListChangesetsPaginateTypeDef,
-    ListDataViewsRequestListDataViewsPaginateTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
-    ListPermissionGroupsByUserResponseTypeDef,
-    ListUsersByPermissionGroupResponseTypeDef,
-    ListUsersResponseTypeDef,
-    PermissionGroupParamsTypeDef,
-    ListChangesetsResponseTypeDef,
-    SchemaUnionOutputTypeDef,
-    SchemaUnionTypeDef,
-    ListDataViewsResponseTypeDef,
-    DatasetTypeDef,
-    GetDatasetResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    SchemaUnionUnionTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
-    ListDatasetsResponseTypeDef,
 )
 
 
 def get_value() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/setup.py` & `types-aiobotocore-finspace-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FinSpaceData 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__init__.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__init__.pyi` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/__main__.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FinSpaceData 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.FinSpaceData 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/client.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    DataViewDestinationTypeParamsUnionTypeDef,
+    DataViewDestinationTypeParamsTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
     GetDatasetResponseTypeDef,
@@ -62,15 +62,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
-    SchemaUnionUnionTypeDef,
+    SchemaUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -161,15 +161,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_changeset)
         """
 
     async def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: DataViewDestinationTypeParamsUnionTypeDef,
+        destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -185,15 +185,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_dataset)
         """
@@ -473,15 +473,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_dataset)
         """
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/client.pyi` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    DataViewDestinationTypeParamsUnionTypeDef,
+    DataViewDestinationTypeParamsTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
     GetDatasetResponseTypeDef,
@@ -62,15 +62,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
-    SchemaUnionUnionTypeDef,
+    SchemaUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -152,15 +152,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_changeset)
         """
     async def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: DataViewDestinationTypeParamsUnionTypeDef,
+        destinationTypeParams: DataViewDestinationTypeParamsTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -175,15 +175,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#create_dataset)
         """
@@ -437,15 +437,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: SchemaUnionUnionTypeDef = ...
+        schemaDefinition: SchemaUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/client/#update_dataset)
         """
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/literals.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/literals.pyi` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/paginator.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/paginator.pyi` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/type_defs.py` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_finspace_data.type_defs import AssociateUserToPermissionGroupRequestRequestTypeDef
 
     data: AssociateUserToPermissionGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
     ColumnDataTypeType,
     DatasetKindType,
@@ -32,28 +32,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
     "DatasetOwnerInfoTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CredentialsTypeDef",
-    "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "GetChangesetRequestRequestTypeDef",
@@ -98,19 +96,17 @@
     "ResetUserPasswordResponseTypeDef",
     "UpdateChangesetResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
-    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
-    "DataViewDestinationTypeParamsUnionTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListChangesetsRequestListChangesetsPaginateTypeDef",
     "ListDataViewsRequestListDataViewsPaginateTypeDef",
@@ -118,21 +114,19 @@
     "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
-    "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "SchemaUnionUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -144,22 +138,20 @@
     "_OptionalAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class AssociateUserToPermissionGroupRequestRequestTypeDef(
     _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef,
     _OptionalAssociateUserToPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -210,21 +202,19 @@
     "_OptionalCreateChangesetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateChangesetRequestRequestTypeDef(
     _RequiredCreateChangesetRequestRequestTypeDef, _OptionalCreateChangesetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDataViewDestinationTypeParamsTypeDef = TypedDict(
     "_RequiredDataViewDestinationTypeParamsTypeDef",
     {
         "destinationType": str,
     },
 )
 _OptionalDataViewDestinationTypeParamsTypeDef = TypedDict(
@@ -232,21 +222,19 @@
     {
         "s3DestinationExportFileFormat": ExportFileFormatType,
         "s3DestinationExportFileFormatOptions": Mapping[str, str],
     },
     total=False,
 )
 
-
 class DataViewDestinationTypeParamsTypeDef(
     _RequiredDataViewDestinationTypeParamsTypeDef, _OptionalDataViewDestinationTypeParamsTypeDef
 ):
     pass
 
-
 DatasetOwnerInfoTypeDef = TypedDict(
     "DatasetOwnerInfoTypeDef",
     {
         "name": str,
         "phoneNumber": str,
         "email": str,
     },
@@ -265,22 +253,20 @@
     {
         "description": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreatePermissionGroupRequestRequestTypeDef(
     _RequiredCreatePermissionGroupRequestRequestTypeDef,
     _OptionalCreatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "emailAddress": str,
         "type": UserTypeType,
     },
 )
@@ -292,54 +278,29 @@
         "ApiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
     total=False,
 )
 
-_RequiredDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
-    "_RequiredDataViewDestinationTypeParamsOutputTypeDef",
-    {
-        "destinationType": str,
-    },
-)
-_OptionalDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
-    "_OptionalDataViewDestinationTypeParamsOutputTypeDef",
-    {
-        "s3DestinationExportFileFormat": ExportFileFormatType,
-        "s3DestinationExportFileFormatOptions": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class DataViewDestinationTypeParamsOutputTypeDef(
-    _RequiredDataViewDestinationTypeParamsOutputTypeDef,
-    _OptionalDataViewDestinationTypeParamsOutputTypeDef,
-):
-    pass
-
-
 DataViewErrorInfoTypeDef = TypedDict(
     "DataViewErrorInfoTypeDef",
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
@@ -355,64 +316,58 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeletePermissionGroupRequestRequestTypeDef(
     _RequiredDeletePermissionGroupRequestRequestTypeDef,
     _OptionalDeletePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisableUserRequestRequestTypeDef = TypedDict(
     "_RequiredDisableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalDisableUserRequestRequestTypeDef = TypedDict(
     "_OptionalDisableUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DisableUserRequestRequestTypeDef(
     _RequiredDisableUserRequestRequestTypeDef, _OptionalDisableUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "userId": str,
     },
 )
@@ -420,43 +375,39 @@
     "_OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DisassociateUserFromPermissionGroupRequestRequestTypeDef(
     _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef,
     _OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredEnableUserRequestRequestTypeDef = TypedDict(
     "_RequiredEnableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalEnableUserRequestRequestTypeDef = TypedDict(
     "_OptionalEnableUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class EnableUserRequestRequestTypeDef(
     _RequiredEnableUserRequestRequestTypeDef, _OptionalEnableUserRequestRequestTypeDef
 ):
     pass
 
-
 GetChangesetRequestRequestTypeDef = TypedDict(
     "GetChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
     },
 )
@@ -523,22 +474,20 @@
     "_OptionalGetProgrammaticAccessCredentialsRequestRequestTypeDef",
     {
         "durationInMinutes": int,
     },
     total=False,
 )
 
-
 class GetProgrammaticAccessCredentialsRequestRequestTypeDef(
     _RequiredGetProgrammaticAccessCredentialsRequestRequestTypeDef,
     _OptionalGetProgrammaticAccessCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 
@@ -571,21 +520,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListChangesetsRequestRequestTypeDef(
     _RequiredListChangesetsRequestRequestTypeDef, _OptionalListChangesetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListDataViewsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataViewsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestRequestTypeDef = TypedDict(
@@ -593,21 +540,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDataViewsRequestRequestTypeDef(
     _RequiredListDataViewsRequestRequestTypeDef, _OptionalListDataViewsRequestRequestTypeDef
 ):
     pass
 
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -624,22 +569,20 @@
     "_OptionalListPermissionGroupsByUserRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPermissionGroupsByUserRequestRequestTypeDef(
     _RequiredListPermissionGroupsByUserRequestRequestTypeDef,
     _OptionalListPermissionGroupsByUserRequestRequestTypeDef,
 ):
     pass
 
-
 PermissionGroupByUserTypeDef = TypedDict(
     "PermissionGroupByUserTypeDef",
     {
         "permissionGroupId": str,
         "name": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
@@ -656,22 +599,20 @@
     "_OptionalListPermissionGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListPermissionGroupsRequestRequestTypeDef(
     _RequiredListPermissionGroupsRequestRequestTypeDef,
     _OptionalListPermissionGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListUsersByPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersByPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "maxResults": int,
     },
 )
@@ -679,22 +620,20 @@
     "_OptionalListUsersByPermissionGroupRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListUsersByPermissionGroupRequestRequestTypeDef(
     _RequiredListUsersByPermissionGroupRequestRequestTypeDef,
     _OptionalListUsersByPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UserByPermissionGroupTypeDef = TypedDict(
     "UserByPermissionGroupTypeDef",
     {
         "userId": str,
         "status": UserStatusType,
         "firstName": str,
         "lastName": str,
@@ -717,21 +656,19 @@
     "_OptionalListUsersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "userId": str,
         "status": UserStatusType,
         "firstName": str,
         "lastName": str,
@@ -766,21 +703,19 @@
     "_OptionalResetUserPasswordRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class ResetUserPasswordRequestRequestTypeDef(
     _RequiredResetUserPasswordRequestRequestTypeDef, _OptionalResetUserPasswordRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateChangesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
         "sourceParams": Mapping[str, str],
         "formatParams": Mapping[str, str],
@@ -790,21 +725,19 @@
     "_OptionalUpdateChangesetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateChangesetRequestRequestTypeDef(
     _RequiredUpdateChangesetRequestRequestTypeDef, _OptionalUpdateChangesetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -814,22 +747,20 @@
         "description": str,
         "applicationPermissions": Sequence[ApplicationPermissionType],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdatePermissionGroupRequestRequestTypeDef(
     _RequiredUpdatePermissionGroupRequestRequestTypeDef,
     _OptionalUpdatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -841,21 +772,19 @@
         "apiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-
 AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
     "AssociateUserToPermissionGroupResponseTypeDef",
     {
         "statusCode": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1050,23 +979,14 @@
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaDefinitionOutputTypeDef = TypedDict(
-    "SchemaDefinitionOutputTypeDef",
-    {
-        "columns": List[ColumnDefinitionTypeDef],
-        "primaryKeyColumns": List[str],
-    },
-    total=False,
-)
-
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnDefinitionTypeDef],
         "primaryKeyColumns": Sequence[str],
     },
     total=False,
@@ -1087,45 +1007,40 @@
         "sortColumns": Sequence[str],
         "partitionColumns": Sequence[str],
         "asOfTimestamp": int,
     },
     total=False,
 )
 
-
 class CreateDataViewRequestRequestTypeDef(
     _RequiredCreateDataViewRequestRequestTypeDef, _OptionalCreateDataViewRequestRequestTypeDef
 ):
     pass
 
-
 GetProgrammaticAccessCredentialsResponseTypeDef = TypedDict(
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataViewDestinationTypeParamsUnionTypeDef = Union[
-    DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
-]
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
         "partitionColumns": List[str],
         "sortColumns": List[str],
         "status": DataViewStatusType,
         "errorInfo": DataViewErrorInfoTypeDef,
-        "destinationTypeProperties": DataViewDestinationTypeParamsOutputTypeDef,
+        "destinationTypeProperties": DataViewDestinationTypeParamsTypeDef,
         "autoUpdate": bool,
         "createTime": int,
         "lastModifiedTime": int,
     },
     total=False,
 )
 
@@ -1138,15 +1053,15 @@
         "asOfTimestamp": int,
         "errorInfo": DataViewErrorInfoTypeDef,
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
-        "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
+        "destinationTypeParams": DataViewDestinationTypeParamsTypeDef,
         "status": DataViewStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
@@ -1184,44 +1099,40 @@
     "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListChangesetsRequestListChangesetsPaginateTypeDef(
     _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
     _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
     "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
     "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDataViewsRequestListDataViewsPaginateTypeDef(
     _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
     _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
 ):
     pass
 
-
 ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1283,22 +1194,14 @@
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaUnionOutputTypeDef = TypedDict(
-    "SchemaUnionOutputTypeDef",
-    {
-        "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 SchemaUnionTypeDef = TypedDict(
     "SchemaUnionTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1308,26 +1211,51 @@
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "datasetTitle": str,
+        "kind": DatasetKindType,
+        "permissionGroupParams": PermissionGroupParamsTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "datasetDescription": str,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "alias": str,
+        "schemaDefinition": SchemaUnionTypeDef,
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "ownerInfo": DatasetOwnerInfoTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionOutputTypeDef,
+        "schemaDefinition": SchemaUnionTypeDef,
         "alias": str,
     },
     total=False,
 )
 
 GetDatasetResponseTypeDef = TypedDict(
     "GetDatasetResponseTypeDef",
@@ -1335,49 +1263,21 @@
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionOutputTypeDef,
+        "schemaDefinition": SchemaUnionTypeDef,
         "alias": str,
         "status": DatasetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "datasetTitle": str,
-        "kind": DatasetKindType,
-        "permissionGroupParams": PermissionGroupParamsTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
-        "alias": str,
-        "schemaDefinition": SchemaUnionTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
-SchemaUnionUnionTypeDef = Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
@@ -1389,21 +1289,19 @@
         "datasetDescription": str,
         "alias": str,
         "schemaDefinition": SchemaUnionTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data/type_defs.pyi` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_finspace_data.type_defs import AssociateUserToPermissionGroupRequestRequestTypeDef
 
     data: AssociateUserToPermissionGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
     ColumnDataTypeType,
     DatasetKindType,
@@ -32,27 +32,27 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
     "DatasetOwnerInfoTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "CredentialsTypeDef",
-    "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "GetChangesetRequestRequestTypeDef",
@@ -97,19 +97,17 @@
     "ResetUserPasswordResponseTypeDef",
     "UpdateChangesetResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
-    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
-    "DataViewDestinationTypeParamsUnionTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListChangesetsRequestListChangesetsPaginateTypeDef",
     "ListDataViewsRequestListDataViewsPaginateTypeDef",
@@ -117,21 +115,19 @@
     "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
-    "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "SchemaUnionUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -143,20 +139,22 @@
     "_OptionalAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class AssociateUserToPermissionGroupRequestRequestTypeDef(
     _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef,
     _OptionalAssociateUserToPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -207,19 +205,21 @@
     "_OptionalCreateChangesetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateChangesetRequestRequestTypeDef(
     _RequiredCreateChangesetRequestRequestTypeDef, _OptionalCreateChangesetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDataViewDestinationTypeParamsTypeDef = TypedDict(
     "_RequiredDataViewDestinationTypeParamsTypeDef",
     {
         "destinationType": str,
     },
 )
 _OptionalDataViewDestinationTypeParamsTypeDef = TypedDict(
@@ -227,19 +227,21 @@
     {
         "s3DestinationExportFileFormat": ExportFileFormatType,
         "s3DestinationExportFileFormatOptions": Mapping[str, str],
     },
     total=False,
 )
 
+
 class DataViewDestinationTypeParamsTypeDef(
     _RequiredDataViewDestinationTypeParamsTypeDef, _OptionalDataViewDestinationTypeParamsTypeDef
 ):
     pass
 
+
 DatasetOwnerInfoTypeDef = TypedDict(
     "DatasetOwnerInfoTypeDef",
     {
         "name": str,
         "phoneNumber": str,
         "email": str,
     },
@@ -258,20 +260,22 @@
     {
         "description": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreatePermissionGroupRequestRequestTypeDef(
     _RequiredCreatePermissionGroupRequestRequestTypeDef,
     _OptionalCreatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "emailAddress": str,
         "type": UserTypeType,
     },
 )
@@ -283,50 +287,31 @@
         "ApiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
     total=False,
 )
 
-_RequiredDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
-    "_RequiredDataViewDestinationTypeParamsOutputTypeDef",
-    {
-        "destinationType": str,
-    },
-)
-_OptionalDataViewDestinationTypeParamsOutputTypeDef = TypedDict(
-    "_OptionalDataViewDestinationTypeParamsOutputTypeDef",
-    {
-        "s3DestinationExportFileFormat": ExportFileFormatType,
-        "s3DestinationExportFileFormatOptions": Dict[str, str],
-    },
-    total=False,
-)
-
-class DataViewDestinationTypeParamsOutputTypeDef(
-    _RequiredDataViewDestinationTypeParamsOutputTypeDef,
-    _OptionalDataViewDestinationTypeParamsOutputTypeDef,
-):
-    pass
-
 DataViewErrorInfoTypeDef = TypedDict(
     "DataViewErrorInfoTypeDef",
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
@@ -342,58 +327,64 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeletePermissionGroupRequestRequestTypeDef(
     _RequiredDeletePermissionGroupRequestRequestTypeDef,
     _OptionalDeletePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisableUserRequestRequestTypeDef = TypedDict(
     "_RequiredDisableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalDisableUserRequestRequestTypeDef = TypedDict(
     "_OptionalDisableUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DisableUserRequestRequestTypeDef(
     _RequiredDisableUserRequestRequestTypeDef, _OptionalDisableUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "userId": str,
     },
 )
@@ -401,39 +392,43 @@
     "_OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DisassociateUserFromPermissionGroupRequestRequestTypeDef(
     _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef,
     _OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredEnableUserRequestRequestTypeDef = TypedDict(
     "_RequiredEnableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalEnableUserRequestRequestTypeDef = TypedDict(
     "_OptionalEnableUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class EnableUserRequestRequestTypeDef(
     _RequiredEnableUserRequestRequestTypeDef, _OptionalEnableUserRequestRequestTypeDef
 ):
     pass
 
+
 GetChangesetRequestRequestTypeDef = TypedDict(
     "GetChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
     },
 )
@@ -500,20 +495,22 @@
     "_OptionalGetProgrammaticAccessCredentialsRequestRequestTypeDef",
     {
         "durationInMinutes": int,
     },
     total=False,
 )
 
+
 class GetProgrammaticAccessCredentialsRequestRequestTypeDef(
     _RequiredGetProgrammaticAccessCredentialsRequestRequestTypeDef,
     _OptionalGetProgrammaticAccessCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 
@@ -546,19 +543,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListChangesetsRequestRequestTypeDef(
     _RequiredListChangesetsRequestRequestTypeDef, _OptionalListChangesetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListDataViewsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataViewsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestRequestTypeDef = TypedDict(
@@ -566,19 +565,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListDataViewsRequestRequestTypeDef(
     _RequiredListDataViewsRequestRequestTypeDef, _OptionalListDataViewsRequestRequestTypeDef
 ):
     pass
 
+
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -595,20 +596,22 @@
     "_OptionalListPermissionGroupsByUserRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPermissionGroupsByUserRequestRequestTypeDef(
     _RequiredListPermissionGroupsByUserRequestRequestTypeDef,
     _OptionalListPermissionGroupsByUserRequestRequestTypeDef,
 ):
     pass
 
+
 PermissionGroupByUserTypeDef = TypedDict(
     "PermissionGroupByUserTypeDef",
     {
         "permissionGroupId": str,
         "name": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
@@ -625,20 +628,22 @@
     "_OptionalListPermissionGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListPermissionGroupsRequestRequestTypeDef(
     _RequiredListPermissionGroupsRequestRequestTypeDef,
     _OptionalListPermissionGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListUsersByPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersByPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "maxResults": int,
     },
 )
@@ -646,20 +651,22 @@
     "_OptionalListUsersByPermissionGroupRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListUsersByPermissionGroupRequestRequestTypeDef(
     _RequiredListUsersByPermissionGroupRequestRequestTypeDef,
     _OptionalListUsersByPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UserByPermissionGroupTypeDef = TypedDict(
     "UserByPermissionGroupTypeDef",
     {
         "userId": str,
         "status": UserStatusType,
         "firstName": str,
         "lastName": str,
@@ -682,19 +689,21 @@
     "_OptionalListUsersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "userId": str,
         "status": UserStatusType,
         "firstName": str,
         "lastName": str,
@@ -729,19 +738,21 @@
     "_OptionalResetUserPasswordRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class ResetUserPasswordRequestRequestTypeDef(
     _RequiredResetUserPasswordRequestRequestTypeDef, _OptionalResetUserPasswordRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateChangesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
         "sourceParams": Mapping[str, str],
         "formatParams": Mapping[str, str],
@@ -751,19 +762,21 @@
     "_OptionalUpdateChangesetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateChangesetRequestRequestTypeDef(
     _RequiredUpdateChangesetRequestRequestTypeDef, _OptionalUpdateChangesetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -773,20 +786,22 @@
         "description": str,
         "applicationPermissions": Sequence[ApplicationPermissionType],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdatePermissionGroupRequestRequestTypeDef(
     _RequiredUpdatePermissionGroupRequestRequestTypeDef,
     _OptionalUpdatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -798,19 +813,21 @@
         "apiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+
 AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
     "AssociateUserToPermissionGroupResponseTypeDef",
     {
         "statusCode": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1005,23 +1022,14 @@
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaDefinitionOutputTypeDef = TypedDict(
-    "SchemaDefinitionOutputTypeDef",
-    {
-        "columns": List[ColumnDefinitionTypeDef],
-        "primaryKeyColumns": List[str],
-    },
-    total=False,
-)
-
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnDefinitionTypeDef],
         "primaryKeyColumns": Sequence[str],
     },
     total=False,
@@ -1042,43 +1050,42 @@
         "sortColumns": Sequence[str],
         "partitionColumns": Sequence[str],
         "asOfTimestamp": int,
     },
     total=False,
 )
 
+
 class CreateDataViewRequestRequestTypeDef(
     _RequiredCreateDataViewRequestRequestTypeDef, _OptionalCreateDataViewRequestRequestTypeDef
 ):
     pass
 
+
 GetProgrammaticAccessCredentialsResponseTypeDef = TypedDict(
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataViewDestinationTypeParamsUnionTypeDef = Union[
-    DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
-]
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
         "partitionColumns": List[str],
         "sortColumns": List[str],
         "status": DataViewStatusType,
         "errorInfo": DataViewErrorInfoTypeDef,
-        "destinationTypeProperties": DataViewDestinationTypeParamsOutputTypeDef,
+        "destinationTypeProperties": DataViewDestinationTypeParamsTypeDef,
         "autoUpdate": bool,
         "createTime": int,
         "lastModifiedTime": int,
     },
     total=False,
 )
 
@@ -1091,15 +1098,15 @@
         "asOfTimestamp": int,
         "errorInfo": DataViewErrorInfoTypeDef,
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
-        "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
+        "destinationTypeParams": DataViewDestinationTypeParamsTypeDef,
         "status": DataViewStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
@@ -1137,40 +1144,44 @@
     "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListChangesetsRequestListChangesetsPaginateTypeDef(
     _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
     _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
     "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
     "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDataViewsRequestListDataViewsPaginateTypeDef(
     _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
     _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
 ):
     pass
 
+
 ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1232,22 +1243,14 @@
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaUnionOutputTypeDef = TypedDict(
-    "SchemaUnionOutputTypeDef",
-    {
-        "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 SchemaUnionTypeDef = TypedDict(
     "SchemaUnionTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1257,26 +1260,53 @@
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "datasetTitle": str,
+        "kind": DatasetKindType,
+        "permissionGroupParams": PermissionGroupParamsTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "datasetDescription": str,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
+        "alias": str,
+        "schemaDefinition": SchemaUnionTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "ownerInfo": DatasetOwnerInfoTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionOutputTypeDef,
+        "schemaDefinition": SchemaUnionTypeDef,
         "alias": str,
     },
     total=False,
 )
 
 GetDatasetResponseTypeDef = TypedDict(
     "GetDatasetResponseTypeDef",
@@ -1284,47 +1314,21 @@
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
-        "schemaDefinition": SchemaUnionOutputTypeDef,
+        "schemaDefinition": SchemaUnionTypeDef,
         "alias": str,
         "status": DatasetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "datasetTitle": str,
-        "kind": DatasetKindType,
-        "permissionGroupParams": PermissionGroupParamsTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoTypeDef,
-        "alias": str,
-        "schemaDefinition": SchemaUnionTypeDef,
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-SchemaUnionUnionTypeDef = Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
@@ -1336,19 +1340,21 @@
         "datasetDescription": str,
         "alias": str,
         "schemaDefinition": SchemaUnionTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post1/types_aiobotocore_finspace_data.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-data-2.5.2.post2/types_aiobotocore_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

