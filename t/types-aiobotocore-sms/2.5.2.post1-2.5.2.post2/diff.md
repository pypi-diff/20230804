# Comparing `tmp/types-aiobotocore-sms-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sms-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sms-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-sms-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-sms-2.5.2.post1.tar` & `types-aiobotocore-sms-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-08-02 14:49:52.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31295 2023-08-02 14:49:49.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:48.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.129454 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:01.000000 types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.736643 types-aiobotocore-sms-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13220 2023-08-04 13:59:26.736643 types-aiobotocore-sms-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11718 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.736643 types-aiobotocore-sms-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.736643 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1385 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1384 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27735 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27686 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11076 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11074 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6254 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6247 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28536 2023-08-04 13:53:48.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28519 2023-08-04 13:53:48.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:47.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.736643 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13220 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:26.000000 types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/LICENSE` & `types-aiobotocore-sms-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sms-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,158 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sms.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SMS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/literals/).
+
 ```python
-from types_aiobotocore_sms.literals import (
-    AppLaunchConfigurationStatusType,
-    AppLaunchStatusType,
-    AppReplicationConfigurationStatusType,
-    AppReplicationStatusType,
-    AppStatusType,
-    AppValidationStrategyType,
-    ConnectorCapabilityType,
-    ConnectorStatusType,
-    GetConnectorsPaginatorName,
-    GetReplicationJobsPaginatorName,
-    GetReplicationRunsPaginatorName,
-    GetServersPaginatorName,
-    LicenseTypeType,
-    ListAppsPaginatorName,
-    OutputFormatType,
-    ReplicationJobStateType,
-    ReplicationRunStateType,
-    ReplicationRunTypeType,
-    ScriptTypeType,
-    ServerCatalogStatusType,
-    ServerTypeType,
-    ServerValidationStrategyType,
-    ValidationStatusType,
-    VmManagerTypeType,
-    SMSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sms.literals import AppLaunchConfigurationStatusType
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sms.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SMS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/type_defs/).
+
 ```python
-from types_aiobotocore_sms.type_defs import (
-    LaunchDetailsTypeDef,
-    ConnectorTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    DeleteAppLaunchConfigurationRequestRequestTypeDef,
-    DeleteAppReplicationConfigurationRequestRequestTypeDef,
-    DeleteAppRequestRequestTypeDef,
-    DeleteAppValidationConfigurationRequestRequestTypeDef,
-    DeleteReplicationJobRequestRequestTypeDef,
-    DisassociateConnectorRequestRequestTypeDef,
-    GenerateChangeSetRequestRequestTypeDef,
-    S3LocationTypeDef,
-    GenerateTemplateRequestRequestTypeDef,
-    GetAppLaunchConfigurationRequestRequestTypeDef,
-    GetAppReplicationConfigurationRequestRequestTypeDef,
-    GetAppRequestRequestTypeDef,
-    GetAppValidationConfigurationRequestRequestTypeDef,
-    GetAppValidationOutputRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestRequestTypeDef,
-    VmServerAddressTypeDef,
-    ImportAppCatalogRequestRequestTypeDef,
-    LaunchAppRequestRequestTypeDef,
-    ListAppsRequestRequestTypeDef,
-    NotificationContextTypeDef,
-    ReplicationRunStageDetailsTypeDef,
-    ServerReplicationParametersOutputTypeDef,
-    StartAppReplicationRequestRequestTypeDef,
-    StartOnDemandAppReplicationRequestRequestTypeDef,
-    StartOnDemandReplicationRunRequestRequestTypeDef,
-    StopAppReplicationRequestRequestTypeDef,
-    TerminateAppRequestRequestTypeDef,
-    AppSummaryTypeDef,
-    CreateReplicationJobResponseTypeDef,
-    GetConnectorsResponseTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
-    ServerReplicationParametersTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
-    GenerateChangeSetResponseTypeDef,
-    GenerateTemplateResponseTypeDef,
-    SSMOutputTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
-    GetServersRequestGetServersPaginateTypeDef,
-    GetServersRequestRequestTypeDef,
-    VmServerTypeDef,
-    NotifyAppValidationOutputRequestRequestTypeDef,
-    ReplicationRunTypeDef,
-    ListAppsResponseTypeDef,
-    AppValidationOutputTypeDef,
-    SSMValidationParametersTypeDef,
-    UserDataValidationParametersTypeDef,
-    ServerTypeDef,
-    ReplicationJobTypeDef,
-    AppValidationConfigurationTypeDef,
-    GetServersResponseTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerGroupTypeDef,
-    ServerLaunchConfigurationTypeDef,
-    ServerReplicationConfigurationOutputTypeDef,
-    ServerReplicationConfigurationTypeDef,
-    ServerValidationConfigurationTypeDef,
-    ServerValidationOutputTypeDef,
-    GetReplicationJobsResponseTypeDef,
-    GetReplicationRunsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    GetAppResponseTypeDef,
-    UpdateAppResponseTypeDef,
-    ServerGroupUnionTypeDef,
-    ServerGroupLaunchConfigurationOutputTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationOutputTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupValidationConfigurationOutputTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
-    ValidationOutputTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
-    GetAppLaunchConfigurationResponseTypeDef,
-    ServerGroupLaunchConfigurationUnionTypeDef,
-    GetAppReplicationConfigurationResponseTypeDef,
-    ServerGroupReplicationConfigurationUnionTypeDef,
-    GetAppValidationConfigurationResponseTypeDef,
-    ServerGroupValidationConfigurationUnionTypeDef,
-    GetAppValidationOutputResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
-)
+from types_aiobotocore_sms.type_defs import LaunchDetailsTypeDef
 
 
 def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/setup.py` & `types-aiobotocore-sms-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sms",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__init__.pyi` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/__main__.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SMS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationUnionTypeDef,
