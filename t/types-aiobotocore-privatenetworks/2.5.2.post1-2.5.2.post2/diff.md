# Comparing `tmp/types-aiobotocore-privatenetworks-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-privatenetworks-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-privatenetworks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-privatenetworks-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-privatenetworks-2.5.2.post1.tar` & `types-aiobotocore-privatenetworks-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.933492 types-aiobotocore-privatenetworks-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-08-02 14:52:49.933492 types-aiobotocore-privatenetworks-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15496 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:49.933492 types-aiobotocore-privatenetworks-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.929492 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-08-02 14:45:07.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28252 2023-08-02 14:45:07.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:06.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.933492 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:49.000000 types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13960 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12416 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2122 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1525 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1524 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23100 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23060 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10088 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10086 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7369 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7361 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28972 2023-08-04 13:47:11.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28919 2023-08-04 13:47:11.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13960 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/LICENSE` & `types-aiobotocore-privatenetworks-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/PKG-INFO` & `types-aiobotocore-privatenetworks-2.5.2.post2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,128 +305,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_privatenetworks.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `Private5G` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/literals/).
+
 ```python
-from types_aiobotocore_privatenetworks.literals import (
-    AcknowledgmentStatusType,
-    DeviceIdentifierFilterKeysType,
-    DeviceIdentifierStatusType,
-    ElevationReferenceType,
-    ElevationUnitType,
-    HealthStatusType,
-    ListDeviceIdentifiersPaginatorName,
-    ListNetworkResourcesPaginatorName,
-    ListNetworkSitesPaginatorName,
-    ListNetworksPaginatorName,
-    ListOrdersPaginatorName,
-    NetworkFilterKeysType,
-    NetworkResourceDefinitionTypeType,
-    NetworkResourceFilterKeysType,
-    NetworkResourceStatusType,
-    NetworkResourceTypeType,
-    NetworkSiteFilterKeysType,
-    NetworkSiteStatusType,
-    NetworkStatusType,
-    OrderFilterKeysType,
-    UpdateTypeType,
-    Private5GServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_privatenetworks.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Private5G` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/type_defs/).
+
 ```python
-from types_aiobotocore_privatenetworks.type_defs import (
-    AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ActivateDeviceIdentifierRequestRequestTypeDef,
-    DeviceIdentifierTypeDef,
-    AddressTypeDef,
-    PositionTypeDef,
-    CreateNetworkRequestRequestTypeDef,
-    NetworkTypeDef,
-    DeactivateDeviceIdentifierRequestRequestTypeDef,
-    DeleteNetworkRequestRequestTypeDef,
-    DeleteNetworkSiteRequestRequestTypeDef,
-    GetDeviceIdentifierRequestRequestTypeDef,
-    GetNetworkRequestRequestTypeDef,
-    GetNetworkResourceRequestRequestTypeDef,
-    GetNetworkSiteRequestRequestTypeDef,
-    GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairTypeDef,
-    TrackingInformationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
-    ActivateDeviceIdentifierResponseTypeDef,
-    DeactivateDeviceIdentifierResponseTypeDef,
-    GetDeviceIdentifierResponseTypeDef,
-    ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    ReturnInformationTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
-    ConfigureAccessPointRequestRequestTypeDef,
-    CreateNetworkResponseTypeDef,
-    DeleteNetworkResponseTypeDef,
-    GetNetworkResponseTypeDef,
-    ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
-    NetworkResourceDefinitionOutputTypeDef,
-    NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
-    NetworkResourceTypeDef,
-    SitePlanOutputTypeDef,
-    SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
-    ConfigureAccessPointResponseTypeDef,
-    GetNetworkResourceResponseTypeDef,
-    ListNetworkResourcesResponseTypeDef,
-    StartNetworkResourceUpdateResponseTypeDef,
-    NetworkSiteTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
-    SitePlanUnionTypeDef,
-    UpdateNetworkSitePlanRequestRequestTypeDef,
-    ActivateNetworkSiteResponseTypeDef,
-    CreateNetworkSiteResponseTypeDef,
-    DeleteNetworkSiteResponseTypeDef,
-    GetNetworkSiteResponseTypeDef,
-    ListNetworkSitesResponseTypeDef,
-    UpdateNetworkSiteResponseTypeDef,
-)
+from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
 
 def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/README.md` & `types-aiobotocore-privatenetworks-2.5.2.post2/README.md`

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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,128 +273,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_privatenetworks.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `Private5G` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/literals/).
+
 ```python
-from types_aiobotocore_privatenetworks.literals import (
-    AcknowledgmentStatusType,
-    DeviceIdentifierFilterKeysType,
-    DeviceIdentifierStatusType,
-    ElevationReferenceType,
-    ElevationUnitType,
-    HealthStatusType,
-    ListDeviceIdentifiersPaginatorName,
-    ListNetworkResourcesPaginatorName,
-    ListNetworkSitesPaginatorName,
-    ListNetworksPaginatorName,
-    ListOrdersPaginatorName,
-    NetworkFilterKeysType,
-    NetworkResourceDefinitionTypeType,
-    NetworkResourceFilterKeysType,
-    NetworkResourceStatusType,
-    NetworkResourceTypeType,
-    NetworkSiteFilterKeysType,
-    NetworkSiteStatusType,
-    NetworkStatusType,
-    OrderFilterKeysType,
-    UpdateTypeType,
-    Private5GServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_privatenetworks.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Private5G` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/type_defs/).
+
 ```python
-from types_aiobotocore_privatenetworks.type_defs import (
-    AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ActivateDeviceIdentifierRequestRequestTypeDef,
-    DeviceIdentifierTypeDef,
-    AddressTypeDef,
-    PositionTypeDef,
-    CreateNetworkRequestRequestTypeDef,
-    NetworkTypeDef,
-    DeactivateDeviceIdentifierRequestRequestTypeDef,
-    DeleteNetworkRequestRequestTypeDef,
-    DeleteNetworkSiteRequestRequestTypeDef,
-    GetDeviceIdentifierRequestRequestTypeDef,
-    GetNetworkRequestRequestTypeDef,
-    GetNetworkResourceRequestRequestTypeDef,
-    GetNetworkSiteRequestRequestTypeDef,
-    GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairTypeDef,
-    TrackingInformationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
-    ActivateDeviceIdentifierResponseTypeDef,
-    DeactivateDeviceIdentifierResponseTypeDef,
-    GetDeviceIdentifierResponseTypeDef,
-    ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    ReturnInformationTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
-    ConfigureAccessPointRequestRequestTypeDef,
-    CreateNetworkResponseTypeDef,
-    DeleteNetworkResponseTypeDef,
-    GetNetworkResponseTypeDef,
-    ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
-    NetworkResourceDefinitionOutputTypeDef,
-    NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
-    NetworkResourceTypeDef,
-    SitePlanOutputTypeDef,
-    SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
-    ConfigureAccessPointResponseTypeDef,
-    GetNetworkResourceResponseTypeDef,
-    ListNetworkResourcesResponseTypeDef,
-    StartNetworkResourceUpdateResponseTypeDef,
-    NetworkSiteTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
-    SitePlanUnionTypeDef,
-    UpdateNetworkSitePlanRequestRequestTypeDef,
-    ActivateNetworkSiteResponseTypeDef,
-    CreateNetworkSiteResponseTypeDef,
-    DeleteNetworkSiteResponseTypeDef,
-    GetNetworkSiteResponseTypeDef,
-    ListNetworkSitesResponseTypeDef,
-    UpdateNetworkSiteResponseTypeDef,
-)
+from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
 
 def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/setup.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-privatenetworks",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__init__.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__init__.pyi` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/__main__.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Private5G 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Private5G 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/client.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -53,46 +54,42 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
