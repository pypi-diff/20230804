# Comparing `tmp/types-aiobotocore-kafkaconnect-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kafkaconnect-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kafkaconnect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-kafkaconnect-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1.tar` & `types-aiobotocore-kafkaconnect-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.173555 types-aiobotocore-kafkaconnect-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-02 14:52:29.169555 types-aiobotocore-kafkaconnect-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:29.173555 types-aiobotocore-kafkaconnect-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.161555 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-08-02 14:41:17.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25532 2023-08-02 14:41:17.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-08-02 14:41:17.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:16.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.169555 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-02 14:52:28.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:29.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:28.000000 types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.486642 types-aiobotocore-kafkaconnect-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13539 2023-08-04 13:59:13.486642 types-aiobotocore-kafkaconnect-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12001 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.486642 types-aiobotocore-kafkaconnect-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.486642 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1173 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1172 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14157 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14133 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8999 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8997 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4431 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4426 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25532 2023-08-04 13:41:44.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25511 2023-08-04 13:41:44.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:43.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.486642 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13539 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:13.000000 types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/LICENSE` & `types-aiobotocore-kafkaconnect-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kafkaconnect-2.5.2.post2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafkaconnect
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KafkaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KafkaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,128 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kafkaconnect.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KafkaConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/literals/).
+
 ```python
-from types_aiobotocore_kafkaconnect.literals import (
-    ConnectorStateType,
-    CustomPluginContentTypeType,
-    CustomPluginStateType,
-    KafkaClusterClientAuthenticationTypeType,
-    KafkaClusterEncryptionInTransitTypeType,
-    ListConnectorsPaginatorName,
-    ListCustomPluginsPaginatorName,
-    ListWorkerConfigurationsPaginatorName,
-    KafkaConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kafkaconnect.literals import ConnectorStateType
 
 
 def check_value(value: ConnectorStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kafkaconnect.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KafkaConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/type_defs/).
+
 ```python
-from types_aiobotocore_kafkaconnect.type_defs import (
-    VpcDescriptionTypeDef,
-    VpcTypeDef,
-    ScaleInPolicyDescriptionTypeDef,
-    ScaleOutPolicyDescriptionTypeDef,
-    ScaleInPolicyTypeDef,
-    ScaleOutPolicyTypeDef,
-    ScaleInPolicyUpdateTypeDef,
-    ScaleOutPolicyUpdateTypeDef,
-    ProvisionedCapacityDescriptionTypeDef,
-    ProvisionedCapacityTypeDef,
-    ProvisionedCapacityUpdateTypeDef,
-    CloudWatchLogsLogDeliveryDescriptionTypeDef,
-    CloudWatchLogsLogDeliveryTypeDef,
-    KafkaClusterClientAuthenticationDescriptionTypeDef,
-    KafkaClusterEncryptionInTransitDescriptionTypeDef,
-    WorkerConfigurationDescriptionTypeDef,
-    KafkaClusterClientAuthenticationTypeDef,
-    KafkaClusterEncryptionInTransitTypeDef,
-    WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    CreateWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionSummaryTypeDef,
-    CustomPluginDescriptionTypeDef,
-    CustomPluginFileDescriptionTypeDef,
-    S3LocationDescriptionTypeDef,
-    S3LocationTypeDef,
-    CustomPluginTypeDef,
-    DeleteConnectorRequestRequestTypeDef,
-    DeleteCustomPluginRequestRequestTypeDef,
-    DescribeConnectorRequestRequestTypeDef,
-    StateDescriptionTypeDef,
-    DescribeCustomPluginRequestRequestTypeDef,
-    DescribeWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionDescriptionTypeDef,
-    FirehoseLogDeliveryDescriptionTypeDef,
-    FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
-    ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestRequestTypeDef,
-    S3LogDeliveryDescriptionTypeDef,
-    S3LogDeliveryTypeDef,
-    ApacheKafkaClusterDescriptionTypeDef,
-    ApacheKafkaClusterTypeDef,
-    AutoScalingDescriptionTypeDef,
-    AutoScalingTypeDef,
-    AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
-    CreateWorkerConfigurationResponseTypeDef,
-    WorkerConfigurationSummaryTypeDef,
-    PluginDescriptionTypeDef,
-    CustomPluginLocationDescriptionTypeDef,
-    CustomPluginLocationTypeDef,
-    PluginTypeDef,
-    DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
-    WorkerLogDeliveryDescriptionTypeDef,
-    WorkerLogDeliveryTypeDef,
-    KafkaClusterDescriptionTypeDef,
-    KafkaClusterTypeDef,
-    CapacityDescriptionTypeDef,
-    CapacityTypeDef,
-    CapacityUpdateTypeDef,
-    ListWorkerConfigurationsResponseTypeDef,
-    CustomPluginRevisionSummaryTypeDef,
-    CreateCustomPluginRequestRequestTypeDef,
-    LogDeliveryDescriptionTypeDef,
-    LogDeliveryTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
-    CustomPluginSummaryTypeDef,
-    DescribeCustomPluginResponseTypeDef,
-    ConnectorSummaryTypeDef,
-    DescribeConnectorResponseTypeDef,
-    CreateConnectorRequestRequestTypeDef,
-    ListCustomPluginsResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-)
+from types_aiobotocore_kafkaconnect.type_defs import VpcDescriptionTypeDef
 
 
 def get_value() -> VpcDescriptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/README.md` & `types-aiobotocore-kafkaconnect-2.5.2.post2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,128 +267,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kafkaconnect.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KafkaConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/literals/).
