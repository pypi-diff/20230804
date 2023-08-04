# Comparing `tmp/types-aiobotocore-securitylake-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-securitylake-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securitylake-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-securitylake-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-securitylake-2.5.2.post1.tar` & `types-aiobotocore-securitylake-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15531 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.413462 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25772 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25275 2023-08-02 14:49:29.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:28.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.421462 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:59.000000 types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13657 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12119 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1369 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1368 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27925 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27881 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9101 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9099 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5746 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5740 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25502 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25477 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13657 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/LICENSE` & `types-aiobotocore-securitylake-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/PKG-INFO` & `types-aiobotocore-securitylake-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,125 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_securitylake.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SecurityLake` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/literals/).
+
 ```python
-from types_aiobotocore_securitylake.literals import (
-    AccessTypeType,
-    AwsLogSourceNameType,
-    DataLakeStatusType,
-    GetDataLakeSourcesPaginatorName,
-    HttpMethodType,
-    ListDataLakeExceptionsPaginatorName,
-    ListLogSourcesPaginatorName,
-    ListSubscribersPaginatorName,
-    SourceCollectionStatusType,
-    SubscriberStatusType,
-    SecurityLakeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_securitylake.literals import AccessTypeType
 
 
 def check_value(value: AccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_securitylake.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SecurityLake` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/type_defs/).
+
 ```python
-from types_aiobotocore_securitylake.type_defs import (
-    AwsIdentityTypeDef,
-    AwsLogSourceConfigurationTypeDef,
-    AwsLogSourceResourceTypeDef,
-    ResponseMetadataTypeDef,
-    CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CustomLogSourceAttributesTypeDef,
-    CustomLogSourceCrawlerConfigurationTypeDef,
-    CustomLogSourceProviderTypeDef,
-    DataLakeEncryptionConfigurationTypeDef,
-    DataLakeReplicationConfigurationTypeDef,
-    DataLakeExceptionTypeDef,
-    DataLakeLifecycleExpirationTypeDef,
-    DataLakeLifecycleTransitionTypeDef,
-    DataLakeReplicationConfigurationOutputTypeDef,
-    DataLakeSourceStatusTypeDef,
-    DataLakeUpdateExceptionTypeDef,
-    DeleteCustomLogSourceRequestRequestTypeDef,
-    DeleteDataLakeRequestRequestTypeDef,
-    DeleteSubscriberNotificationRequestRequestTypeDef,
-    DeleteSubscriberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    GetDataLakeSourcesRequestRequestTypeDef,
-    GetSubscriberRequestRequestTypeDef,
-    HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestRequestTypeDef,
-    ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestRequestTypeDef,
-    RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateAwsLogSourceRequestRequestTypeDef,
-    DeleteAwsLogSourceRequestRequestTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
-    CustomLogSourceConfigurationTypeDef,
-    CustomLogSourceResourceTypeDef,
-    ListDataLakeExceptionsResponseTypeDef,
-    DataLakeLifecycleConfigurationOutputTypeDef,
-    DataLakeLifecycleConfigurationTypeDef,
-    DataLakeSourceTypeDef,
-    DataLakeUpdateStatusTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
-    NotificationConfigurationTypeDef,
-    GetDataLakeOrganizationConfigurationResponseTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
-    CreateCustomLogSourceRequestRequestTypeDef,
-    CreateCustomLogSourceResponseTypeDef,
-    LogSourceResourceTypeDef,
-    DataLakeConfigurationTypeDef,
-    GetDataLakeSourcesResponseTypeDef,
-    DataLakeResourceTypeDef,
-    CreateSubscriberNotificationRequestRequestTypeDef,
-    UpdateSubscriberNotificationRequestRequestTypeDef,
-    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    CreateSubscriberRequestRequestTypeDef,
-    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
-    ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
-    UpdateSubscriberRequestRequestTypeDef,
-    CreateDataLakeRequestRequestTypeDef,
-    UpdateDataLakeRequestRequestTypeDef,
-    CreateDataLakeResponseTypeDef,
-    ListDataLakesResponseTypeDef,
-    UpdateDataLakeResponseTypeDef,
-    ListLogSourcesResponseTypeDef,
-    CreateSubscriberResponseTypeDef,
-    GetSubscriberResponseTypeDef,
-    ListSubscribersResponseTypeDef,
-    UpdateSubscriberResponseTypeDef,
-)
+from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
 
 def get_value() -> AwsIdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/setup.py` & `types-aiobotocore-securitylake-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securitylake",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__init__.pyi` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/__main__.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityLake 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SecurityLake 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,59 +32,57 @@
     AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     CreateDataLakeResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
     DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogSourceResourceTypeDef,
     NotificationConfigurationTypeDef,
