# Comparing `tmp/types-aiobotocore-appconfig-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appconfig-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfig-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfig-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-appconfig-2.5.2.post1.tar` & `types-aiobotocore-appconfig-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-08-02 14:33:07.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-02 14:33:07.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:06.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.449660 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:51:50.000000 types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.763005 types-aiobotocore-appconfig-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-04 12:00:22.763005 types-aiobotocore-appconfig-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.763005 types-aiobotocore-appconfig-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.759005 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-08-04 11:40:15.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-04 11:40:14.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:13.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.763005 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:00:22.000000 types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/LICENSE` & `types-aiobotocore-appconfig-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/PKG-INFO` & `types-aiobotocore-appconfig-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,124 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appconfig.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `AppConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/literals/).
+
 ```python
-from types_aiobotocore_appconfig.literals import (
-    ActionPointType,
-    DeploymentEventTypeType,
-    DeploymentStateType,
-    EnvironmentStateType,
-    GrowthTypeType,
-    ReplicateToType,
-    TriggeredByType,
-    ValidatorTypeType,
-    AppConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appconfig.literals import ActionPointType
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/type_defs/).
+
 ```python
-from types_aiobotocore_appconfig.type_defs import (
-    ActionInvocationTypeDef,
-    ActionTypeDef,
-    ResponseMetadataTypeDef,
-    ApplicationTypeDef,
-    AppliedExtensionTypeDef,
-    BlobTypeDef,
-    ConfigurationProfileSummaryTypeDef,
-    ValidatorTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    CreateDeploymentStrategyRequestRequestTypeDef,
-    MonitorTypeDef,
-    CreateExtensionAssociationRequestRequestTypeDef,
-    ParameterTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteConfigurationProfileRequestRequestTypeDef,
-    DeleteDeploymentStrategyRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    DeleteExtensionAssociationRequestRequestTypeDef,
-    DeleteExtensionRequestRequestTypeDef,
-    DeleteHostedConfigurationVersionRequestRequestTypeDef,
-    DeploymentStrategyTypeDef,
-    DeploymentSummaryTypeDef,
-    ExtensionAssociationSummaryTypeDef,
-    ExtensionSummaryTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetConfigurationProfileRequestRequestTypeDef,
-    GetConfigurationRequestRequestTypeDef,
-    GetDeploymentRequestRequestTypeDef,
-    GetDeploymentStrategyRequestRequestTypeDef,
-    GetEnvironmentRequestRequestTypeDef,
-    GetExtensionAssociationRequestRequestTypeDef,
-    GetExtensionRequestRequestTypeDef,
-    GetHostedConfigurationVersionRequestRequestTypeDef,
-    HostedConfigurationVersionSummaryTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListConfigurationProfilesRequestRequestTypeDef,
-    ListDeploymentStrategiesRequestRequestTypeDef,
-    ListDeploymentsRequestRequestTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListExtensionAssociationsRequestRequestTypeDef,
-    ListExtensionsRequestRequestTypeDef,
-    ListHostedConfigurationVersionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartDeploymentRequestRequestTypeDef,
-    StopDeploymentRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    UpdateDeploymentStrategyRequestRequestTypeDef,
-    UpdateExtensionAssociationRequestRequestTypeDef,
-    ValidateConfigurationRequestRequestTypeDef,
-    DeploymentEventTypeDef,
-    ApplicationResponseTypeDef,
-    ConfigurationTypeDef,
-    DeploymentStrategyResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExtensionAssociationTypeDef,
-    HostedConfigurationVersionTypeDef,
-    ResourceTagsTypeDef,
-    ApplicationsTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
-    ConfigurationProfilesTypeDef,
-    ConfigurationProfileTypeDef,
-    CreateConfigurationProfileRequestRequestTypeDef,
-    UpdateConfigurationProfileRequestRequestTypeDef,
-    CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseTypeDef,
-    EnvironmentTypeDef,
-    UpdateEnvironmentRequestRequestTypeDef,
-    CreateExtensionRequestRequestTypeDef,
-    ExtensionTypeDef,
-    UpdateExtensionRequestRequestTypeDef,
-    DeploymentStrategiesTypeDef,
-    DeploymentsTypeDef,
-    ExtensionAssociationsTypeDef,
-    ExtensionsTypeDef,
-    HostedConfigurationVersionsTypeDef,
-    DeploymentTypeDef,
-    EnvironmentsTypeDef,
-)
+from types_aiobotocore_appconfig.type_defs import ActionInvocationTypeDef
 
 
 def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/README.md` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-appconfig
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore appconfig type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appconfig"></a>
 
 # types-aiobotocore-appconfig
 
 [![PyPI - types-aiobotocore-appconfig](https://img.shields.io/pypi/v/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
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
 [types-aiobotocore-appconfig docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,124 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appconfig.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `AppConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/literals/).