-    ServerGroupReplicationConfigurationUnionTypeDef,
-    ServerGroupUnionTypeDef,
-    ServerGroupValidationConfigurationUnionTypeDef,
+    ServerGroupLaunchConfigurationTypeDef,
+    ServerGroupReplicationConfigurationTypeDef,
+    ServerGroupTypeDef,
+    ServerGroupValidationConfigurationTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
@@ -125,15 +125,15 @@
     async def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
@@ -399,29 +399,29 @@
 
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
 
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            ServerGroupReplicationConfigurationUnionTypeDef
+            ServerGroupReplicationConfigurationTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
@@ -429,15 +429,15 @@
 
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            ServerGroupValidationConfigurationUnionTypeDef
+            ServerGroupValidationConfigurationTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
@@ -492,15 +492,15 @@
     async def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/client.pyi` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationUnionTypeDef,
-    ServerGroupReplicationConfigurationUnionTypeDef,
-    ServerGroupUnionTypeDef,
-    ServerGroupValidationConfigurationUnionTypeDef,
+    ServerGroupLaunchConfigurationTypeDef,
+    ServerGroupReplicationConfigurationTypeDef,
+    ServerGroupTypeDef,
+    ServerGroupValidationConfigurationTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
@@ -118,15 +118,15 @@
     async def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#create_app)
@@ -366,43 +366,43 @@
         """
     async def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_launch_configuration)
         """
     async def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            ServerGroupReplicationConfigurationUnionTypeDef
+            ServerGroupReplicationConfigurationTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_replication_configuration)
         """
     async def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            ServerGroupValidationConfigurationUnionTypeDef
+            ServerGroupValidationConfigurationTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#put_app_validation_configuration)
@@ -451,15 +451,15 @@
     async def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
+        serverGroups: Sequence[ServerGroupTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/client/#update_app)
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,15 @@
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
@@ -239,14 +240,15 @@
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
@@ -325,26 +327,28 @@
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
@@ -487,29 +491,8 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_connectors", "get_replication_jobs", "get_replication_runs", "get_servers", "list_apps"
 ]
-RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
-    "ap-south-1",
-    "ap-southeast-1",
-    "ap-southeast-2",
-    "ca-central-1",
-    "eu-central-1",
-    "eu-north-1",
-    "eu-south-1",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
-]
+RegionName = Literal["us-west-2"]
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/literals.pyi` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,15 @@
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
@@ -237,14 +238,15 @@
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
@@ -323,26 +325,28 @@
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
@@ -485,29 +489,8 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "get_connectors", "get_replication_jobs", "get_replication_runs", "get_servers", "list_apps"
 ]
-RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
-    "ap-south-1",
-    "ap-southeast-1",
-    "ap-southeast-2",
-    "ca-central-1",
-    "eu-central-1",
-    "eu-north-1",
-    "eu-south-1",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
-]
+RegionName = Literal["us-west-2"]
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/paginator.pyi` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.py` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,26 +70,25 @@
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ServerReplicationParametersOutputTypeDef",
+    "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
-    "ServerReplicationParametersTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
@@ -105,46 +104,37 @@
     "AppValidationOutputTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
     "ServerTypeDef",
     "ReplicationJobTypeDef",
     "AppValidationConfigurationTypeDef",
     "GetServersResponseTypeDef",
-    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
-    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
+    "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "UpdateAppResponseTypeDef",
-    "ServerGroupUnionTypeDef",
-    "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
-    "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
-    "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "ServerGroupLaunchConfigurationUnionTypeDef",
-    "GetAppReplicationConfigurationResponseTypeDef",
-    "ServerGroupReplicationConfigurationUnionTypeDef",
-    "GetAppValidationConfigurationResponseTypeDef",
-    "ServerGroupValidationConfigurationUnionTypeDef",
-    "GetAppValidationOutputResponseTypeDef",
     "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "GetAppReplicationConfigurationResponseTypeDef",
     "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "GetAppValidationConfigurationResponseTypeDef",
     "PutAppValidationConfigurationRequestRequestTypeDef",
+    "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -405,16 +395,16 @@
     {
         "stage": str,
         "stageProgress": str,
     },
     total=False,
 )
 
-ServerReplicationParametersOutputTypeDef = TypedDict(
-    "ServerReplicationParametersOutputTypeDef",
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
@@ -568,28 +558,14 @@
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
 
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
-    {
-        "seedTime": TimestampTypeDef,
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationJobRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
@@ -868,24 +844,14 @@
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupOutputTypeDef = TypedDict(
-    "ServerGroupOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "name": str,
-        "serverList": List[ServerTypeDef],
-    },
-    total=False,
-)
-
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
         "serverList": Sequence[ServerTypeDef],
     },