+    TagTypeDef,
     UpdateDataLakeResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SecurityLakeClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class SecurityLakeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
     """
 
     meta: ClientMeta
@@ -93,41 +91,37 @@
     def exceptions(self) -> Exceptions:
         """
         SecurityLakeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#close)
         """
-
     async def create_aws_log_source(
         self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> CreateAwsLogSourceResponseTypeDef:
         """
         Adds a natively supported Amazon Web Service as an Amazon Security Lake source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_aws_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_aws_log_source)
         """
-
     async def create_custom_log_source(
         self,
         *,
         sourceName: str,
         configuration: CustomLogSourceConfigurationTypeDef = ...,
         eventClasses: Sequence[str] = ...,
         sourceVersion: str = ...
@@ -135,246 +129,222 @@
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_custom_log_source)
         """
-
     async def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
-        metaStoreManagerRoleArn: str
+        metaStoreManagerRoleArn: str,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake)
         """
-
     async def create_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
         exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Creates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_exception_subscription)
         """
-
     async def create_data_lake_organization_configuration(
-        self,
-        *,
-        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
         Automatically enables Amazon Security Lake for new member accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_organization_configuration)
         """
-
     async def create_subscriber(
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
-        subscriberDescription: str = ...
+        subscriberDescription: str = ...,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_subscriber)
         """
-
     async def create_subscriber_notification(
         self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
     ) -> CreateSubscriberNotificationResponseTypeDef:
         """
         Notifies the subscriber when new data is written to the data lake for the
         sources that the subscriber consumes in Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_subscriber_notification)
         """
-
     async def delete_aws_log_source(
         self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> DeleteAwsLogSourceResponseTypeDef:
         """
         Removes a natively supported Amazon Web Service as an Amazon Security Lake
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_aws_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_aws_log_source)
         """
-
     async def delete_custom_log_source(
         self, *, sourceName: str, sourceVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Removes a custom log source from Amazon Security Lake, to stop sending data from
         the custom source to Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_custom_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_custom_log_source)
         """
-
     async def delete_data_lake(self, *, regions: Sequence[str]) -> Dict[str, Any]:
         """
         When you disable Amazon Security Lake from your account, Security Lake is
         disabled in all Amazon Web Services Regions and it stops collecting data from
         your sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake)
         """
-
     async def delete_data_lake_exception_subscription(self) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_exception_subscription)
         """
-
     async def delete_data_lake_organization_configuration(
-        self,
-        *,
-        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Removes automatic the enablement of configuration settings for new member
-        accounts (but retains the settings for the delegated administrator) from Amazon
-        Security Lake.
+        Turns off automatic enablement of Amazon Security Lake for member accounts that
+        are added to an organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_organization_configuration)
         """
-
     async def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the subscription permission and all notification settings for accounts
         that are already enabled in Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_subscriber)
         """