-    SitePlanUnionTypeDef,
+    SitePlanTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Private5GClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class Private5GClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
     """
 
     meta: ClientMeta
@@ -101,61 +98,60 @@
     def exceptions(self) -> Exceptions:
         """
         Private5GClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#exceptions)
         """
-
     async def acknowledge_order_receipt(
         self, *, orderArn: str
     ) -> AcknowledgeOrderReceiptResponseTypeDef:
         """
         Acknowledges that the specified network order was received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.acknowledge_order_receipt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#acknowledge_order_receipt)
         """
-
     async def activate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> ActivateDeviceIdentifierResponseTypeDef:
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_device_identifier)
         """
-
     async def activate_network_site(
-        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        shippingAddress: AddressTypeDef,
+        clientToken: str = ...,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_network_site)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#close)
         """
-
     async def configure_access_point(
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
@@ -164,325 +160,297 @@
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#configure_access_point)
         """
-
     async def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network)
         """
-
     async def create_network_site(
         self,
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: SitePlanUnionTypeDef = ...,
+        pendingPlan: SitePlanTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network_site)
         """
-
     async def deactivate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> DeactivateDeviceIdentifierResponseTypeDef:
         """
         Deactivates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.deactivate_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#deactivate_device_identifier)
         """
-
     async def delete_network(
         self, *, networkArn: str, clientToken: str = ...
     ) -> DeleteNetworkResponseTypeDef:
         """
         Deletes the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#delete_network)
         """
