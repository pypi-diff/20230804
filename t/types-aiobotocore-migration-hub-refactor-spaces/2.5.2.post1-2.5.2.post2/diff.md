# Comparing `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1.tar` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.981520 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-08-02 14:52:40.981520 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.981520 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.949520 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24615 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29136 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29105 2023-08-02 14:43:41.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.981520 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 14:52:40.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.566643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14769 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13166 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.566643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2226 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1612 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1611 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1025 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24605 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24567 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10271 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10269 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7278 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7271 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28376 2023-08-04 13:45:05.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28347 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14769 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1231 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       48 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/LICENSE` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/PKG-INFO` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migration-hub-refactor-spaces
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
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
 [types-aiobotocore-migration-hub-refactor-spaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,126 +309,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_migration_hub_refactor_spaces.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `MigrationHubRefactorSpaces` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/literals/).
+
 ```python
-from types_aiobotocore_migration_hub_refactor_spaces.literals import (
-    ApiGatewayEndpointTypeType,
-    ApplicationStateType,
-    EnvironmentStateType,
-    ErrorCodeType,
-    ErrorResourceTypeType,
-    HttpMethodType,
-    ListApplicationsPaginatorName,
-    ListEnvironmentVpcsPaginatorName,
-    ListEnvironmentsPaginatorName,
-    ListRoutesPaginatorName,
-    ListServicesPaginatorName,
-    NetworkFabricTypeType,
-    ProxyTypeType,
-    RouteActivationStateType,
-    RouteStateType,
-    RouteTypeType,
-    ServiceEndpointTypeType,
-    ServiceStateType,
-    MigrationHubRefactorSpacesServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_migration_hub_refactor_spaces.literals import ApiGatewayEndpointTypeType
 
 
 def check_value(value: ApiGatewayEndpointTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_migration_hub_refactor_spaces.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `MigrationHubRefactorSpaces` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/type_defs/).
+
 ```python
-from types_aiobotocore_migration_hub_refactor_spaces.type_defs import (
-    ApiGatewayProxyConfigTypeDef,
-    ApiGatewayProxyInputTypeDef,
-    ApiGatewayProxySummaryTypeDef,
-    ErrorResponseTypeDef,
-    ResponseMetadataTypeDef,
-    CreateEnvironmentRequestRequestTypeDef,
-    DefaultRouteInputTypeDef,
-    UriPathRouteInputTypeDef,
-    UriPathRouteInputOutputTypeDef,
-    LambdaEndpointInputTypeDef,
-    UrlEndpointInputTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteRouteRequestRequestTypeDef,
-    DeleteServiceRequestRequestTypeDef,
-    EnvironmentVpcTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetEnvironmentRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    GetRouteRequestRequestTypeDef,
-    GetServiceRequestRequestTypeDef,
-    LambdaEndpointConfigTypeDef,
-    UrlEndpointConfigTypeDef,
-    LambdaEndpointSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListEnvironmentVpcsRequestRequestTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListRoutesRequestRequestTypeDef,
-    ListServicesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    UrlEndpointSummaryTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ApplicationSummaryTypeDef,
-    EnvironmentSummaryTypeDef,
-    RouteSummaryTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DeleteEnvironmentResponseTypeDef,
-    DeleteRouteResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    GetApplicationResponseTypeDef,
-    GetEnvironmentResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetRouteResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRouteResponseTypeDef,
-    CreateRouteRequestRequestTypeDef,
-    CreateRouteResponseTypeDef,
-    UriPathRouteInputUnionTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    CreateServiceResponseTypeDef,
-    ListEnvironmentVpcsResponseTypeDef,
-    GetServiceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ServiceSummaryTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListEnvironmentsResponseTypeDef,
-    ListRoutesResponseTypeDef,
-    ListServicesResponseTypeDef,
-)
+from types_aiobotocore_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
 
 def get_value() -> ApiGatewayProxyConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/README.md` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-migration-hub-refactor-spaces
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore migration-hub-refactor-spaces type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-migration-hub-refactor-spaces"></a>
 
 # types-aiobotocore-migration-hub-refactor-spaces
 
 [![PyPI - types-aiobotocore-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
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
 [types-aiobotocore-migration-hub-refactor-spaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,126 +309,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_migration_hub_refactor_spaces.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `MigrationHubRefactorSpaces` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/literals/).
+
 ```python