-
     async def delete_subscriber_notification(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_subscriber_notification)
         """
-
     async def deregister_data_lake_delegated_administrator(self) -> Dict[str, Any]:
         """
         Deletes the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.deregister_data_lake_delegated_administrator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#deregister_data_lake_delegated_administrator)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#generate_presigned_url)
         """
-
     async def get_data_lake_exception_subscription(
         self,
     ) -> GetDataLakeExceptionSubscriptionResponseTypeDef:
         """
         Retrieves the details of exception notifications for the account in Amazon
         Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_exception_subscription)
         """
-
     async def get_data_lake_organization_configuration(
         self,
     ) -> GetDataLakeOrganizationConfigurationResponseTypeDef:
         """
         Retrieves the configuration that will be automatically set up for accounts added
         to the organization after the organization has onboarded to Amazon Security
         Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_organization_configuration)
         """
-
     async def get_data_lake_sources(
         self, *, accounts: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetDataLakeSourcesResponseTypeDef:
         """
         Retrieves a snapshot of the current Region, including whether Amazon Security
         Lake is enabled for those accounts and which sources Security Lake is collecting
         data from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_sources)
         """
-
     async def get_subscriber(self, *, subscriberId: str) -> GetSubscriberResponseTypeDef:
         """
         Retrieves the subscription information for the specified subscription ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_subscriber)
         """
-
     async def list_data_lake_exceptions(
         self, *, maxResults: int = ..., nextToken: str = ..., regions: Sequence[str] = ...
     ) -> ListDataLakeExceptionsResponseTypeDef:
         """
         Lists the Amazon Security Lake exceptions that you can use to find the source of
         problems and fix them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_data_lake_exceptions)
         """
-
     async def list_data_lakes(
         self, *, regions: Sequence[str] = ...
     ) -> ListDataLakesResponseTypeDef:
         """
         Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Web Services Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_data_lakes)
         """
-
     async def list_log_sources(
         self,
         *,
         accounts: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regions: Sequence[str] = ...,
@@ -382,59 +352,83 @@
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_log_sources)
         """
-
     async def list_subscribers(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSubscribersResponseTypeDef:
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_subscribers)
         """
+    async def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseTypeDef:
+        """
+        Retrieves the tags (keys and values) that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_tags_for_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_tags_for_resource)
+        """
     async def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
         Designates the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#register_data_lake_delegated_administrator)
         """
+    async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+        """
+        Adds or updates one or more tags that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.tag_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#tag_resource)
+        """
+    async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes one or more tags (keys and values) from an Amazon Security Lake
+        resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.untag_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#untag_resource)
+        """
     async def update_data_lake(
         self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
     ) -> UpdateDataLakeResponseTypeDef:
         """
         Specifies where to store your security data and for how long.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_data_lake)
         """
-
     async def update_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
         exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_data_lake_exception_subscription)
         """
-
     async def update_subscriber(
         self,
         *,
         subscriberId: str,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
         subscriberIdentity: AwsIdentityTypeDef = ...,
@@ -442,64 +436,57 @@
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber)
         """
-
     async def update_subscriber_notification(
         self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
     ) -> UpdateSubscriberNotificationResponseTypeDef:
         """
         Updates an existing notification method for the subscription (SQS or HTTPs
         endpoint) or switches the notification subscription endpoint for a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber_notification)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_data_lake_sources"]
     ) -> GetDataLakeSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_data_lake_exceptions"]
     ) -> ListDataLakeExceptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_log_sources"]) -> ListLogSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_subscribers"]
     ) -> ListSubscribersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "SecurityLakeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
         """
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/client.pyi` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,55 +32,61 @@
     AwsLogSourceConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateCustomLogSourceResponseTypeDef,
     CreateDataLakeResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     CustomLogSourceConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationTypeDef,
     DataLakeConfigurationTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogSourceResourceTypeDef,
     NotificationConfigurationTypeDef,
+    TagTypeDef,
     UpdateDataLakeResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SecurityLakeClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class SecurityLakeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
     """
 
     meta: ClientMeta
@@ -89,37 +95,41 @@
     def exceptions(self) -> Exceptions:
         """
         SecurityLakeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#close)
         """
