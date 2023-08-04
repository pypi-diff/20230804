# Comparing `tmp/types-aiobotocore-codecatalyst-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codecatalyst-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codecatalyst-2.5.2.post1.tar` & `types-aiobotocore-codecatalyst-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.569625 types-aiobotocore-codecatalyst-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.569625 types-aiobotocore-codecatalyst-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-02 14:34:58.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34697 2023-08-02 14:34:59.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:57.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.557625 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:02.000000 types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.579537 types-aiobotocore-codecatalyst-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-08-04 12:00:36.579537 types-aiobotocore-codecatalyst-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.579537 types-aiobotocore-codecatalyst-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:42:13.000000 types-aiobotocore-codecatalyst-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.575537 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-08-04 11:42:15.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34697 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:14.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.579537 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:36.000000 types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/LICENSE` & `types-aiobotocore-codecatalyst-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,136 +315,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codecatalyst.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CodeCatalyst` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/literals/).
+
 ```python
-from types_aiobotocore_codecatalyst.literals import (
-    ComparisonOperatorType,
-    DevEnvironmentSessionTypeType,
-    DevEnvironmentStatusType,
-    FilterKeyType,
-    InstanceTypeType,
-    ListAccessTokensPaginatorName,
-    ListDevEnvironmentSessionsPaginatorName,
-    ListDevEnvironmentsPaginatorName,
-    ListEventLogsPaginatorName,
-    ListProjectsPaginatorName,
-    ListSourceRepositoriesPaginatorName,
-    ListSourceRepositoryBranchesPaginatorName,
-    ListSpacesPaginatorName,
-    OperationTypeType,
-    UserTypeType,
-    CodeCatalystServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codecatalyst.literals import ComparisonOperatorType
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codecatalyst.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeCatalyst` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/type_defs/).
+
 ```python
-from types_aiobotocore_codecatalyst.type_defs import (
-    AccessTokenSummaryTypeDef,
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    IdeConfigurationTypeDef,
-    PersistentStorageConfigurationTypeDef,
-    RepositoryInputTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    CreateSourceRepositoryBranchRequestRequestTypeDef,
-    DeleteAccessTokenRequestRequestTypeDef,
-    DeleteDevEnvironmentRequestRequestTypeDef,
-    DevEnvironmentAccessDetailsTypeDef,
-    DevEnvironmentRepositorySummaryTypeDef,
-    ExecuteCommandSessionConfigurationTypeDef,
-    DevEnvironmentSessionSummaryTypeDef,
-    IdeTypeDef,
-    PersistentStorageTypeDef,
-    EmailAddressTypeDef,
-    EventPayloadTypeDef,
-    ProjectInformationTypeDef,
-    UserIdentityTypeDef,
-    FilterTypeDef,
-    GetDevEnvironmentRequestRequestTypeDef,
-    GetProjectRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSpaceRequestRequestTypeDef,
-    GetSubscriptionRequestRequestTypeDef,
-    GetUserDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ProjectListFilterTypeDef,
-    ProjectSummaryTypeDef,
-    ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestRequestTypeDef,
-    ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestRequestTypeDef,
-    SpaceSummaryTypeDef,
-    StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentSessionRequestRequestTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    ListEventLogsRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
-    GetProjectResponseTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
-    GetSpaceResponseTypeDef,
-    GetSubscriptionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
-    StartDevEnvironmentResponseTypeDef,
-    StopDevEnvironmentResponseTypeDef,
-    StopDevEnvironmentSessionResponseTypeDef,
-    VerifySessionResponseTypeDef,
-    StartDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
-    CreateDevEnvironmentRequestRequestTypeDef,
-    StartDevEnvironmentSessionResponseTypeDef,
-    DevEnvironmentSessionConfigurationTypeDef,
-    ListDevEnvironmentSessionsResponseTypeDef,
-    DevEnvironmentSummaryTypeDef,
-    GetDevEnvironmentResponseTypeDef,
-    GetUserDetailsResponseTypeDef,
-    EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ListProjectsResponseTypeDef,
-    ListSourceRepositoriesResponseTypeDef,
-    ListSourceRepositoryBranchesResponseTypeDef,
-    ListSpacesResponseTypeDef,
-    StartDevEnvironmentSessionRequestRequestTypeDef,
-    ListDevEnvironmentsResponseTypeDef,
-    ListEventLogsResponseTypeDef,
-)
+from types_aiobotocore_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
 
 def get_value() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/setup.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecatalyst",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__init__.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/__main__.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCatalyst 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeCatalyst 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/client.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/literals.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/paginator.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.py` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst/type_defs.pyi` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
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
 [types-aiobotocore-codecatalyst docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,136 +315,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codecatalyst.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CodeCatalyst` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/literals/).