+
 ```python
-from types_aiobotocore_appconfig.literals import (
-    ActionPointType,
-    DeploymentEventTypeType,
-    DeploymentStateType,
-    EnvironmentStateType,
-    GrowthTypeType,
-    ReplicateToType,
-    TriggeredByType,
-    ValidatorTypeType,
-    AppConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appconfig.literals import ActionPointType
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/type_defs/).
+
 ```python
-from types_aiobotocore_appconfig.type_defs import (
-    ActionInvocationTypeDef,
-    ActionTypeDef,
-    ResponseMetadataTypeDef,
-    ApplicationTypeDef,
-    AppliedExtensionTypeDef,
-    BlobTypeDef,
-    ConfigurationProfileSummaryTypeDef,
-    ValidatorTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    CreateDeploymentStrategyRequestRequestTypeDef,
-    MonitorTypeDef,
-    CreateExtensionAssociationRequestRequestTypeDef,
-    ParameterTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteConfigurationProfileRequestRequestTypeDef,
-    DeleteDeploymentStrategyRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    DeleteExtensionAssociationRequestRequestTypeDef,
-    DeleteExtensionRequestRequestTypeDef,
-    DeleteHostedConfigurationVersionRequestRequestTypeDef,
-    DeploymentStrategyTypeDef,
-    DeploymentSummaryTypeDef,
-    ExtensionAssociationSummaryTypeDef,
-    ExtensionSummaryTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetConfigurationProfileRequestRequestTypeDef,
-    GetConfigurationRequestRequestTypeDef,
-    GetDeploymentRequestRequestTypeDef,
-    GetDeploymentStrategyRequestRequestTypeDef,
-    GetEnvironmentRequestRequestTypeDef,
-    GetExtensionAssociationRequestRequestTypeDef,
-    GetExtensionRequestRequestTypeDef,
-    GetHostedConfigurationVersionRequestRequestTypeDef,
-    HostedConfigurationVersionSummaryTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListConfigurationProfilesRequestRequestTypeDef,
-    ListDeploymentStrategiesRequestRequestTypeDef,
-    ListDeploymentsRequestRequestTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListExtensionAssociationsRequestRequestTypeDef,
-    ListExtensionsRequestRequestTypeDef,
-    ListHostedConfigurationVersionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartDeploymentRequestRequestTypeDef,
-    StopDeploymentRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    UpdateDeploymentStrategyRequestRequestTypeDef,
-    UpdateExtensionAssociationRequestRequestTypeDef,
-    ValidateConfigurationRequestRequestTypeDef,
-    DeploymentEventTypeDef,
-    ApplicationResponseTypeDef,
-    ConfigurationTypeDef,
-    DeploymentStrategyResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExtensionAssociationTypeDef,
-    HostedConfigurationVersionTypeDef,
-    ResourceTagsTypeDef,
-    ApplicationsTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
-    ConfigurationProfilesTypeDef,
-    ConfigurationProfileTypeDef,
-    CreateConfigurationProfileRequestRequestTypeDef,
-    UpdateConfigurationProfileRequestRequestTypeDef,
-    CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseTypeDef,
-    EnvironmentTypeDef,
-    UpdateEnvironmentRequestRequestTypeDef,
-    CreateExtensionRequestRequestTypeDef,
-    ExtensionTypeDef,
-    UpdateExtensionRequestRequestTypeDef,
-    DeploymentStrategiesTypeDef,
-    DeploymentsTypeDef,
-    ExtensionAssociationsTypeDef,
-    ExtensionsTypeDef,
-    HostedConfigurationVersionsTypeDef,
-    DeploymentTypeDef,
-    EnvironmentsTypeDef,
-)
+from types_aiobotocore_appconfig.type_defs import ActionInvocationTypeDef
 
 
 def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/setup.py` & `types-aiobotocore-appconfig-2.5.2.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfig",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/__main__.py` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfig 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AppConfig 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.py` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/client.pyi` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.py` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/literals.pyi` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.py` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig/type_defs.pyi` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post1/types_aiobotocore_appconfig.egg-info/SOURCES.txt` & `types-aiobotocore-appconfig-2.5.2.post2/types_aiobotocore_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