+
     async def create_aws_log_source(
         self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> CreateAwsLogSourceResponseTypeDef:
         """
         Adds a natively supported Amazon Web Service as an Amazon Security Lake source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_aws_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_aws_log_source)
         """
+
     async def create_custom_log_source(
         self,
         *,
         sourceName: str,
         configuration: CustomLogSourceConfigurationTypeDef = ...,
         eventClasses: Sequence[str] = ...,
         sourceVersion: str = ...
@@ -127,225 +137,243 @@
         """
         Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
         Services Region where you want to create a custom source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_custom_log_source)
         """
+
     async def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
-        metaStoreManagerRoleArn: str
+        metaStoreManagerRoleArn: str,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake)
         """
+
     async def create_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
         exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Creates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_exception_subscription)
         """
+
     async def create_data_lake_organization_configuration(
-        self,
-        *,
-        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
         Automatically enables Amazon Security Lake for new member accounts in your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_data_lake_organization_configuration)
         """
+
     async def create_subscriber(
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
-        subscriberDescription: str = ...
+        subscriberDescription: str = ...,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_subscriber)
         """
+
     async def create_subscriber_notification(
         self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
     ) -> CreateSubscriberNotificationResponseTypeDef:
         """
         Notifies the subscriber when new data is written to the data lake for the
         sources that the subscriber consumes in Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#create_subscriber_notification)
         """
+
     async def delete_aws_log_source(
         self, *, sources: Sequence[AwsLogSourceConfigurationTypeDef]
     ) -> DeleteAwsLogSourceResponseTypeDef:
         """
         Removes a natively supported Amazon Web Service as an Amazon Security Lake
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_aws_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_aws_log_source)
         """
+
     async def delete_custom_log_source(
         self, *, sourceName: str, sourceVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Removes a custom log source from Amazon Security Lake, to stop sending data from
         the custom source to Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_custom_log_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_custom_log_source)
         """
+
     async def delete_data_lake(self, *, regions: Sequence[str]) -> Dict[str, Any]:
         """
         When you disable Amazon Security Lake from your account, Security Lake is
         disabled in all Amazon Web Services Regions and it stops collecting data from
         your sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake)
         """
+
     async def delete_data_lake_exception_subscription(self) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_exception_subscription)
         """
+
     async def delete_data_lake_organization_configuration(
-        self,
-        *,
-        autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef]
+        self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Removes automatic the enablement of configuration settings for new member
-        accounts (but retains the settings for the delegated administrator) from Amazon
-        Security Lake.
+        Turns off automatic enablement of Amazon Security Lake for member accounts that
+        are added to an organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_data_lake_organization_configuration)
         """
+
     async def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the subscription permission and all notification settings for accounts
         that are already enabled in Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_subscriber)
         """
+
     async def delete_subscriber_notification(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#delete_subscriber_notification)
         """
+
     async def deregister_data_lake_delegated_administrator(self) -> Dict[str, Any]:
         """
         Deletes the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.deregister_data_lake_delegated_administrator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#deregister_data_lake_delegated_administrator)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#generate_presigned_url)
         """
+
     async def get_data_lake_exception_subscription(
         self,
     ) -> GetDataLakeExceptionSubscriptionResponseTypeDef:
         """
         Retrieves the details of exception notifications for the account in Amazon
         Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_exception_subscription)
         """
+
     async def get_data_lake_organization_configuration(
         self,
     ) -> GetDataLakeOrganizationConfigurationResponseTypeDef:
         """
         Retrieves the configuration that will be automatically set up for accounts added
         to the organization after the organization has onboarded to Amazon Security
         Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_organization_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_organization_configuration)
         """
+
     async def get_data_lake_sources(
         self, *, accounts: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetDataLakeSourcesResponseTypeDef:
         """
         Retrieves a snapshot of the current Region, including whether Amazon Security
         Lake is enabled for those accounts and which sources Security Lake is collecting
         data from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_data_lake_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_data_lake_sources)
         """
+
     async def get_subscriber(self, *, subscriberId: str) -> GetSubscriberResponseTypeDef:
         """
         Retrieves the subscription information for the specified subscription ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_subscriber)
         """
+
     async def list_data_lake_exceptions(
         self, *, maxResults: int = ..., nextToken: str = ..., regions: Sequence[str] = ...
     ) -> ListDataLakeExceptionsResponseTypeDef:
         """
         Lists the Amazon Security Lake exceptions that you can use to find the source of
         problems and fix them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_data_lake_exceptions)
         """
+
     async def list_data_lakes(
         self, *, regions: Sequence[str] = ...
     ) -> ListDataLakesResponseTypeDef:
         """
         Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Web Services Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_data_lakes)
         """
+
     async def list_log_sources(
         self,
         *,
         accounts: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regions: Sequence[str] = ...,
@@ -353,54 +381,91 @@
     ) -> ListLogSourcesResponseTypeDef:
         """
         Retrieves the log sources in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_log_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_log_sources)
         """
+
     async def list_subscribers(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSubscribersResponseTypeDef:
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_subscribers)
         """