@@ -907,23 +873,14 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
-ServerReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerReplicationConfigurationOutputTypeDef",
-    {
-        "server": ServerTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerReplicationConfigurationTypeDef = TypedDict(
     "ServerReplicationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
@@ -964,97 +921,94 @@
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
+    {
+        "appId": str,
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
-ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
-ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
-    },
-    total=False,
-)
-
-ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1065,127 +1019,87 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[ServerGroupUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 GetAppLaunchConfigurationResponseTypeDef = TypedDict(
     "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupLaunchConfigurationUnionTypeDef = Union[
-    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-]
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[
-            ServerGroupReplicationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupReplicationConfigurationUnionTypeDef = Union[
-    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
-]
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[
-            ServerGroupValidationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupValidationConfigurationUnionTypeDef = Union[
-    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
-]
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
-            ServerGroupReplicationConfigurationUnionTypeDef
+            ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": Sequence[
-            ServerGroupValidationConfigurationUnionTypeDef
-        ],
+        "serverGroupValidationConfigurations": Sequence[ServerGroupValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
+
+
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms/type_defs.pyi` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -69,26 +69,25 @@
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ServerReplicationParametersOutputTypeDef",
+    "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
-    "ServerReplicationParametersTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
@@ -104,46 +103,37 @@
     "AppValidationOutputTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
     "ServerTypeDef",
     "ReplicationJobTypeDef",
     "AppValidationConfigurationTypeDef",
     "GetServersResponseTypeDef",
-    "ServerGroupOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
-    "ServerReplicationConfigurationOutputTypeDef",
     "ServerReplicationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
+    "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "UpdateAppResponseTypeDef",
-    "ServerGroupUnionTypeDef",
-    "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
-    "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
-    "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "ServerGroupLaunchConfigurationUnionTypeDef",
-    "GetAppReplicationConfigurationResponseTypeDef",
-    "ServerGroupReplicationConfigurationUnionTypeDef",
-    "GetAppValidationConfigurationResponseTypeDef",
-    "ServerGroupValidationConfigurationUnionTypeDef",
-    "GetAppValidationOutputResponseTypeDef",
     "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "GetAppReplicationConfigurationResponseTypeDef",
     "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "GetAppValidationConfigurationResponseTypeDef",
     "PutAppValidationConfigurationRequestRequestTypeDef",
+    "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -402,16 +392,16 @@
     {
         "stage": str,
         "stageProgress": str,
     },
     total=False,
 )
 
-ServerReplicationParametersOutputTypeDef = TypedDict(
-    "ServerReplicationParametersOutputTypeDef",
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
     {
         "seedTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
@@ -559,28 +549,14 @@
 
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
-    {
-        "seedTime": TimestampTypeDef,
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationJobRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
@@ -853,24 +829,14 @@
         "serverCatalogStatus": ServerCatalogStatusType,
         "serverList": List[ServerTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupOutputTypeDef = TypedDict(
-    "ServerGroupOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "name": str,
-        "serverList": List[ServerTypeDef],
-    },
-    total=False,
-)
-
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
         "serverList": Sequence[ServerTypeDef],
     },
@@ -892,23 +858,14 @@
         "iamInstanceProfileName": str,
         "configureScript": S3LocationTypeDef,
         "configureScriptType": ScriptTypeType,
     },
     total=False,
 )
 
-ServerReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerReplicationConfigurationOutputTypeDef",
-    {
-        "server": ServerTypeDef,
-        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerReplicationConfigurationTypeDef = TypedDict(
     "ServerReplicationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
@@ -949,97 +906,94 @@
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppResponseTypeDef = TypedDict(
     "GetAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
+    {
+        "appId": str,
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupOutputTypeDef],
+        "serverGroups": List[ServerGroupTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
-ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupLaunchConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
-ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupReplicationConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
-    },
-    total=False,
-)
-
-ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
-    "ServerGroupValidationConfigurationOutputTypeDef",
-    {
-        "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1050,126 +1004,85 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[ServerGroupUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
 GetAppLaunchConfigurationResponseTypeDef = TypedDict(
     "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupLaunchConfigurationUnionTypeDef = Union[
-    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-]
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[
-            ServerGroupReplicationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupReplicationConfigurationUnionTypeDef = Union[
-    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
-]
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[
-            ServerGroupValidationConfigurationOutputTypeDef
-        ],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerGroupValidationConfigurationUnionTypeDef = Union[
-    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
-]
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
-            ServerGroupReplicationConfigurationUnionTypeDef
+            ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
+        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": Sequence[
-            ServerGroupValidationConfigurationUnionTypeDef
-        ],
+        "serverGroupValidationConfigurations": Sequence[ServerGroupValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
+
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/PKG-INFO` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SMS 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/
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
 [types-aiobotocore-sms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,158 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sms.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SMS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/literals/).
+
 ```python
-from types_aiobotocore_sms.literals import (
-    AppLaunchConfigurationStatusType,
-    AppLaunchStatusType,
-    AppReplicationConfigurationStatusType,
-    AppReplicationStatusType,
-    AppStatusType,
-    AppValidationStrategyType,
-    ConnectorCapabilityType,
-    ConnectorStatusType,
-    GetConnectorsPaginatorName,
-    GetReplicationJobsPaginatorName,
-    GetReplicationRunsPaginatorName,
-    GetServersPaginatorName,
-    LicenseTypeType,
-    ListAppsPaginatorName,
-    OutputFormatType,
-    ReplicationJobStateType,
-    ReplicationRunStateType,
-    ReplicationRunTypeType,
-    ScriptTypeType,
-    ServerCatalogStatusType,
-    ServerTypeType,
-    ServerValidationStrategyType,
-    ValidationStatusType,
-    VmManagerTypeType,
-    SMSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sms.literals import AppLaunchConfigurationStatusType
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sms.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SMS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms/type_defs/).
+
 ```python
-from types_aiobotocore_sms.type_defs import (
-    LaunchDetailsTypeDef,
-    ConnectorTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    DeleteAppLaunchConfigurationRequestRequestTypeDef,
-    DeleteAppReplicationConfigurationRequestRequestTypeDef,
-    DeleteAppRequestRequestTypeDef,
-    DeleteAppValidationConfigurationRequestRequestTypeDef,
-    DeleteReplicationJobRequestRequestTypeDef,
-    DisassociateConnectorRequestRequestTypeDef,
-    GenerateChangeSetRequestRequestTypeDef,
-    S3LocationTypeDef,
-    GenerateTemplateRequestRequestTypeDef,
-    GetAppLaunchConfigurationRequestRequestTypeDef,
-    GetAppReplicationConfigurationRequestRequestTypeDef,
-    GetAppRequestRequestTypeDef,
-    GetAppValidationConfigurationRequestRequestTypeDef,
-    GetAppValidationOutputRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestRequestTypeDef,
-    VmServerAddressTypeDef,
-    ImportAppCatalogRequestRequestTypeDef,
-    LaunchAppRequestRequestTypeDef,
-    ListAppsRequestRequestTypeDef,
-    NotificationContextTypeDef,
-    ReplicationRunStageDetailsTypeDef,
-    ServerReplicationParametersOutputTypeDef,
-    StartAppReplicationRequestRequestTypeDef,
-    StartOnDemandAppReplicationRequestRequestTypeDef,
-    StartOnDemandReplicationRunRequestRequestTypeDef,
-    StopAppReplicationRequestRequestTypeDef,
-    TerminateAppRequestRequestTypeDef,
-    AppSummaryTypeDef,
-    CreateReplicationJobResponseTypeDef,
-    GetConnectorsResponseTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
-    ServerReplicationParametersTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
-    GenerateChangeSetResponseTypeDef,
-    GenerateTemplateResponseTypeDef,
-    SSMOutputTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
-    GetServersRequestGetServersPaginateTypeDef,
-    GetServersRequestRequestTypeDef,
-    VmServerTypeDef,
-    NotifyAppValidationOutputRequestRequestTypeDef,
-    ReplicationRunTypeDef,
-    ListAppsResponseTypeDef,
-    AppValidationOutputTypeDef,
-    SSMValidationParametersTypeDef,
-    UserDataValidationParametersTypeDef,
-    ServerTypeDef,
-    ReplicationJobTypeDef,
-    AppValidationConfigurationTypeDef,
-    GetServersResponseTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerGroupTypeDef,
-    ServerLaunchConfigurationTypeDef,
-    ServerReplicationConfigurationOutputTypeDef,
-    ServerReplicationConfigurationTypeDef,
-    ServerValidationConfigurationTypeDef,
-    ServerValidationOutputTypeDef,
-    GetReplicationJobsResponseTypeDef,
-    GetReplicationRunsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    GetAppResponseTypeDef,
-    UpdateAppResponseTypeDef,
-    ServerGroupUnionTypeDef,
-    ServerGroupLaunchConfigurationOutputTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupReplicationConfigurationOutputTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupValidationConfigurationOutputTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
-    ValidationOutputTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
-    GetAppLaunchConfigurationResponseTypeDef,
-    ServerGroupLaunchConfigurationUnionTypeDef,
-    GetAppReplicationConfigurationResponseTypeDef,
-    ServerGroupReplicationConfigurationUnionTypeDef,
-    GetAppValidationConfigurationResponseTypeDef,
-    ServerGroupValidationConfigurationUnionTypeDef,
-    GetAppValidationOutputResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
-)
+from types_aiobotocore_sms.type_defs import LaunchDetailsTypeDef
 
 
 def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sms-2.5.2.post1/types_aiobotocore_sms.egg-info/SOURCES.txt` & `types-aiobotocore-sms-2.5.2.post2/types_aiobotocore_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

