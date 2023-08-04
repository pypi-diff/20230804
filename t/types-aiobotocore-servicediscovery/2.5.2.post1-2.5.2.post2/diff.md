# Comparing `tmp/types-aiobotocore-servicediscovery-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-servicediscovery-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-servicediscovery-2.5.2.post1.tar` & `types-aiobotocore-servicediscovery-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.733458 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-08-02 14:49:40.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28990 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13791 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12237 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1295 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1294 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24549 2023-08-04 13:53:25.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24510 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10287 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10285 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5740 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5734 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28436 2023-08-04 13:53:29.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28400 2023-08-04 13:53:29.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13791 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/LICENSE` & `types-aiobotocore-servicediscovery-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,150 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicediscovery.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ServiceDiscovery` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/literals/).
+
 ```python
-from types_aiobotocore_servicediscovery.literals import (
-    CustomHealthStatusType,
-    FilterConditionType,
-    HealthCheckTypeType,
-    HealthStatusFilterType,
-    HealthStatusType,
-    ListInstancesPaginatorName,
-    ListNamespacesPaginatorName,
-    ListOperationsPaginatorName,
-    ListServicesPaginatorName,
-    NamespaceFilterNameType,
-    NamespaceTypeType,
-    OperationFilterNameType,
-    OperationStatusType,
-    OperationTargetTypeType,
-    OperationTypeType,
-    RecordTypeType,
-    RoutingPolicyType,
-    ServiceFilterNameType,
-    ServiceTypeOptionType,
-    ServiceTypeType,
-    ServiceDiscoveryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicediscovery.literals import CustomHealthStatusType
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceDiscovery` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/type_defs/).
+
 ```python
-from types_aiobotocore_servicediscovery.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    HealthCheckConfigTypeDef,
-    HealthCheckCustomConfigTypeDef,
-    DeleteNamespaceRequestRequestTypeDef,
-    DeleteServiceRequestRequestTypeDef,
-    DeregisterInstanceRequestRequestTypeDef,
-    DiscoverInstancesRequestRequestTypeDef,
-    HttpInstanceSummaryTypeDef,
-    DnsRecordTypeDef,
-    SOATypeDef,
-    GetInstanceRequestRequestTypeDef,
-    InstanceTypeDef,
-    GetInstancesHealthStatusRequestRequestTypeDef,
-    GetNamespaceRequestRequestTypeDef,
-    GetOperationRequestRequestTypeDef,
-    OperationTypeDef,
-    GetServiceRequestRequestTypeDef,
-    HttpNamespaceChangeTypeDef,
-    HttpPropertiesTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    NamespaceFilterTypeDef,
-    OperationFilterTypeDef,
-    OperationSummaryTypeDef,
-    ServiceFilterTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SOAChangeTypeDef,
-    RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterInstanceResponseTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceResponseTypeDef,
-    UpdatePublicDnsNamespaceResponseTypeDef,
-    UpdateServiceResponseTypeDef,
-    DiscoverInstancesResponseTypeDef,
-    DnsConfigChangeTypeDef,
-    DnsConfigOutputTypeDef,
-    DnsConfigTypeDef,
-    DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
-    GetInstanceResponseTypeDef,
-    GetOperationResponseTypeDef,
-    UpdateHttpNamespaceRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListNamespacesRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
-    ListOperationsResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesRequestRequestTypeDef,
-    PrivateDnsPropertiesMutableChangeTypeDef,
-    PublicDnsPropertiesMutableChangeTypeDef,
-    ServiceChangeTypeDef,
-    ServiceSummaryTypeDef,
-    ServiceTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    DnsConfigUnionTypeDef,
-    NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
-    CreateServiceResponseTypeDef,
-    GetServiceResponseTypeDef,
-    NamespaceSummaryTypeDef,
-    NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
-    ListNamespacesResponseTypeDef,
-    GetNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceRequestRequestTypeDef,
-    UpdatePublicDnsNamespaceRequestRequestTypeDef,
-)
+from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/README.md` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-servicediscovery
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,150 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicediscovery.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ServiceDiscovery` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/literals/).
+
 ```python