+
 ```python
-from types_aiobotocore_codecatalyst.literals import (
-    ComparisonOperatorType,
-    DevEnvironmentSessionTypeType,
-    DevEnvironmentStatusType,
-    FilterKeyType,
-    InstanceTypeType,
-    ListAccessTokensPaginatorName,
-    ListDevEnvironmentSessionsPaginatorName,
-    ListDevEnvironmentsPaginatorName,
-    ListEventLogsPaginatorName,
-    ListProjectsPaginatorName,
-    ListSourceRepositoriesPaginatorName,
-    ListSourceRepositoryBranchesPaginatorName,
-    ListSpacesPaginatorName,
-    OperationTypeType,
-    UserTypeType,
-    CodeCatalystServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codecatalyst.literals import ComparisonOperatorType
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codecatalyst.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeCatalyst` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/type_defs/).
+
 ```python
-from types_aiobotocore_codecatalyst.type_defs import (
-    AccessTokenSummaryTypeDef,
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    IdeConfigurationTypeDef,
-    PersistentStorageConfigurationTypeDef,
-    RepositoryInputTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    CreateSourceRepositoryBranchRequestRequestTypeDef,
-    DeleteAccessTokenRequestRequestTypeDef,
-    DeleteDevEnvironmentRequestRequestTypeDef,
-    DevEnvironmentAccessDetailsTypeDef,
-    DevEnvironmentRepositorySummaryTypeDef,
-    ExecuteCommandSessionConfigurationTypeDef,
-    DevEnvironmentSessionSummaryTypeDef,
-    IdeTypeDef,
-    PersistentStorageTypeDef,
-    EmailAddressTypeDef,
-    EventPayloadTypeDef,
-    ProjectInformationTypeDef,
-    UserIdentityTypeDef,
-    FilterTypeDef,
-    GetDevEnvironmentRequestRequestTypeDef,
-    GetProjectRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSpaceRequestRequestTypeDef,
-    GetSubscriptionRequestRequestTypeDef,
-    GetUserDetailsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ProjectListFilterTypeDef,
-    ProjectSummaryTypeDef,
-    ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestRequestTypeDef,
-    ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestRequestTypeDef,
-    SpaceSummaryTypeDef,
-    StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentSessionRequestRequestTypeDef,
-    CreateAccessTokenRequestRequestTypeDef,
-    ListEventLogsRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
-    GetProjectResponseTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
-    GetSpaceResponseTypeDef,
-    GetSubscriptionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
-    StartDevEnvironmentResponseTypeDef,
-    StopDevEnvironmentResponseTypeDef,
-    StopDevEnvironmentSessionResponseTypeDef,
-    VerifySessionResponseTypeDef,
-    StartDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
-    CreateDevEnvironmentRequestRequestTypeDef,
-    StartDevEnvironmentSessionResponseTypeDef,
-    DevEnvironmentSessionConfigurationTypeDef,
-    ListDevEnvironmentSessionsResponseTypeDef,
-    DevEnvironmentSummaryTypeDef,
-    GetDevEnvironmentResponseTypeDef,
-    GetUserDetailsResponseTypeDef,
-    EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ListProjectsResponseTypeDef,
-    ListSourceRepositoriesResponseTypeDef,
-    ListSourceRepositoryBranchesResponseTypeDef,
-    ListSpacesResponseTypeDef,
-    StartDevEnvironmentSessionRequestRequestTypeDef,
-    ListDevEnvironmentsResponseTypeDef,
-    ListEventLogsResponseTypeDef,
-)
+from types_aiobotocore_codecatalyst.type_defs import AccessTokenSummaryTypeDef
 
 
 def get_value() -> AccessTokenSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post1/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt` & `types-aiobotocore-codecatalyst-2.5.2.post2/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