+
+    async def list_tags_for_resource(
+        self, *, resourceArn: str
+    ) -> ListTagsForResourceResponseTypeDef:
+        """
+        Retrieves the tags (keys and values) that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_tags_for_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#list_tags_for_resource)
+        """
+
     async def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
         Designates the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#register_data_lake_delegated_administrator)
         """
+
+    async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+        """
+        Adds or updates one or more tags that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.tag_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#tag_resource)
+        """
+
+    async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes one or more tags (keys and values) from an Amazon Security Lake
+        resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.untag_resource)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#untag_resource)
+        """
+
     async def update_data_lake(
         self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
     ) -> UpdateDataLakeResponseTypeDef:
         """
         Specifies where to store your security data and for how long.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_data_lake)
         """
+
     async def update_data_lake_exception_subscription(
         self,
         *,
         notificationEndpoint: str,
         subscriptionProtocol: str,
         exceptionTimeToLive: int = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified notification subscription in Amazon Security Lake for the
         organization you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake_exception_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_data_lake_exception_subscription)
         """
+
     async def update_subscriber(
         self,
         *,
         subscriberId: str,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
         subscriberDescription: str = ...,
         subscriberIdentity: AwsIdentityTypeDef = ...,
@@ -408,57 +473,64 @@
     ) -> UpdateSubscriberResponseTypeDef:
         """
         Updates an existing subscription for the given Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber)
         """
+
     async def update_subscriber_notification(
         self, *, configuration: NotificationConfigurationTypeDef, subscriberId: str
     ) -> UpdateSubscriberNotificationResponseTypeDef:
         """
         Updates an existing notification method for the subscription (SQS or HTTPs
         endpoint) or switches the notification subscription endpoint for a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_subscriber_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#update_subscriber_notification)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_data_lake_sources"]
     ) -> GetDataLakeSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_data_lake_exceptions"]
     ) -> ListDataLakeExceptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_log_sources"]) -> ListLogSourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_subscribers"]
     ) -> ListSubscribersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "SecurityLakeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/client/)
         """
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
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
@@ -165,14 +166,15 @@
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
@@ -251,26 +253,28 @@
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

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/literals.pyi` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
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
@@ -163,14 +164,15 @@
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
@@ -249,26 +251,28 @@
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

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/paginator.pyi` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.py` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
     data: AwsIdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessTypeType,
     AwsLogSourceNameType,
     DataLakeStatusType,
     HttpMethodType,
     SourceCollectionStatusType,
@@ -32,70 +32,71 @@
 
 __all__ = (
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
     "AwsLogSourceResourceTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "TagTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
     "DataLakeExceptionTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
-    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
     "ListSubscribersRequestRequestTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
-    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     "CreateAwsLogSourceResponseTypeDef",
     "CreateSubscriberNotificationResponseTypeDef",
     "DeleteAwsLogSourceResponseTypeDef",
     "GetDataLakeExceptionSubscriptionResponseTypeDef",
     "UpdateSubscriberNotificationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
-    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
-    "DataLakeAutoEnableNewAccountConfigurationUnionTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
     "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
@@ -180,14 +181,22 @@
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
     },
@@ -251,23 +260,14 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
-DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
-    "DataLakeReplicationConfigurationOutputTypeDef",
-    {
-        "regions": List[str],
-        "roleArn": str,
-    },
-    total=False,
-)
-
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
     total=False,
@@ -399,21 +399,36 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
         "subscriptionProtocol": str,
     },
 )
@@ -443,22 +458,14 @@
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
-DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
-    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
-    {
-        "region": str,
-        "sources": List[AwsLogSourceResourceTypeDef],
-    },
-)
-
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
@@ -501,14 +508,30 @@
     "UpdateSubscriberNotificationResponseTypeDef",
     {
         "subscriberEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
@@ -529,23 +552,14 @@
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
-    "DataLakeLifecycleConfigurationOutputTypeDef",
-    {
-        "expiration": DataLakeLifecycleExpirationTypeDef,
-        "transitions": List[DataLakeLifecycleTransitionTypeDef],
-    },
-    total=False,
-)
-
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
     },
     total=False,
@@ -603,26 +617,36 @@
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+    },
+)
+
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+    },
+)
+
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeAutoEnableNewAccountConfigurationUnionTypeDef = Union[
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
-]
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -701,16 +725,16 @@
     },
 )
 _OptionalDataLakeResourceTypeDef = TypedDict(
     "_OptionalDataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
     total=False,
 )
 
 
@@ -730,41 +754,28 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
-CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
-    },
-)
-
-DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
-    },
-)
-
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
@@ -859,21 +870,35 @@
 
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
 
-CreateDataLakeRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeRequestRequestTypeDef",
+_RequiredCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
+_OptionalCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateDataLakeRequestRequestTypeDef(
+    _RequiredCreateDataLakeRequestRequestTypeDef, _OptionalCreateDataLakeRequestRequestTypeDef
+):
+    pass
+
 
 UpdateDataLakeRequestRequestTypeDef = TypedDict(
     "UpdateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake/type_defs.pyi` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
     data: AwsIdentityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessTypeType,
     AwsLogSourceNameType,
     DataLakeStatusType,
     HttpMethodType,
     SourceCollectionStatusType,
@@ -31,70 +31,71 @@
 
 __all__ = (
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
     "AwsLogSourceResourceTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
+    "TagTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
     "DataLakeExceptionTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
-    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
     "ListSubscribersRequestRequestTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
-    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     "CreateAwsLogSourceResponseTypeDef",
     "CreateSubscriberNotificationResponseTypeDef",
     "DeleteAwsLogSourceResponseTypeDef",
     "GetDataLakeExceptionSubscriptionResponseTypeDef",
     "UpdateSubscriberNotificationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
-    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
-    "DataLakeAutoEnableNewAccountConfigurationUnionTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
     "LogSourceTypeDef",
     "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
@@ -175,14 +176,22 @@
 
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
     },
@@ -246,23 +255,14 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
-DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
-    "DataLakeReplicationConfigurationOutputTypeDef",
-    {
-        "regions": List[str],
-        "roleArn": str,
-    },
-    total=False,
-)
-
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
     total=False,
@@ -390,21 +390,36 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
         "subscriptionProtocol": str,
     },
 )
@@ -432,22 +447,14 @@
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
-DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
-    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
-    {
-        "region": str,
-        "sources": List[AwsLogSourceResourceTypeDef],
-    },
-)
-
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
@@ -490,14 +497,30 @@
     "UpdateSubscriberNotificationResponseTypeDef",
     {
         "subscriberEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
@@ -518,23 +541,14 @@
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
-    "DataLakeLifecycleConfigurationOutputTypeDef",
-    {
-        "expiration": DataLakeLifecycleExpirationTypeDef,
-        "transitions": List[DataLakeLifecycleTransitionTypeDef],
-    },
-    total=False,
-)
-
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
     },
     total=False,
@@ -592,26 +606,36 @@
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+    },
+)
+
+DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
+    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
+    {
+        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
+    },
+)
+
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeAutoEnableNewAccountConfigurationUnionTypeDef = Union[
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
-]
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -686,16 +710,16 @@
     },
 )
 _OptionalDataLakeResourceTypeDef = TypedDict(
     "_OptionalDataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
         "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
     total=False,
 )
 
 class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
@@ -713,41 +737,28 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
-CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
-    },
-)
-
-DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
-    "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    {
-        "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef],
-    },
-)
-
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
@@ -836,21 +847,33 @@
 )
 
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
-CreateDataLakeRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeRequestRequestTypeDef",
+_RequiredCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
+_OptionalCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDataLakeRequestRequestTypeDef(
+    _RequiredCreateDataLakeRequestRequestTypeDef, _OptionalCreateDataLakeRequestRequestTypeDef
+):
+    pass
 
 UpdateDataLakeRequestRequestTypeDef = TypedDict(
     "UpdateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/PKG-INFO` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
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
 [types-aiobotocore-securitylake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,125 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_securitylake.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SecurityLake` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/literals/).
+
 ```python
-from types_aiobotocore_securitylake.literals import (
-    AccessTypeType,
-    AwsLogSourceNameType,
-    DataLakeStatusType,
-    GetDataLakeSourcesPaginatorName,
-    HttpMethodType,
-    ListDataLakeExceptionsPaginatorName,
-    ListLogSourcesPaginatorName,
-    ListSubscribersPaginatorName,
-    SourceCollectionStatusType,
-    SubscriberStatusType,
-    SecurityLakeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_securitylake.literals import AccessTypeType
 
 
 def check_value(value: AccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_securitylake.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SecurityLake` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/type_defs/).
+
 ```python
-from types_aiobotocore_securitylake.type_defs import (
-    AwsIdentityTypeDef,
-    AwsLogSourceConfigurationTypeDef,
-    AwsLogSourceResourceTypeDef,
-    ResponseMetadataTypeDef,
-    CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CustomLogSourceAttributesTypeDef,
-    CustomLogSourceCrawlerConfigurationTypeDef,
-    CustomLogSourceProviderTypeDef,
-    DataLakeEncryptionConfigurationTypeDef,
-    DataLakeReplicationConfigurationTypeDef,
-    DataLakeExceptionTypeDef,
-    DataLakeLifecycleExpirationTypeDef,
-    DataLakeLifecycleTransitionTypeDef,
-    DataLakeReplicationConfigurationOutputTypeDef,
-    DataLakeSourceStatusTypeDef,
-    DataLakeUpdateExceptionTypeDef,
-    DeleteCustomLogSourceRequestRequestTypeDef,
-    DeleteDataLakeRequestRequestTypeDef,
-    DeleteSubscriberNotificationRequestRequestTypeDef,
-    DeleteSubscriberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    GetDataLakeSourcesRequestRequestTypeDef,
-    GetSubscriberRequestRequestTypeDef,
-    HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestRequestTypeDef,
-    ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestRequestTypeDef,
-    RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateAwsLogSourceRequestRequestTypeDef,
-    DeleteAwsLogSourceRequestRequestTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
-    CustomLogSourceConfigurationTypeDef,
-    CustomLogSourceResourceTypeDef,
-    ListDataLakeExceptionsResponseTypeDef,
-    DataLakeLifecycleConfigurationOutputTypeDef,
-    DataLakeLifecycleConfigurationTypeDef,
-    DataLakeSourceTypeDef,
-    DataLakeUpdateStatusTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
-    NotificationConfigurationTypeDef,
-    GetDataLakeOrganizationConfigurationResponseTypeDef,
-    DataLakeAutoEnableNewAccountConfigurationUnionTypeDef,
-    CreateCustomLogSourceRequestRequestTypeDef,
-    CreateCustomLogSourceResponseTypeDef,
-    LogSourceResourceTypeDef,
-    DataLakeConfigurationTypeDef,
-    GetDataLakeSourcesResponseTypeDef,
-    DataLakeResourceTypeDef,
-    CreateSubscriberNotificationRequestRequestTypeDef,
-    UpdateSubscriberNotificationRequestRequestTypeDef,
-    CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    CreateSubscriberRequestRequestTypeDef,
-    ListLogSourcesRequestListLogSourcesPaginateTypeDef,
-    ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
-    UpdateSubscriberRequestRequestTypeDef,
-    CreateDataLakeRequestRequestTypeDef,
-    UpdateDataLakeRequestRequestTypeDef,
-    CreateDataLakeResponseTypeDef,
-    ListDataLakesResponseTypeDef,
-    UpdateDataLakeResponseTypeDef,
-    ListLogSourcesResponseTypeDef,
-    CreateSubscriberResponseTypeDef,
-    GetSubscriberResponseTypeDef,
-    ListSubscribersResponseTypeDef,
-    UpdateSubscriberResponseTypeDef,
-)
+from types_aiobotocore_securitylake.type_defs import AwsIdentityTypeDef
 
 
 def get_value() -> AwsIdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post1/types_aiobotocore_securitylake.egg-info/SOURCES.txt` & `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