+
 ```python
-from types_aiobotocore_kafkaconnect.literals import (
-    ConnectorStateType,
-    CustomPluginContentTypeType,
-    CustomPluginStateType,
-    KafkaClusterClientAuthenticationTypeType,
-    KafkaClusterEncryptionInTransitTypeType,
-    ListConnectorsPaginatorName,
-    ListCustomPluginsPaginatorName,
-    ListWorkerConfigurationsPaginatorName,
-    KafkaConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kafkaconnect.literals import ConnectorStateType
 
 
 def check_value(value: ConnectorStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kafkaconnect.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KafkaConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/type_defs/).
+
 ```python
-from types_aiobotocore_kafkaconnect.type_defs import (
-    VpcDescriptionTypeDef,
-    VpcTypeDef,
-    ScaleInPolicyDescriptionTypeDef,
-    ScaleOutPolicyDescriptionTypeDef,
-    ScaleInPolicyTypeDef,
-    ScaleOutPolicyTypeDef,
-    ScaleInPolicyUpdateTypeDef,
-    ScaleOutPolicyUpdateTypeDef,
-    ProvisionedCapacityDescriptionTypeDef,
-    ProvisionedCapacityTypeDef,
-    ProvisionedCapacityUpdateTypeDef,
-    CloudWatchLogsLogDeliveryDescriptionTypeDef,
-    CloudWatchLogsLogDeliveryTypeDef,
-    KafkaClusterClientAuthenticationDescriptionTypeDef,
-    KafkaClusterEncryptionInTransitDescriptionTypeDef,
-    WorkerConfigurationDescriptionTypeDef,
-    KafkaClusterClientAuthenticationTypeDef,
-    KafkaClusterEncryptionInTransitTypeDef,
-    WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    CreateWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionSummaryTypeDef,
-    CustomPluginDescriptionTypeDef,
-    CustomPluginFileDescriptionTypeDef,
-    S3LocationDescriptionTypeDef,
-    S3LocationTypeDef,
-    CustomPluginTypeDef,
-    DeleteConnectorRequestRequestTypeDef,
-    DeleteCustomPluginRequestRequestTypeDef,
-    DescribeConnectorRequestRequestTypeDef,
-    StateDescriptionTypeDef,
-    DescribeCustomPluginRequestRequestTypeDef,
-    DescribeWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionDescriptionTypeDef,
-    FirehoseLogDeliveryDescriptionTypeDef,
-    FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
-    ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestRequestTypeDef,
-    S3LogDeliveryDescriptionTypeDef,
-    S3LogDeliveryTypeDef,
-    ApacheKafkaClusterDescriptionTypeDef,
-    ApacheKafkaClusterTypeDef,
-    AutoScalingDescriptionTypeDef,
-    AutoScalingTypeDef,
-    AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
-    CreateWorkerConfigurationResponseTypeDef,
-    WorkerConfigurationSummaryTypeDef,
-    PluginDescriptionTypeDef,
-    CustomPluginLocationDescriptionTypeDef,
-    CustomPluginLocationTypeDef,
-    PluginTypeDef,
-    DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
-    WorkerLogDeliveryDescriptionTypeDef,
-    WorkerLogDeliveryTypeDef,
-    KafkaClusterDescriptionTypeDef,
-    KafkaClusterTypeDef,
-    CapacityDescriptionTypeDef,
-    CapacityTypeDef,
-    CapacityUpdateTypeDef,
-    ListWorkerConfigurationsResponseTypeDef,
-    CustomPluginRevisionSummaryTypeDef,
-    CreateCustomPluginRequestRequestTypeDef,
-    LogDeliveryDescriptionTypeDef,
-    LogDeliveryTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
-    CustomPluginSummaryTypeDef,
-    DescribeCustomPluginResponseTypeDef,
-    ConnectorSummaryTypeDef,
-    DescribeConnectorResponseTypeDef,
-    CreateConnectorRequestRequestTypeDef,
-    ListCustomPluginsResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-)
+from types_aiobotocore_kafkaconnect.type_defs import VpcDescriptionTypeDef
 
 
 def get_value() -> VpcDescriptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/setup.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kafkaconnect",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kafkaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KafkaConnect 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__init__.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__init__.pyi` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/__main__.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KafkaConnect 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.KafkaConnect 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect\nOther"
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

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/client.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/client.pyi` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/literals.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
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
@@ -161,14 +162,15 @@
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
@@ -247,26 +249,28 @@
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

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/literals.pyi` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
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
@@ -159,14 +160,15 @@
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
@@ -245,26 +247,28 @@
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

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/paginator.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/paginator.pyi` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/type_defs.py` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect/type_defs.pyi` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kafkaconnect
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KafkaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KafkaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/
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
 [types-aiobotocore-kafkaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,128 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kafkaconnect.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KafkaConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/literals/).
+
 ```python