-from types_aiobotocore_servicediscovery.literals import (
-    CustomHealthStatusType,
-    FilterConditionType,
-    HealthCheckTypeType,
-    HealthStatusFilterType,
-    HealthStatusType,
-    ListInstancesPaginatorName,
-    ListNamespacesPaginatorName,
-    ListOperationsPaginatorName,
-    ListServicesPaginatorName,
-    NamespaceFilterNameType,
-    NamespaceTypeType,
-    OperationFilterNameType,
-    OperationStatusType,
-    OperationTargetTypeType,
-    OperationTypeType,
-    RecordTypeType,
-    RoutingPolicyType,
-    ServiceFilterNameType,
-    ServiceTypeOptionType,
-    ServiceTypeType,
-    ServiceDiscoveryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicediscovery.literals import CustomHealthStatusType
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceDiscovery` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/type_defs/).
+
 ```python
-from types_aiobotocore_servicediscovery.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    HealthCheckConfigTypeDef,
-    HealthCheckCustomConfigTypeDef,
-    DeleteNamespaceRequestRequestTypeDef,
-    DeleteServiceRequestRequestTypeDef,
-    DeregisterInstanceRequestRequestTypeDef,
-    DiscoverInstancesRequestRequestTypeDef,
-    HttpInstanceSummaryTypeDef,
-    DnsRecordTypeDef,
-    SOATypeDef,
-    GetInstanceRequestRequestTypeDef,
-    InstanceTypeDef,
-    GetInstancesHealthStatusRequestRequestTypeDef,
-    GetNamespaceRequestRequestTypeDef,
-    GetOperationRequestRequestTypeDef,
-    OperationTypeDef,
-    GetServiceRequestRequestTypeDef,
-    HttpNamespaceChangeTypeDef,
-    HttpPropertiesTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    NamespaceFilterTypeDef,
-    OperationFilterTypeDef,
-    OperationSummaryTypeDef,
-    ServiceFilterTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SOAChangeTypeDef,
-    RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterInstanceResponseTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceResponseTypeDef,
-    UpdatePublicDnsNamespaceResponseTypeDef,
-    UpdateServiceResponseTypeDef,
-    DiscoverInstancesResponseTypeDef,
-    DnsConfigChangeTypeDef,
-    DnsConfigOutputTypeDef,
-    DnsConfigTypeDef,
-    DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
-    GetInstanceResponseTypeDef,
-    GetOperationResponseTypeDef,
-    UpdateHttpNamespaceRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListNamespacesRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
-    ListOperationsResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesRequestRequestTypeDef,
-    PrivateDnsPropertiesMutableChangeTypeDef,
-    PublicDnsPropertiesMutableChangeTypeDef,
-    ServiceChangeTypeDef,
-    ServiceSummaryTypeDef,
-    ServiceTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    DnsConfigUnionTypeDef,
-    NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
-    CreateServiceResponseTypeDef,
-    GetServiceResponseTypeDef,
-    NamespaceSummaryTypeDef,
-    NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
-    ListNamespacesResponseTypeDef,
-    GetNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceRequestRequestTypeDef,
-    UpdatePublicDnsNamespaceRequestRequestTypeDef,
-)
+from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/setup.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicediscovery",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__main__.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ServiceDiscovery 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigUnionTypeDef,
+    DnsConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -186,15 +186,15 @@
     async def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: DnsConfigUnionTypeDef = ...,
+        DnsConfig: DnsConfigTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigUnionTypeDef,
+    DnsConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -176,15 +176,15 @@
     async def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: DnsConfigUnionTypeDef = ...,
+        DnsConfig: DnsConfigTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.pyi`

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
     "CustomHealthStatusType",
     "FilterConditionType",
     "HealthCheckTypeType",
     "HealthStatusFilterType",
     "HealthStatusType",
     "ListInstancesPaginatorName",
@@ -43,15 +42,14 @@
     "ServiceDiscoveryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CustomHealthStatusType = Literal["HEALTHY", "UNHEALTHY"]
 FilterConditionType = Literal["BEGINS_WITH", "BETWEEN", "EQ", "IN"]
 HealthCheckTypeType = Literal["HTTP", "HTTPS", "TCP"]
 HealthStatusFilterType = Literal["ALL", "HEALTHY", "HEALTHY_OR_ELSE_ALL", "UNHEALTHY"]
 HealthStatusType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 ListInstancesPaginatorName = Literal["list_instances"]
 ListNamespacesPaginatorName = Literal["list_namespaces"]
@@ -87,14 +85,15 @@
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
@@ -190,14 +189,15 @@
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
@@ -276,26 +276,28 @@
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
@@ -457,14 +459,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.py`

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
     "CustomHealthStatusType",
     "FilterConditionType",
     "HealthCheckTypeType",
     "HealthStatusFilterType",
     "HealthStatusType",
     "ListInstancesPaginatorName",