-from types_aiobotocore_migration_hub_refactor_spaces.literals import (
-    ApiGatewayEndpointTypeType,
-    ApplicationStateType,
-    EnvironmentStateType,
-    ErrorCodeType,
-    ErrorResourceTypeType,
-    HttpMethodType,
-    ListApplicationsPaginatorName,
-    ListEnvironmentVpcsPaginatorName,
-    ListEnvironmentsPaginatorName,
-    ListRoutesPaginatorName,
-    ListServicesPaginatorName,
-    NetworkFabricTypeType,
-    ProxyTypeType,
-    RouteActivationStateType,
-    RouteStateType,
-    RouteTypeType,
-    ServiceEndpointTypeType,
-    ServiceStateType,
-    MigrationHubRefactorSpacesServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_migration_hub_refactor_spaces.literals import ApiGatewayEndpointTypeType
 
 
 def check_value(value: ApiGatewayEndpointTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_migration_hub_refactor_spaces.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `MigrationHubRefactorSpaces` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/type_defs/).
+
 ```python
-from types_aiobotocore_migration_hub_refactor_spaces.type_defs import (
-    ApiGatewayProxyConfigTypeDef,
-    ApiGatewayProxyInputTypeDef,
-    ApiGatewayProxySummaryTypeDef,
-    ErrorResponseTypeDef,
-    ResponseMetadataTypeDef,
-    CreateEnvironmentRequestRequestTypeDef,
-    DefaultRouteInputTypeDef,
-    UriPathRouteInputTypeDef,
-    UriPathRouteInputOutputTypeDef,
-    LambdaEndpointInputTypeDef,
-    UrlEndpointInputTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteRouteRequestRequestTypeDef,
-    DeleteServiceRequestRequestTypeDef,
-    EnvironmentVpcTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetEnvironmentRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    GetRouteRequestRequestTypeDef,
-    GetServiceRequestRequestTypeDef,
-    LambdaEndpointConfigTypeDef,
-    UrlEndpointConfigTypeDef,
-    LambdaEndpointSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListEnvironmentVpcsRequestRequestTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListRoutesRequestRequestTypeDef,
-    ListServicesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    UrlEndpointSummaryTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ApplicationSummaryTypeDef,
-    EnvironmentSummaryTypeDef,
-    RouteSummaryTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    DeleteApplicationResponseTypeDef,
-    DeleteEnvironmentResponseTypeDef,
-    DeleteRouteResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    GetApplicationResponseTypeDef,
-    GetEnvironmentResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetRouteResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRouteResponseTypeDef,
-    CreateRouteRequestRequestTypeDef,
-    CreateRouteResponseTypeDef,
-    UriPathRouteInputUnionTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    CreateServiceResponseTypeDef,
-    ListEnvironmentVpcsResponseTypeDef,
-    GetServiceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ServiceSummaryTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListEnvironmentsResponseTypeDef,
-    ListRoutesResponseTypeDef,
-    ListServicesResponseTypeDef,
-)
+from types_aiobotocore_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
 
 def get_value() -> ApiGatewayProxyConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/setup.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migration-hub-refactor-spaces",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__init__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/__main__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/client.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,47 +53,43 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
-    UriPathRouteInputUnionTypeDef,
+    UriPathRouteInputTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MigrationHubRefactorSpacesClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class MigrationHubRefactorSpacesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
     """
 
     meta: ClientMeta
@@ -102,31 +98,28 @@
     def exceptions(self) -> Exceptions:
         """
         MigrationHubRefactorSpacesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#close)
         """
-
     async def create_application(
         self,
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
@@ -136,15 +129,14 @@
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_application)
         """
-
     async def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
@@ -152,34 +144,32 @@
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_environment)
         """
-
     async def create_route(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputUnionTypeDef = ...
+        UriPathRoute: UriPathRouteInputTypeDef = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_route)
         """
-
     async def create_service(
         self,
         *,
         ApplicationIdentifier: str,
         EndpointType: ServiceEndpointTypeType,
         EnvironmentIdentifier: str,
         Name: str,
@@ -192,156 +182,141 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_service)
         """
-
     async def delete_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> DeleteApplicationResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_application)
         """
-
     async def delete_environment(
         self, *, EnvironmentIdentifier: str
     ) -> DeleteEnvironmentResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_environment)
         """
-
     async def delete_resource_policy(self, *, Identifier: str) -> Dict[str, Any]:
         """
         Deletes the resource policy set for the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_resource_policy)
         """
-
     async def delete_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> DeleteRouteResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_route)
         """
-
     async def delete_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#generate_presigned_url)
         """
-
     async def get_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> GetApplicationResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_application)
         """
-
     async def get_environment(self, *, EnvironmentIdentifier: str) -> GetEnvironmentResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_environment)
         """
-
     async def get_resource_policy(self, *, Identifier: str) -> GetResourcePolicyResponseTypeDef:
         """
         Gets the resource-based permission policy that is set for the given environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_resource_policy)
         """
-
     async def get_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> GetRouteResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_route)
         """
-
     async def get_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> GetServiceResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_service)
         """
-
     async def list_applications(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces applications
         within an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_applications)
         """
-
     async def list_environment_vpcs(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentVpcsResponseTypeDef:
         """
         Lists all Amazon Web Services Migration Hub Refactor Spaces service virtual
         private clouds (VPCs) that are part of the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environment_vpcs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_environment_vpcs)
         """
-
     async def list_environments(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists Amazon Web Services Migration Hub Refactor Spaces environments owned by a
         caller account or shared with the caller account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_environments)
         """
-
     async def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -349,15 +324,14 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_routes)
         """
-
     async def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -365,110 +339,98 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_services)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_tags_for_resource)
         """
-
     async def put_resource_policy(self, *, Policy: str, ResourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to the Amazon Web Services Migration
         Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#put_resource_policy)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Removes the tags of a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#untag_resource)
         """
-
     async def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteIdentifier: str
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#update_route)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_vpcs"]
     ) -> ListEnvironmentVpcsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "MigrationHubRefactorSpacesClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/client.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,43 +53,47 @@
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateRouteResponseTypeDef,
-    UriPathRouteInputUnionTypeDef,
+    UriPathRouteInputTypeDef,
     UrlEndpointInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("MigrationHubRefactorSpacesClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidResourcePolicyException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class MigrationHubRefactorSpacesClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
     """
 
     meta: ClientMeta
@@ -98,28 +102,31 @@
     def exceptions(self) -> Exceptions:
         """
         MigrationHubRefactorSpacesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#close)
         """
+
     async def create_application(
         self,
         *,
         EnvironmentIdentifier: str,
         Name: str,
         ProxyType: Literal["API_GATEWAY"],
         VpcId: str,
@@ -129,14 +136,15 @@
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_application)
         """
+
     async def create_environment(
         self,
         *,
         Name: str,
         NetworkFabricType: NetworkFabricTypeType,
         ClientToken: str = ...,
         Description: str = ...,
@@ -144,32 +152,34 @@
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_environment)
         """
+
     async def create_route(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteType: RouteTypeType,
         ServiceIdentifier: str,
         ClientToken: str = ...,
         DefaultRoute: DefaultRouteInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        UriPathRoute: UriPathRouteInputUnionTypeDef = ...
+        UriPathRoute: UriPathRouteInputTypeDef = ...
     ) -> CreateRouteResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_route)
         """
+
     async def create_service(
         self,
         *,
         ApplicationIdentifier: str,
         EndpointType: ServiceEndpointTypeType,
         EnvironmentIdentifier: str,
         Name: str,
@@ -182,141 +192,156 @@
     ) -> CreateServiceResponseTypeDef:
         """
         Creates an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#create_service)
         """
+
     async def delete_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> DeleteApplicationResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_application)
         """
+
     async def delete_environment(
         self, *, EnvironmentIdentifier: str
     ) -> DeleteEnvironmentResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_environment)
         """
+
     async def delete_resource_policy(self, *, Identifier: str) -> Dict[str, Any]:
         """
         Deletes the resource policy set for the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_resource_policy)
         """
+
     async def delete_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> DeleteRouteResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_route)
         """
+
     async def delete_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.delete_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#delete_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#generate_presigned_url)
         """
+
     async def get_application(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str
     ) -> GetApplicationResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_application)
         """
+
     async def get_environment(self, *, EnvironmentIdentifier: str) -> GetEnvironmentResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_environment)
         """
+
     async def get_resource_policy(self, *, Identifier: str) -> GetResourcePolicyResponseTypeDef:
         """
         Gets the resource-based permission policy that is set for the given environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_resource_policy)
         """
+
     async def get_route(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, RouteIdentifier: str
     ) -> GetRouteResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_route)
         """
+
     async def get_service(
         self, *, ApplicationIdentifier: str, EnvironmentIdentifier: str, ServiceIdentifier: str
     ) -> GetServiceResponseTypeDef:
         """
         Gets an Amazon Web Services Migration Hub Refactor Spaces service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_service)
         """
+
     async def list_applications(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces applications
         within an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_applications)
         """
+
     async def list_environment_vpcs(
         self, *, EnvironmentIdentifier: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentVpcsResponseTypeDef:
         """
         Lists all Amazon Web Services Migration Hub Refactor Spaces service virtual
         private clouds (VPCs) that are part of the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environment_vpcs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_environment_vpcs)
         """
+
     async def list_environments(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEnvironmentsResponseTypeDef:
         """
         Lists Amazon Web Services Migration Hub Refactor Spaces environments owned by a
         caller account or shared with the caller account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_environments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_environments)
         """
+
     async def list_routes(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -324,14 +349,15 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces routes within an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_routes)
         """
+
     async def list_services(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -339,98 +365,110 @@
         """
         Lists all the Amazon Web Services Migration Hub Refactor Spaces services within
         an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_services)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#list_tags_for_resource)
         """
+
     async def put_resource_policy(self, *, Policy: str, ResourceArn: str) -> Dict[str, Any]:
         """
         Attaches a resource-based permission policy to the Amazon Web Services Migration
         Hub Refactor Spaces environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#put_resource_policy)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Removes the tags of a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#untag_resource)
         """
+
     async def update_route(
         self,
         *,
         ActivationState: RouteActivationStateType,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
         RouteIdentifier: str
     ) -> UpdateRouteResponseTypeDef:
         """
         Updates an Amazon Web Services Migration Hub Refactor Spaces route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#update_route)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environment_vpcs"]
     ) -> ListEnvironmentVpcsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_environments"]
     ) -> ListEnvironmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "MigrationHubRefactorSpacesClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/client/)
         """
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/literals.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApiGatewayEndpointTypeType",
     "ApplicationStateType",
     "EnvironmentStateType",
     "ErrorCodeType",
     "ErrorResourceTypeType",
     "HttpMethodType",
@@ -40,15 +39,14 @@
     "ServiceStateType",
     "MigrationHubRefactorSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ApiGatewayEndpointTypeType = Literal["PRIVATE", "REGIONAL"]
 ApplicationStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 EnvironmentStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 ErrorCodeType = Literal[
     "INVALID_RESOURCE_STATE",
     "NOT_AUTHORIZED",
     "REQUEST_LIMIT_EXCEEDED",
@@ -108,14 +106,15 @@
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
@@ -211,14 +210,15 @@
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
@@ -297,26 +297,28 @@
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApiGatewayEndpointTypeType",
     "ApplicationStateType",
     "EnvironmentStateType",
     "ErrorCodeType",
     "ErrorResourceTypeType",
     "HttpMethodType",
@@ -39,14 +40,15 @@
     "ServiceStateType",
     "MigrationHubRefactorSpacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ApiGatewayEndpointTypeType = Literal["PRIVATE", "REGIONAL"]
 ApplicationStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 EnvironmentStateType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 ErrorCodeType = Literal[
     "INVALID_RESOURCE_STATE",
     "NOT_AUTHORIZED",
     "REQUEST_LIMIT_EXCEEDED",
@@ -106,14 +108,15 @@
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
@@ -209,14 +212,15 @@
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
@@ -295,26 +299,28 @@
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/paginator.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
     data: ApiGatewayProxyConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
@@ -45,15 +45,14 @@
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
-    "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
@@ -92,15 +91,14 @@
     "GetEnvironmentResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
-    "UriPathRouteInputUnionTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
@@ -226,38 +224,14 @@
 
 class UriPathRouteInputTypeDef(
     _RequiredUriPathRouteInputTypeDef, _OptionalUriPathRouteInputTypeDef
 ):
     pass
 
 
-_RequiredUriPathRouteInputOutputTypeDef = TypedDict(
-    "_RequiredUriPathRouteInputOutputTypeDef",
-    {
-        "ActivationState": RouteActivationStateType,
-        "SourcePath": str,
-    },
-)
-_OptionalUriPathRouteInputOutputTypeDef = TypedDict(
-    "_OptionalUriPathRouteInputOutputTypeDef",
-    {
-        "AppendSourcePath": bool,
-        "IncludeChildPaths": bool,
-        "Methods": List[HttpMethodType],
-    },
-    total=False,
-)
-
-
-class UriPathRouteInputOutputTypeDef(
-    _RequiredUriPathRouteInputOutputTypeDef, _OptionalUriPathRouteInputOutputTypeDef
-):
-    pass
-
-
 LambdaEndpointInputTypeDef = TypedDict(
     "LambdaEndpointInputTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -870,20 +844,19 @@
         "LastUpdatedTime": datetime,
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "UriPathRoute": UriPathRouteInputOutputTypeDef,
+        "UriPathRoute": UriPathRouteInputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UriPathRouteInputUnionTypeDef = Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef]
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentIdentifier": str,
         "Name": str,
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_migration_hub_refactor_spaces.type_defs import ApiGatewayProxyConfigTypeDef
 
     data: ApiGatewayProxyConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApiGatewayEndpointTypeType,
     ApplicationStateType,
     EnvironmentStateType,
     ErrorCodeType,
     ErrorResourceTypeType,
@@ -44,15 +44,14 @@
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
     "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
-    "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
@@ -91,15 +90,14 @@
     "GetEnvironmentResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
-    "UriPathRouteInputUnionTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
@@ -221,36 +219,14 @@
 )
 
 class UriPathRouteInputTypeDef(
     _RequiredUriPathRouteInputTypeDef, _OptionalUriPathRouteInputTypeDef
 ):
     pass
 
-_RequiredUriPathRouteInputOutputTypeDef = TypedDict(
-    "_RequiredUriPathRouteInputOutputTypeDef",
-    {
-        "ActivationState": RouteActivationStateType,
-        "SourcePath": str,
-    },
-)
-_OptionalUriPathRouteInputOutputTypeDef = TypedDict(
-    "_OptionalUriPathRouteInputOutputTypeDef",
-    {
-        "AppendSourcePath": bool,
-        "IncludeChildPaths": bool,
-        "Methods": List[HttpMethodType],
-    },
-    total=False,
-)
-
-class UriPathRouteInputOutputTypeDef(
-    _RequiredUriPathRouteInputOutputTypeDef, _OptionalUriPathRouteInputOutputTypeDef
-):
-    pass
-
 LambdaEndpointInputTypeDef = TypedDict(
     "LambdaEndpointInputTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -849,20 +825,19 @@
         "LastUpdatedTime": datetime,
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "UriPathRoute": UriPathRouteInputOutputTypeDef,
+        "UriPathRoute": UriPathRouteInputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UriPathRouteInputUnionTypeDef = Union[UriPathRouteInputTypeDef, UriPathRouteInputOutputTypeDef]
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentIdentifier": str,
         "Name": str,
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post1/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