-from types_aiobotocore_kafkaconnect.literals import (
-    ConnectorStateType,
-    CustomPluginContentTypeType,
-    CustomPluginStateType,
-    KafkaClusterClientAuthenticationTypeType,
-    KafkaClusterEncryptionInTransitTypeType,
-    ListConnectorsPaginatorName,
-    ListCustomPluginsPaginatorName,
-    ListWorkerConfigurationsPaginatorName,
-    KafkaConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kafkaconnect.literals import ConnectorStateType
 
 
 def check_value(value: ConnectorStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kafkaconnect.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KafkaConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafkaconnect/type_defs/).
+
 ```python
-from types_aiobotocore_kafkaconnect.type_defs import (
-    VpcDescriptionTypeDef,
-    VpcTypeDef,
-    ScaleInPolicyDescriptionTypeDef,
-    ScaleOutPolicyDescriptionTypeDef,
-    ScaleInPolicyTypeDef,
-    ScaleOutPolicyTypeDef,
-    ScaleInPolicyUpdateTypeDef,
-    ScaleOutPolicyUpdateTypeDef,
-    ProvisionedCapacityDescriptionTypeDef,
-    ProvisionedCapacityTypeDef,
-    ProvisionedCapacityUpdateTypeDef,
-    CloudWatchLogsLogDeliveryDescriptionTypeDef,
-    CloudWatchLogsLogDeliveryTypeDef,
-    KafkaClusterClientAuthenticationDescriptionTypeDef,
-    KafkaClusterEncryptionInTransitDescriptionTypeDef,
-    WorkerConfigurationDescriptionTypeDef,
-    KafkaClusterClientAuthenticationTypeDef,
-    KafkaClusterEncryptionInTransitTypeDef,
-    WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    CreateWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionSummaryTypeDef,
-    CustomPluginDescriptionTypeDef,
-    CustomPluginFileDescriptionTypeDef,
-    S3LocationDescriptionTypeDef,
-    S3LocationTypeDef,
-    CustomPluginTypeDef,
-    DeleteConnectorRequestRequestTypeDef,
-    DeleteCustomPluginRequestRequestTypeDef,
-    DescribeConnectorRequestRequestTypeDef,
-    StateDescriptionTypeDef,
-    DescribeCustomPluginRequestRequestTypeDef,
-    DescribeWorkerConfigurationRequestRequestTypeDef,
-    WorkerConfigurationRevisionDescriptionTypeDef,
-    FirehoseLogDeliveryDescriptionTypeDef,
-    FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
-    ListConnectorsRequestRequestTypeDef,
-    ListCustomPluginsRequestRequestTypeDef,
-    ListWorkerConfigurationsRequestRequestTypeDef,
-    S3LogDeliveryDescriptionTypeDef,
-    S3LogDeliveryTypeDef,
-    ApacheKafkaClusterDescriptionTypeDef,
-    ApacheKafkaClusterTypeDef,
-    AutoScalingDescriptionTypeDef,
-    AutoScalingTypeDef,
-    AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
-    CreateWorkerConfigurationResponseTypeDef,
-    WorkerConfigurationSummaryTypeDef,
-    PluginDescriptionTypeDef,
-    CustomPluginLocationDescriptionTypeDef,
-    CustomPluginLocationTypeDef,
-    PluginTypeDef,
-    DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
-    WorkerLogDeliveryDescriptionTypeDef,
-    WorkerLogDeliveryTypeDef,
-    KafkaClusterDescriptionTypeDef,
-    KafkaClusterTypeDef,
-    CapacityDescriptionTypeDef,
-    CapacityTypeDef,
-    CapacityUpdateTypeDef,
-    ListWorkerConfigurationsResponseTypeDef,
-    CustomPluginRevisionSummaryTypeDef,
-    CreateCustomPluginRequestRequestTypeDef,
-    LogDeliveryDescriptionTypeDef,
-    LogDeliveryTypeDef,
-    UpdateConnectorRequestRequestTypeDef,
-    CustomPluginSummaryTypeDef,
-    DescribeCustomPluginResponseTypeDef,
-    ConnectorSummaryTypeDef,
-    DescribeConnectorResponseTypeDef,
-    CreateConnectorRequestRequestTypeDef,
-    ListCustomPluginsResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-)
+from types_aiobotocore_kafkaconnect.type_defs import VpcDescriptionTypeDef
 
 
 def get_value() -> VpcDescriptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kafkaconnect-2.5.2.post1/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt` & `types-aiobotocore-kafkaconnect-2.5.2.post2/types_aiobotocore_kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