@@ -42,14 +43,15 @@
     "ServiceDiscoveryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CustomHealthStatusType = Literal["HEALTHY", "UNHEALTHY"]
 FilterConditionType = Literal["BEGINS_WITH", "BETWEEN", "EQ", "IN"]
 HealthCheckTypeType = Literal["HTTP", "HTTPS", "TCP"]
 HealthStatusFilterType = Literal["ALL", "HEALTHY", "HEALTHY_OR_ELSE_ALL", "UNHEALTHY"]
 HealthStatusType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 ListInstancesPaginatorName = Literal["list_instances"]
 ListNamespacesPaginatorName = Literal["list_namespaces"]
@@ -85,14 +87,15 @@
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
@@ -188,14 +191,15 @@
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
@@ -274,26 +278,28 @@
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
@@ -455,14 +461,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.py` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
     data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
@@ -88,15 +87,14 @@
     "RegisterInstanceResponseTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
-    "DnsConfigOutputTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
@@ -108,18 +106,17 @@
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
-    "CreateServiceRequestRequestTypeDef",
-    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -167,21 +164,19 @@
     {
         "ResourcePath": str,
         "FailureThreshold": int,
     },
     total=False,
 )
 
-
 class HealthCheckConfigTypeDef(
     _RequiredHealthCheckConfigTypeDef, _OptionalHealthCheckConfigTypeDef
 ):
     pass
 
-
 HealthCheckCustomConfigTypeDef = TypedDict(
     "HealthCheckCustomConfigTypeDef",
     {
         "FailureThreshold": int,
     },
     total=False,
 )
@@ -222,21 +217,19 @@
         "QueryParameters": Mapping[str, str],
         "OptionalParameters": Mapping[str, str],
         "HealthStatus": HealthStatusFilterType,
     },
     total=False,
 )
 
-
 class DiscoverInstancesRequestRequestTypeDef(
     _RequiredDiscoverInstancesRequestRequestTypeDef, _OptionalDiscoverInstancesRequestRequestTypeDef
 ):
     pass
 
-
 HttpInstanceSummaryTypeDef = TypedDict(
     "HttpInstanceSummaryTypeDef",
     {
         "InstanceId": str,
         "NamespaceName": str,
         "ServiceName": str,
         "HealthStatus": HealthStatusType,
@@ -279,19 +272,17 @@
     {
         "CreatorRequestId": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
-
 _RequiredGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstancesHealthStatusRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
@@ -300,22 +291,20 @@
         "Instances": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
-
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -393,21 +382,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstancesRequestRequestTypeDef(
     _RequiredListInstancesRequestRequestTypeDef, _OptionalListInstancesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredNamespaceFilterTypeDef = TypedDict(
     "_RequiredNamespaceFilterTypeDef",
     {
         "Name": NamespaceFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -415,19 +402,17 @@
     "_OptionalNamespaceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class NamespaceFilterTypeDef(_RequiredNamespaceFilterTypeDef, _OptionalNamespaceFilterTypeDef):
     pass
 
-
 _RequiredOperationFilterTypeDef = TypedDict(
     "_RequiredOperationFilterTypeDef",
     {
         "Name": OperationFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -435,19 +420,17 @@
     "_OptionalOperationFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class OperationFilterTypeDef(_RequiredOperationFilterTypeDef, _OptionalOperationFilterTypeDef):
     pass
 
-
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Status": OperationStatusType,
     },
     total=False,
@@ -464,19 +447,17 @@
     "_OptionalServiceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
-
 class ServiceFilterTypeDef(_RequiredServiceFilterTypeDef, _OptionalServiceFilterTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -499,21 +480,19 @@
     "_OptionalRegisterInstanceRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -539,22 +518,20 @@
         "CreatorRequestId": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHttpNamespaceRequestRequestTypeDef(
     _RequiredCreateHttpNamespaceRequestRequestTypeDef,
     _OptionalCreateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -674,34 +651,14 @@
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
-_RequiredDnsConfigOutputTypeDef = TypedDict(
-    "_RequiredDnsConfigOutputTypeDef",
-    {
-        "DnsRecords": List[DnsRecordTypeDef],
-    },
-)
-_OptionalDnsConfigOutputTypeDef = TypedDict(
-    "_OptionalDnsConfigOutputTypeDef",
-    {
-        "NamespaceId": str,
-        "RoutingPolicy": RoutingPolicyType,
-    },
-    total=False,
-)
-
-
-class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
-    pass
-
-
 _RequiredDnsConfigTypeDef = TypedDict(
     "_RequiredDnsConfigTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 _OptionalDnsConfigTypeDef = TypedDict(
@@ -709,19 +666,17 @@
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
-
 class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
-
 DnsPropertiesTypeDef = TypedDict(
     "DnsPropertiesTypeDef",
     {
         "HostedZoneId": str,
         "SOA": SOATypeDef,
     },
     total=False,
@@ -768,22 +723,20 @@
     "_OptionalUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdateHttpNamespaceRequestRequestTypeDef(
     _RequiredUpdateHttpNamespaceRequestRequestTypeDef,
     _OptionalUpdateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -799,22 +752,20 @@
     "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListInstancesRequestListInstancesPaginateTypeDef(
     _RequiredListInstancesRequestListInstancesPaginateTypeDef,
     _OptionalListInstancesRequestListInstancesPaginateTypeDef,
 ):
     pass
 
-
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -897,24 +848,50 @@
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
+    {
+        "NamespaceId": str,
+        "CreatorRequestId": str,
+        "Description": str,
+        "DnsConfig": DnsConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "Type": Literal["HTTP"],
+    },
+    total=False,
+)
+
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
+        "DnsConfig": DnsConfigTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -923,53 +900,24 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
+        "DnsConfig": DnsConfigTypeDef,
         "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "NamespaceId": str,
-        "CreatorRequestId": str,
-        "Description": str,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Type": Literal["HTTP"],
-    },
-    total=False,
-)
-
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
-
-DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
@@ -1081,22 +1029,20 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PrivateDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
@@ -1106,22 +1052,20 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PublicDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 PrivateDnsNamespaceChangeTypeDef = TypedDict(
     "PrivateDnsNamespaceChangeTypeDef",
     {
         "Description": str,
         "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
     },
     total=False,
@@ -1164,22 +1108,20 @@
     "_OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
         "Namespace": PublicDnsNamespaceChangeTypeDef,
     },
 )
@@ -1187,13 +1129,12 @@
     "_OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
-
 class UpdatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
     data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -37,14 +37,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
@@ -87,15 +88,14 @@
     "RegisterInstanceResponseTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
-    "DnsConfigOutputTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
@@ -107,18 +107,17 @@
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
-    "CreateServiceRequestRequestTypeDef",
-    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -166,19 +165,21 @@
     {
         "ResourcePath": str,
         "FailureThreshold": int,
     },
     total=False,
 )
 
+
 class HealthCheckConfigTypeDef(
     _RequiredHealthCheckConfigTypeDef, _OptionalHealthCheckConfigTypeDef
 ):
     pass
 
+
 HealthCheckCustomConfigTypeDef = TypedDict(
     "HealthCheckCustomConfigTypeDef",
     {
         "FailureThreshold": int,
     },
     total=False,
 )
@@ -219,19 +220,21 @@
         "QueryParameters": Mapping[str, str],
         "OptionalParameters": Mapping[str, str],
         "HealthStatus": HealthStatusFilterType,
     },
     total=False,
 )
 
+
 class DiscoverInstancesRequestRequestTypeDef(
     _RequiredDiscoverInstancesRequestRequestTypeDef, _OptionalDiscoverInstancesRequestRequestTypeDef
 ):
     pass
 
+
 HttpInstanceSummaryTypeDef = TypedDict(
     "HttpInstanceSummaryTypeDef",
     {
         "InstanceId": str,
         "NamespaceName": str,
         "ServiceName": str,
         "HealthStatus": HealthStatusType,
@@ -274,17 +277,19 @@
     {
         "CreatorRequestId": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
+
 class InstanceTypeDef(_RequiredInstanceTypeDef, _OptionalInstanceTypeDef):
     pass
 
+
 _RequiredGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstancesHealthStatusRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalGetInstancesHealthStatusRequestRequestTypeDef = TypedDict(
@@ -293,20 +298,22 @@
         "Instances": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
+
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -384,19 +391,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstancesRequestRequestTypeDef(
     _RequiredListInstancesRequestRequestTypeDef, _OptionalListInstancesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredNamespaceFilterTypeDef = TypedDict(
     "_RequiredNamespaceFilterTypeDef",
     {
         "Name": NamespaceFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -404,17 +413,19 @@
     "_OptionalNamespaceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class NamespaceFilterTypeDef(_RequiredNamespaceFilterTypeDef, _OptionalNamespaceFilterTypeDef):
     pass
 
+
 _RequiredOperationFilterTypeDef = TypedDict(
     "_RequiredOperationFilterTypeDef",
     {
         "Name": OperationFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -422,17 +433,19 @@
     "_OptionalOperationFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class OperationFilterTypeDef(_RequiredOperationFilterTypeDef, _OptionalOperationFilterTypeDef):
     pass
 
+
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Status": OperationStatusType,
     },
     total=False,
@@ -449,17 +462,19 @@
     "_OptionalServiceFilterTypeDef",
     {
         "Condition": FilterConditionType,
     },
     total=False,
 )
 
+
 class ServiceFilterTypeDef(_RequiredServiceFilterTypeDef, _OptionalServiceFilterTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -482,19 +497,21 @@
     "_OptionalRegisterInstanceRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -520,20 +537,22 @@
         "CreatorRequestId": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHttpNamespaceRequestRequestTypeDef(
     _RequiredCreateHttpNamespaceRequestRequestTypeDef,
     _OptionalCreateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -653,32 +672,14 @@
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
-_RequiredDnsConfigOutputTypeDef = TypedDict(
-    "_RequiredDnsConfigOutputTypeDef",
-    {
-        "DnsRecords": List[DnsRecordTypeDef],
-    },
-)
-_OptionalDnsConfigOutputTypeDef = TypedDict(
-    "_OptionalDnsConfigOutputTypeDef",
-    {
-        "NamespaceId": str,
-        "RoutingPolicy": RoutingPolicyType,
-    },
-    total=False,
-)
-
-class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
-    pass
-
 _RequiredDnsConfigTypeDef = TypedDict(
     "_RequiredDnsConfigTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 _OptionalDnsConfigTypeDef = TypedDict(
@@ -686,17 +687,19 @@
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
+
 class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
+
 DnsPropertiesTypeDef = TypedDict(
     "DnsPropertiesTypeDef",
     {
         "HostedZoneId": str,
         "SOA": SOATypeDef,
     },
     total=False,
@@ -743,20 +746,22 @@
     "_OptionalUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdateHttpNamespaceRequestRequestTypeDef(
     _RequiredUpdateHttpNamespaceRequestRequestTypeDef,
     _OptionalUpdateHttpNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -772,20 +777,22 @@
     "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListInstancesRequestListInstancesPaginateTypeDef(
     _RequiredListInstancesRequestListInstancesPaginateTypeDef,
     _OptionalListInstancesRequestListInstancesPaginateTypeDef,
 ):
     pass
 
+
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -868,24 +875,52 @@
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
+    {
+        "NamespaceId": str,
+        "CreatorRequestId": str,
+        "Description": str,
+        "DnsConfig": DnsConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "Type": Literal["HTTP"],
+    },
+    total=False,
+)
+
+
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
+
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
+        "DnsConfig": DnsConfigTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -894,51 +929,24 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
+        "DnsConfig": DnsConfigTypeDef,
         "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "NamespaceId": str,
-        "CreatorRequestId": str,
-        "Description": str,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Type": Literal["HTTP"],
-    },
-    total=False,
-)
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
-DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
@@ -1050,20 +1058,22 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PrivateDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
@@ -1073,20 +1083,22 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "Properties": PublicDnsNamespacePropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 PrivateDnsNamespaceChangeTypeDef = TypedDict(
     "PrivateDnsNamespaceChangeTypeDef",
     {
         "Description": str,
         "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
     },
     total=False,
@@ -1129,20 +1141,22 @@
     "_OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdatePrivateDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePrivateDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
         "Namespace": PublicDnsNamespaceChangeTypeDef,
     },
 )
@@ -1150,12 +1164,13 @@
     "_OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef",
     {
         "UpdaterRequestId": str,
     },
     total=False,
 )
 
+
 class UpdatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredUpdatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalUpdatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-servicediscovery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,150 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_servicediscovery.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ServiceDiscovery` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/literals/).
