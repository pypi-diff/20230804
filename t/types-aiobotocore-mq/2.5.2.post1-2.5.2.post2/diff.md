# Comparing `tmp/types-aiobotocore-mq-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mq-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mq-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-mq-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-mq-2.5.2.post1.tar` & `types-aiobotocore-mq-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.901513 types-aiobotocore-mq-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-08-02 14:52:42.901513 types-aiobotocore-mq-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:42.901513 types-aiobotocore-mq-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.901513 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28037 2023-08-02 14:43:49.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27990 2023-08-02 14:43:49.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:48.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.901513 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:42.000000 types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11108 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      589 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      588 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18730 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18697 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9414 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9412 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1878 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1875 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28037 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27990 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      718 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mq-2.5.2.post1/LICENSE` & `types-aiobotocore-mq-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/README.md` & `types-aiobotocore-mq-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mq
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mq type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mq"></a>
 
 # types-aiobotocore-mq
 
 [![PyPI - types-aiobotocore-mq](https://img.shields.io/pypi/v/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
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
 [types-aiobotocore-mq docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -255,117 +287,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mq.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `MQ` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/literals/).
+
 ```python
-from types_aiobotocore_mq.literals import (
-    AuthenticationStrategyType,
-    BrokerStateType,
-    BrokerStorageTypeType,
-    ChangeTypeType,
-    DataReplicationModeType,
-    DayOfWeekType,
-    DeploymentModeType,
-    EngineTypeType,
-    ListBrokersPaginatorName,
-    PromoteModeType,
-    SanitizationWarningReasonType,
-    MQServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mq.literals import AuthenticationStrategyType
 
 
 def check_value(value: AuthenticationStrategyType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mq.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MQ` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/type_defs/).
+
 ```python
-from types_aiobotocore_mq.type_defs import (
-    ActionRequiredTypeDef,
-    AvailabilityZoneTypeDef,
-    EngineVersionTypeDef,
-    BrokerInstanceTypeDef,
-    BrokerSummaryTypeDef,
-    ConfigurationIdTypeDef,
-    ConfigurationRevisionTypeDef,
-    EncryptionOptionsTypeDef,
-    LdapServerMetadataInputTypeDef,
-    LogsTypeDef,
-    UserTypeDef,
-    WeeklyStartTimeTypeDef,
-    ResponseMetadataTypeDef,
-    CreateConfigurationRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    CreateUserRequestRequestTypeDef,
-    DataReplicationCounterpartTypeDef,
-    DeleteBrokerRequestRequestTypeDef,
-    DeleteTagsRequestRequestTypeDef,
-    DeleteUserRequestRequestTypeDef,
-    DescribeBrokerEngineTypesRequestRequestTypeDef,
-    DescribeBrokerInstanceOptionsRequestRequestTypeDef,
-    DescribeBrokerRequestRequestTypeDef,
-    LdapServerMetadataOutputTypeDef,
-    UserSummaryTypeDef,
-    DescribeConfigurationRequestRequestTypeDef,
-    DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeUserRequestRequestTypeDef,
-    UserPendingChangesTypeDef,
-    PaginatorConfigTypeDef,
-    ListBrokersRequestRequestTypeDef,
-    ListConfigurationRevisionsRequestRequestTypeDef,
-    ListConfigurationsRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    ListUsersRequestRequestTypeDef,
-    PendingLogsTypeDef,
-    PromoteRequestRequestTypeDef,
-    RebootBrokerRequestRequestTypeDef,
-    SanitizationWarningTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
-    UpdateUserRequestRequestTypeDef,
-    BrokerInstanceOptionTypeDef,
-    BrokerEngineTypeTypeDef,
-    ConfigurationsTypeDef,
-    ConfigurationTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
-    CreateBrokerResponseTypeDef,
-    CreateConfigurationResponseTypeDef,
-    DeleteBrokerResponseTypeDef,
-    DescribeConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersResponseTypeDef,
-    ListConfigurationRevisionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PromoteResponseTypeDef,
-    DataReplicationMetadataOutputTypeDef,
-    ListUsersResponseTypeDef,
-    DescribeUserResponseTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
-    LogsSummaryTypeDef,
-    UpdateConfigurationResponseTypeDef,
-    DescribeBrokerInstanceOptionsResponseTypeDef,
-    DescribeBrokerEngineTypesResponseTypeDef,
-    ListConfigurationsResponseTypeDef,
-    UpdateBrokerResponseTypeDef,
-    DescribeBrokerResponseTypeDef,
-)
+from types_aiobotocore_mq.type_defs import ActionRequiredTypeDef
 
 
 def get_value() -> ActionRequiredTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mq-2.5.2.post1/setup.py` & `types-aiobotocore-mq-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mq",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__init__.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__init__.pyi` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/__main__.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MQ 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MQ 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
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

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/client.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/client.pyi` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/literals.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthenticationStrategyType",
     "BrokerStateType",
     "BrokerStorageTypeType",
     "ChangeTypeType",
     "DataReplicationModeType",
     "DayOfWeekType",
@@ -34,15 +33,14 @@
     "MQServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthenticationStrategyType = Literal["LDAP", "SIMPLE"]
 BrokerStateType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CRITICAL_ACTION_REQUIRED",
     "DELETION_IN_PROGRESS",
     "REBOOT_IN_PROGRESS",
@@ -74,14 +72,15 @@
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
@@ -177,14 +176,15 @@
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
@@ -263,26 +263,28 @@
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

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/literals.pyi` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.py`

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
     "AuthenticationStrategyType",
     "BrokerStateType",
     "BrokerStorageTypeType",
     "ChangeTypeType",
     "DataReplicationModeType",
     "DayOfWeekType",
@@ -33,14 +34,15 @@
     "MQServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AuthenticationStrategyType = Literal["LDAP", "SIMPLE"]
 BrokerStateType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CRITICAL_ACTION_REQUIRED",
     "DELETION_IN_PROGRESS",
     "REBOOT_IN_PROGRESS",
@@ -72,14 +74,15 @@
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
@@ -175,14 +178,15 @@
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
@@ -261,26 +265,28 @@
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

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/paginator.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/paginator.pyi` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/type_defs.py` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq/type_defs.pyi` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post1/types_aiobotocore_mq.egg-info/SOURCES.txt` & `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