-
     async def delete_network_site(
         self, *, networkSiteArn: str, clientToken: str = ...
     ) -> DeleteNetworkSiteResponseTypeDef:
         """
         Deletes the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#delete_network_site)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#generate_presigned_url)
         """
-
     async def get_device_identifier(
         self, *, deviceIdentifierArn: str
     ) -> GetDeviceIdentifierResponseTypeDef:
         """
         Gets the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_device_identifier)
         """
-
     async def get_network(self, *, networkArn: str) -> GetNetworkResponseTypeDef:
         """
         Gets the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network)
         """
-
     async def get_network_resource(
         self, *, networkResourceArn: str
     ) -> GetNetworkResourceResponseTypeDef:
         """
         Gets the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network_resource)
         """
-
     async def get_network_site(self, *, networkSiteArn: str) -> GetNetworkSiteResponseTypeDef:
         """
         Gets the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network_site)
         """
-
     async def get_order(self, *, orderArn: str) -> GetOrderResponseTypeDef:
         """
         Gets the specified order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_order)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_order)
         """
-
     async def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_device_identifiers)
         """
-
     async def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_resources)
         """
-
     async def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_sites)
         """
-
     async def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_networks)
         """
-
     async def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_orders)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_tags_for_resource)
         """
-
     async def ping(self) -> PingResponseTypeDef:
         """
         Checks the health of the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.ping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#ping)
         """
-
     async def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Starts an update of the specified network resource.
+        Use this action to do the following tasks: * Update the duration and renewal
+        status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#start_network_resource_update)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#untag_resource)
         """