+
 ```python
-from types_aiobotocore_servicediscovery.literals import (
-    CustomHealthStatusType,
-    FilterConditionType,
-    HealthCheckTypeType,
-    HealthStatusFilterType,
-    HealthStatusType,
-    ListInstancesPaginatorName,
-    ListNamespacesPaginatorName,
-    ListOperationsPaginatorName,
-    ListServicesPaginatorName,
-    NamespaceFilterNameType,
-    NamespaceTypeType,
-    OperationFilterNameType,
-    OperationStatusType,
-    OperationTargetTypeType,
-    OperationTypeType,
-    RecordTypeType,
-    RoutingPolicyType,
-    ServiceFilterNameType,
-    ServiceTypeOptionType,
-    ServiceTypeType,
-    ServiceDiscoveryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_servicediscovery.literals import CustomHealthStatusType
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceDiscovery` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/type_defs/).
+
 ```python
-from types_aiobotocore_servicediscovery.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    HealthCheckConfigTypeDef,
-    HealthCheckCustomConfigTypeDef,
-    DeleteNamespaceRequestRequestTypeDef,
-    DeleteServiceRequestRequestTypeDef,
-    DeregisterInstanceRequestRequestTypeDef,
-    DiscoverInstancesRequestRequestTypeDef,
-    HttpInstanceSummaryTypeDef,
-    DnsRecordTypeDef,
-    SOATypeDef,
-    GetInstanceRequestRequestTypeDef,
-    InstanceTypeDef,
-    GetInstancesHealthStatusRequestRequestTypeDef,
-    GetNamespaceRequestRequestTypeDef,
-    GetOperationRequestRequestTypeDef,
-    OperationTypeDef,
-    GetServiceRequestRequestTypeDef,
-    HttpNamespaceChangeTypeDef,
-    HttpPropertiesTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    NamespaceFilterTypeDef,
-    OperationFilterTypeDef,
-    OperationSummaryTypeDef,
-    ServiceFilterTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SOAChangeTypeDef,
-    RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterInstanceResponseTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceResponseTypeDef,
-    UpdatePublicDnsNamespaceResponseTypeDef,
-    UpdateServiceResponseTypeDef,
-    DiscoverInstancesResponseTypeDef,
-    DnsConfigChangeTypeDef,
-    DnsConfigOutputTypeDef,
-    DnsConfigTypeDef,
-    DnsPropertiesTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
-    GetInstanceResponseTypeDef,
-    GetOperationResponseTypeDef,
-    UpdateHttpNamespaceRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListNamespacesRequestRequestTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
-    ListOperationsRequestRequestTypeDef,
-    ListOperationsResponseTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesRequestRequestTypeDef,
-    PrivateDnsPropertiesMutableChangeTypeDef,
-    PublicDnsPropertiesMutableChangeTypeDef,
-    ServiceChangeTypeDef,
-    ServiceSummaryTypeDef,
-    ServiceTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    DnsConfigUnionTypeDef,
-    NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesTypeDef,
-    PublicDnsNamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
-    UpdateServiceRequestRequestTypeDef,
-    ListServicesResponseTypeDef,
-    CreateServiceResponseTypeDef,
-    GetServiceResponseTypeDef,
-    NamespaceSummaryTypeDef,
-    NamespaceTypeDef,
-    CreatePrivateDnsNamespaceRequestRequestTypeDef,
-    CreatePublicDnsNamespaceRequestRequestTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
-    ListNamespacesResponseTypeDef,
-    GetNamespaceResponseTypeDef,
-    UpdatePrivateDnsNamespaceRequestRequestTypeDef,
-    UpdatePublicDnsNamespaceRequestRequestTypeDef,
-)
+from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt` & `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