-
     async def update_network_site(
         self, *, networkSiteArn: str, clientToken: str = ..., description: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#update_network_site)
         """
-
     async def update_network_site_plan(
-        self, *, networkSiteArn: str, pendingPlan: SitePlanUnionTypeDef, clientToken: str = ...
+        self, *, networkSiteArn: str, pendingPlan: SitePlanTypeDef, clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#update_network_site_plan)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_device_identifiers"]
     ) -> ListDeviceIdentifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_resources"]
     ) -> ListNetworkResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_sites"]
     ) -> ListNetworkSitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_networks"]) -> ListNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "Private5GClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
         """
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/client.pyi` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
+    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -53,42 +54,46 @@
     ListNetworkResourcesResponseTypeDef,
     ListNetworkSitesResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListOrdersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     PositionTypeDef,
-    SitePlanUnionTypeDef,
+    SitePlanTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
     UpdateNetworkSiteResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("Private5GClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class Private5GClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
     """
 
     meta: ClientMeta
@@ -97,55 +102,66 @@
     def exceptions(self) -> Exceptions:
         """
         Private5GClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#exceptions)
         """
+
     async def acknowledge_order_receipt(
         self, *, orderArn: str
     ) -> AcknowledgeOrderReceiptResponseTypeDef:
         """
         Acknowledges that the specified network order was received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.acknowledge_order_receipt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#acknowledge_order_receipt)
         """
+
     async def activate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> ActivateDeviceIdentifierResponseTypeDef:
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_device_identifier)
         """
+
     async def activate_network_site(
-        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
+        self,
+        *,
+        networkSiteArn: str,
+        shippingAddress: AddressTypeDef,
+        clientToken: str = ...,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#activate_network_site)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#close)
         """
+
     async def configure_access_point(
         self,
         *,
         accessPointArn: str,
         cpiSecretKey: str = ...,
         cpiUserId: str = ...,
         cpiUserPassword: str = ...,
@@ -154,295 +170,327 @@
     ) -> ConfigureAccessPointResponseTypeDef:
         """
         Configures the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.configure_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#configure_access_point)
         """
+
     async def create_network(
         self,
         *,
         networkName: str,
         clientToken: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkResponseTypeDef:
         """
         Creates a network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network)
         """
+
     async def create_network_site(
         self,
         *,
         networkArn: str,
         networkSiteName: str,
         availabilityZone: str = ...,
         availabilityZoneId: str = ...,
         clientToken: str = ...,
         description: str = ...,
-        pendingPlan: SitePlanUnionTypeDef = ...,
+        pendingPlan: SitePlanTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateNetworkSiteResponseTypeDef:
         """
         Creates a network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.create_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#create_network_site)
         """
+
     async def deactivate_device_identifier(
         self, *, deviceIdentifierArn: str, clientToken: str = ...
     ) -> DeactivateDeviceIdentifierResponseTypeDef:
         """
         Deactivates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.deactivate_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#deactivate_device_identifier)
         """
+
     async def delete_network(
         self, *, networkArn: str, clientToken: str = ...
     ) -> DeleteNetworkResponseTypeDef:
         """
         Deletes the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#delete_network)
         """
+
     async def delete_network_site(
         self, *, networkSiteArn: str, clientToken: str = ...
     ) -> DeleteNetworkSiteResponseTypeDef:
         """
         Deletes the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.delete_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#delete_network_site)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#generate_presigned_url)
         """
+
     async def get_device_identifier(
         self, *, deviceIdentifierArn: str
     ) -> GetDeviceIdentifierResponseTypeDef:
         """
         Gets the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_device_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_device_identifier)
         """
+
     async def get_network(self, *, networkArn: str) -> GetNetworkResponseTypeDef:
         """
         Gets the specified network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network)
         """
+
     async def get_network_resource(
         self, *, networkResourceArn: str
     ) -> GetNetworkResourceResponseTypeDef:
         """
         Gets the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network_resource)
         """
+
     async def get_network_site(self, *, networkSiteArn: str) -> GetNetworkSiteResponseTypeDef:
         """
         Gets the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_network_site)
         """
+
     async def get_order(self, *, orderArn: str) -> GetOrderResponseTypeDef:
         """
         Gets the specified order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_order)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_order)
         """
+
     async def list_device_identifiers(
         self,
         *,
         networkArn: str,
         filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListDeviceIdentifiersResponseTypeDef:
         """
         Lists device identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_device_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_device_identifiers)
         """
+
     async def list_network_resources(
         self,
         *,
         networkArn: str,
         filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkResourcesResponseTypeDef:
         """
         Lists network resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_resources)
         """
+
     async def list_network_sites(
         self,
         *,
         networkArn: str,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworkSitesResponseTypeDef:
         """
         Lists network sites.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_network_sites)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_network_sites)
         """
+
     async def list_networks(
         self,
         *,
         filters: Mapping[Literal["STATUS"], Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListNetworksResponseTypeDef:
         """
         Lists networks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_networks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_networks)
         """
+
     async def list_orders(
         self,
         *,
         networkArn: str,
         filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,
         maxResults: int = ...,
         startToken: str = ...
     ) -> ListOrdersResponseTypeDef:
         """
         Lists orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_orders)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_orders)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#list_tags_for_resource)
         """
+
     async def ping(self) -> PingResponseTypeDef:
         """
         Checks the health of the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.ping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#ping)
         """
+
     async def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
+        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Starts an update of the specified network resource.
+        Use this action to do the following tasks: * Update the duration and renewal
+        status of the commitment period for a radio unit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#start_network_resource_update)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#untag_resource)
         """
+
     async def update_network_site(
         self, *, networkSiteArn: str, clientToken: str = ..., description: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#update_network_site)
         """
+
     async def update_network_site_plan(
-        self, *, networkSiteArn: str, pendingPlan: SitePlanUnionTypeDef, clientToken: str = ...
+        self, *, networkSiteArn: str, pendingPlan: SitePlanTypeDef, clientToken: str = ...
     ) -> UpdateNetworkSiteResponseTypeDef:
         """
         Updates the specified network site plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.update_network_site_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#update_network_site_plan)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_device_identifiers"]
     ) -> ListDeviceIdentifiersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_resources"]
     ) -> ListNetworkResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_network_sites"]
     ) -> ListNetworkSitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_networks"]) -> ListNetworksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "Private5GClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/client/)
         """
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/literals.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AcknowledgmentStatusType",
+    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -45,14 +46,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
+CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -74,15 +76,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["REPLACE", "RETURN"]
+UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -91,14 +93,15 @@
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
@@ -194,14 +197,15 @@
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
@@ -280,26 +284,28 @@
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

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/literals.pyi` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AcknowledgmentStatusType",
+    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -43,14 +44,15 @@
     "Private5GServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
+CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -72,15 +74,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["REPLACE", "RETURN"]
+UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -89,14 +91,15 @@
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
@@ -192,14 +195,15 @@
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
@@ -278,26 +282,28 @@
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

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/paginator.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/paginator.pyi` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/type_defs.py` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
     data: AcknowledgeOrderReceiptRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -42,14 +43,15 @@
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
+    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -71,43 +73,42 @@
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
+    "CommitmentInformationTypeDef",
+    "OrderedResourceDefinitionTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListOrdersRequestListOrdersPaginateTypeDef",
-    "NetworkResourceDefinitionOutputTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "OrderTypeDef",
     "NetworkResourceTypeDef",
-    "SitePlanOutputTypeDef",
+    "OrderTypeDef",
     "SitePlanTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
-    "NetworkSiteTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
-    "SitePlanUnionTypeDef",
+    "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -180,26 +181,35 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
+        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
 
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
 
+CommitmentConfigurationTypeDef = TypedDict(
+    "CommitmentConfigurationTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
+
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -586,58 +596,104 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
+_RequiredCommitmentInformationTypeDef = TypedDict(
+    "_RequiredCommitmentInformationTypeDef",
     {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+    },
+)
+_OptionalCommitmentInformationTypeDef = TypedDict(
+    "_OptionalCommitmentInformationTypeDef",
+    {
+        "expiresOn": datetime,
+        "startAt": datetime,
     },
     total=False,
 )
 
+
+class CommitmentInformationTypeDef(
+    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
+):
+    pass
+
+
+_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
+    "_RequiredOrderedResourceDefinitionTypeDef",
+    {
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
+    },
+)
+_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
+    "_OptionalOrderedResourceDefinitionTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class OrderedResourceDefinitionTypeDef(
+    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
+):
+    pass
+
+
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
 
@@ -806,76 +862,41 @@
 class ListOrdersRequestListOrdersPaginateTypeDef(
     _RequiredListOrdersRequestListOrdersPaginateTypeDef,
     _OptionalListOrdersRequestListOrdersPaginateTypeDef,
 ):
     pass
 
 
-_RequiredNetworkResourceDefinitionOutputTypeDef = TypedDict(
-    "_RequiredNetworkResourceDefinitionOutputTypeDef",
-    {
-        "count": int,
-        "type": NetworkResourceDefinitionTypeType,
-    },
-)
-_OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
-    "_OptionalNetworkResourceDefinitionOutputTypeDef",
-    {
-        "options": List[NameValuePairTypeDef],
-    },
-    total=False,
-)
-
-
-class NetworkResourceDefinitionOutputTypeDef(
-    _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
-        "options": Sequence[NameValuePairTypeDef],
+        "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
-
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
+        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -887,148 +908,153 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-SitePlanOutputTypeDef = TypedDict(
-    "SitePlanOutputTypeDef",
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "orderedResources": List[OrderedResourceDefinitionTypeDef],
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
-        "options": Sequence[NameValuePairTypeDef],
-        "resourceDefinitions": Sequence[NetworkResourceDefinitionTypeDef],
+        "options": List[NameValuePairTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
+ConfigureAccessPointResponseTypeDef = TypedDict(
+    "ConfigureAccessPointResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "accessPoint": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
+GetNetworkResourceResponseTypeDef = TypedDict(
+    "GetNetworkResourceResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+ListNetworkResourcesResponseTypeDef = TypedDict(
+    "ListNetworkResourcesResponseTypeDef",
     {
+        "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigureAccessPointResponseTypeDef = TypedDict(
-    "ConfigureAccessPointResponseTypeDef",
+StartNetworkResourceUpdateResponseTypeDef = TypedDict(
+    "StartNetworkResourceUpdateResponseTypeDef",
     {
-        "accessPoint": NetworkResourceTypeDef,
+        "networkResource": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetNetworkResourceResponseTypeDef = TypedDict(
-    "GetNetworkResourceResponseTypeDef",
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
-        "tags": Dict[str, str],
+        "order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListNetworkResourcesResponseTypeDef = TypedDict(
-    "ListNetworkResourcesResponseTypeDef",
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
     {
-        "networkResources": List[NetworkResourceTypeDef],
-        "nextToken": str,
+        "order": OrderTypeDef,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartNetworkResourceUpdateResponseTypeDef = TypedDict(
-    "StartNetworkResourceUpdateResponseTypeDef",
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "nextToken": str,
+        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNetworkSiteTypeDef = TypedDict(
-    "_RequiredNetworkSiteTypeDef",
+_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
-        "networkSiteArn": str,
         "networkSiteName": str,
-        "status": NetworkSiteStatusType,
     },
 )
-_OptionalNetworkSiteTypeDef = TypedDict(
-    "_OptionalNetworkSiteTypeDef",
+_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "createdAt": datetime,
-        "currentPlan": SitePlanOutputTypeDef,
+        "clientToken": str,
         "description": str,
-        "pendingPlan": SitePlanOutputTypeDef,
-        "statusReason": str,
+        "pendingPlan": SitePlanTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
+class CreateNetworkSiteRequestRequestTypeDef(
+    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
+):
     pass
 
 
-_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
+_RequiredNetworkSiteTypeDef = TypedDict(
+    "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
+        "networkSiteArn": str,
         "networkSiteName": str,
+        "status": NetworkSiteStatusType,
     },
 )
-_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
+_OptionalNetworkSiteTypeDef = TypedDict(
+    "_OptionalNetworkSiteTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "clientToken": str,
+        "createdAt": datetime,
+        "currentPlan": SitePlanTypeDef,
         "description": str,
         "pendingPlan": SitePlanTypeDef,
-        "tags": Mapping[str, str],
+        "statusReason": str,
     },
     total=False,
 )
 
 
-class CreateNetworkSiteRequestRequestTypeDef(
-    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
-):
+class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
 
-SitePlanUnionTypeDef = Union[SitePlanTypeDef, SitePlanOutputTypeDef]
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks/type_defs.pyi` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
     data: AcknowledgeOrderReceiptRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
+    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -41,14 +42,15 @@
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
+    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -70,43 +72,42 @@
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
+    "CommitmentInformationTypeDef",
+    "OrderedResourceDefinitionTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListOrdersRequestListOrdersPaginateTypeDef",
-    "NetworkResourceDefinitionOutputTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "OrderTypeDef",
     "NetworkResourceTypeDef",
-    "SitePlanOutputTypeDef",
+    "OrderTypeDef",
     "SitePlanTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
-    "NetworkSiteTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
-    "SitePlanUnionTypeDef",
+    "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
     "ListNetworkSitesResponseTypeDef",
     "UpdateNetworkSiteResponseTypeDef",
@@ -177,24 +178,33 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
+        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+CommitmentConfigurationTypeDef = TypedDict(
+    "CommitmentConfigurationTypeDef",
+    {
+        "automaticRenewal": bool,
+        "commitmentLength": CommitmentLengthType,
+    },
+)
+
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -559,56 +569,98 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
+_RequiredCommitmentInformationTypeDef = TypedDict(
+    "_RequiredCommitmentInformationTypeDef",
     {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+    },
+)
+_OptionalCommitmentInformationTypeDef = TypedDict(
+    "_OptionalCommitmentInformationTypeDef",
+    {
+        "expiresOn": datetime,
+        "startAt": datetime,
+    },
+    total=False,
+)
+
+class CommitmentInformationTypeDef(
+    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
+):
+    pass
+
+_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
+    "_RequiredOrderedResourceDefinitionTypeDef",
+    {
+        "count": int,
+        "type": NetworkResourceDefinitionTypeType,
+    },
+)
+_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
+    "_OptionalOrderedResourceDefinitionTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
+class OrderedResourceDefinitionTypeDef(
+    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
+):
+    pass
+
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
 class StartNetworkResourceUpdateRequestRequestTypeDef(
@@ -765,72 +817,39 @@
 
 class ListOrdersRequestListOrdersPaginateTypeDef(
     _RequiredListOrdersRequestListOrdersPaginateTypeDef,
     _OptionalListOrdersRequestListOrdersPaginateTypeDef,
 ):
     pass
 
-_RequiredNetworkResourceDefinitionOutputTypeDef = TypedDict(
-    "_RequiredNetworkResourceDefinitionOutputTypeDef",
-    {
-        "count": int,
-        "type": NetworkResourceDefinitionTypeType,
-    },
-)
-_OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
-    "_OptionalNetworkResourceDefinitionOutputTypeDef",
-    {
-        "options": List[NameValuePairTypeDef],
-    },
-    total=False,
-)
-
-class NetworkResourceDefinitionOutputTypeDef(
-    _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredNetworkResourceDefinitionTypeDef = TypedDict(
     "_RequiredNetworkResourceDefinitionTypeDef",
     {
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionTypeDef",
     {
-        "options": Sequence[NameValuePairTypeDef],
+        "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
-
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
+        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -842,144 +861,149 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-SitePlanOutputTypeDef = TypedDict(
-    "SitePlanOutputTypeDef",
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
     {
-        "options": List[NameValuePairTypeDef],
-        "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "orderedResources": List[OrderedResourceDefinitionTypeDef],
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
-        "options": Sequence[NameValuePairTypeDef],
-        "resourceDefinitions": Sequence[NetworkResourceDefinitionTypeDef],
+        "options": List[NameValuePairTypeDef],
+        "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
+ConfigureAccessPointResponseTypeDef = TypedDict(
+    "ConfigureAccessPointResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "accessPoint": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
+GetNetworkResourceResponseTypeDef = TypedDict(
+    "GetNetworkResourceResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "networkResource": NetworkResourceTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+ListNetworkResourcesResponseTypeDef = TypedDict(
+    "ListNetworkResourcesResponseTypeDef",
     {
+        "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
-        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigureAccessPointResponseTypeDef = TypedDict(
-    "ConfigureAccessPointResponseTypeDef",
+StartNetworkResourceUpdateResponseTypeDef = TypedDict(
+    "StartNetworkResourceUpdateResponseTypeDef",
     {
-        "accessPoint": NetworkResourceTypeDef,
+        "networkResource": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetNetworkResourceResponseTypeDef = TypedDict(
-    "GetNetworkResourceResponseTypeDef",
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
-        "tags": Dict[str, str],
+        "order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListNetworkResourcesResponseTypeDef = TypedDict(
-    "ListNetworkResourcesResponseTypeDef",
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
     {
-        "networkResources": List[NetworkResourceTypeDef],
-        "nextToken": str,
+        "order": OrderTypeDef,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartNetworkResourceUpdateResponseTypeDef = TypedDict(
-    "StartNetworkResourceUpdateResponseTypeDef",
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "nextToken": str,
+        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNetworkSiteTypeDef = TypedDict(
-    "_RequiredNetworkSiteTypeDef",
+_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
         "networkArn": str,
-        "networkSiteArn": str,
         "networkSiteName": str,
-        "status": NetworkSiteStatusType,
     },
 )
-_OptionalNetworkSiteTypeDef = TypedDict(
-    "_OptionalNetworkSiteTypeDef",
+_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "createdAt": datetime,
-        "currentPlan": SitePlanOutputTypeDef,
+        "clientToken": str,
         "description": str,
-        "pendingPlan": SitePlanOutputTypeDef,
-        "statusReason": str,
+        "pendingPlan": SitePlanTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
+class CreateNetworkSiteRequestRequestTypeDef(
+    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
+):
     pass
 
-_RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkSiteRequestRequestTypeDef",
+_RequiredNetworkSiteTypeDef = TypedDict(
+    "_RequiredNetworkSiteTypeDef",
     {
         "networkArn": str,
+        "networkSiteArn": str,
         "networkSiteName": str,
+        "status": NetworkSiteStatusType,
     },
 )
-_OptionalCreateNetworkSiteRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkSiteRequestRequestTypeDef",
+_OptionalNetworkSiteTypeDef = TypedDict(
+    "_OptionalNetworkSiteTypeDef",
     {
         "availabilityZone": str,
         "availabilityZoneId": str,
-        "clientToken": str,
+        "createdAt": datetime,
+        "currentPlan": SitePlanTypeDef,
         "description": str,
         "pendingPlan": SitePlanTypeDef,
-        "tags": Mapping[str, str],
+        "statusReason": str,
     },
     total=False,
 )
 
-class CreateNetworkSiteRequestRequestTypeDef(
-    _RequiredCreateNetworkSiteRequestRequestTypeDef, _OptionalCreateNetworkSiteRequestRequestTypeDef
-):
+class NetworkSiteTypeDef(_RequiredNetworkSiteTypeDef, _OptionalNetworkSiteTypeDef):
     pass
 
-SitePlanUnionTypeDef = Union[SitePlanTypeDef, SitePlanOutputTypeDef]
 _RequiredUpdateNetworkSitePlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSitePlanRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "pendingPlan": SitePlanTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/PKG-INFO` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
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
 [types-aiobotocore-privatenetworks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,128 +305,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_privatenetworks.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `Private5G` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/literals/).
+
 ```python
-from types_aiobotocore_privatenetworks.literals import (
-    AcknowledgmentStatusType,
-    DeviceIdentifierFilterKeysType,
-    DeviceIdentifierStatusType,
-    ElevationReferenceType,
-    ElevationUnitType,
-    HealthStatusType,
-    ListDeviceIdentifiersPaginatorName,
-    ListNetworkResourcesPaginatorName,
-    ListNetworkSitesPaginatorName,
-    ListNetworksPaginatorName,
-    ListOrdersPaginatorName,
-    NetworkFilterKeysType,
-    NetworkResourceDefinitionTypeType,
-    NetworkResourceFilterKeysType,
-    NetworkResourceStatusType,
-    NetworkResourceTypeType,
-    NetworkSiteFilterKeysType,
-    NetworkSiteStatusType,
-    NetworkStatusType,
-    OrderFilterKeysType,
-    UpdateTypeType,
-    Private5GServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType
 
 
 def check_value(value: AcknowledgmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_privatenetworks.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Private5G` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/type_defs/).
+
 ```python
-from types_aiobotocore_privatenetworks.type_defs import (
-    AcknowledgeOrderReceiptRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ActivateDeviceIdentifierRequestRequestTypeDef,
-    DeviceIdentifierTypeDef,
-    AddressTypeDef,
-    PositionTypeDef,
-    CreateNetworkRequestRequestTypeDef,
-    NetworkTypeDef,
-    DeactivateDeviceIdentifierRequestRequestTypeDef,
-    DeleteNetworkRequestRequestTypeDef,
-    DeleteNetworkSiteRequestRequestTypeDef,
-    GetDeviceIdentifierRequestRequestTypeDef,
-    GetNetworkRequestRequestTypeDef,
-    GetNetworkResourceRequestRequestTypeDef,
-    GetNetworkSiteRequestRequestTypeDef,
-    GetOrderRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceIdentifiersRequestRequestTypeDef,
-    ListNetworkResourcesRequestRequestTypeDef,
-    ListNetworkSitesRequestRequestTypeDef,
-    ListNetworksRequestRequestTypeDef,
-    ListOrdersRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairTypeDef,
-    TrackingInformationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateNetworkSiteRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PingResponseTypeDef,
-    ActivateDeviceIdentifierResponseTypeDef,
-    DeactivateDeviceIdentifierResponseTypeDef,
-    GetDeviceIdentifierResponseTypeDef,
-    ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    ReturnInformationTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
-    ConfigureAccessPointRequestRequestTypeDef,
-    CreateNetworkResponseTypeDef,
-    DeleteNetworkResponseTypeDef,
-    GetNetworkResponseTypeDef,
-    ListNetworksResponseTypeDef,
-    ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
-    ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
-    ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
-    ListNetworksRequestListNetworksPaginateTypeDef,
-    ListOrdersRequestListOrdersPaginateTypeDef,
-    NetworkResourceDefinitionOutputTypeDef,
-    NetworkResourceDefinitionTypeDef,
-    OrderTypeDef,
-    NetworkResourceTypeDef,
-    SitePlanOutputTypeDef,
-    SitePlanTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
-    ConfigureAccessPointResponseTypeDef,
-    GetNetworkResourceResponseTypeDef,
-    ListNetworkResourcesResponseTypeDef,
-    StartNetworkResourceUpdateResponseTypeDef,
-    NetworkSiteTypeDef,
-    CreateNetworkSiteRequestRequestTypeDef,
-    SitePlanUnionTypeDef,
-    UpdateNetworkSitePlanRequestRequestTypeDef,
-    ActivateNetworkSiteResponseTypeDef,
-    CreateNetworkSiteResponseTypeDef,
-    DeleteNetworkSiteResponseTypeDef,
-    GetNetworkSiteResponseTypeDef,
-    ListNetworkSitesResponseTypeDef,
-    UpdateNetworkSiteResponseTypeDef,
-)
+from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef
 
 
 def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post1/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt` & `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

