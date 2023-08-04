# Comparing `tmp/types-aiobotocore-outposts-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-outposts-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-outposts-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-outposts-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-outposts-2.5.2.post1.tar` & `types-aiobotocore-outposts-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.793503 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20144 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-08-02 14:44:34.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21379 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.346643 types-aiobotocore-outposts-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13595 2023-08-04 13:59:20.346643 types-aiobotocore-outposts-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12073 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.346643 types-aiobotocore-outposts-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.346643 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1611 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1610 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23137 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23096 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11619 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11617 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8135 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8127 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24602 2023-08-04 13:46:21.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24579 2023-08-04 13:46:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:19.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.346643 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13595 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:20.000000 types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/LICENSE` & `types-aiobotocore-outposts-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2.post1/PKG-INFO` & `types-aiobotocore-outposts-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +71,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -258,132 +259,82 @@
 
 session = get_session()
 async with session.create_client("outposts") as client:
     client: OutpostsClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`types_aiobotocore_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from aiobotocore.session import get_session
+
+from types_aiobotocore_outposts import OutpostsClient
+from types_aiobotocore_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+session = get_session()
+async with session.create_client("outposts") as client:
+    client: OutpostsClient
+
+    # Explicit type annotations are optional here
+    # Types should be correctly discovered by mypy and IDEs
+    get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+        "get_outpost_instance_types"
+    )
+    list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator(
+        "list_catalog_items"
+    )
+    list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+    list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+    list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/literals/).
+
 ```python
-from types_aiobotocore_outposts.literals import (
-    AddressTypeType,
-    AssetStateType,
-    AssetTypeType,
-    CatalogItemClassType,
-    CatalogItemStatusType,
-    ComputeAssetStateType,
-    FiberOpticCableTypeType,
-    LineItemStatusType,
-    MaximumSupportedWeightLbsType,
-    OpticalStandardType,
-    OrderStatusType,
-    OrderTypeType,
-    PaymentOptionType,
-    PaymentTermType,
-    PowerConnectorType,
-    PowerDrawKvaType,
-    PowerFeedDropType,
-    PowerPhaseType,
-    ShipmentCarrierType,
-    SupportedHardwareTypeType,
-    SupportedStorageEnumType,
-    UplinkCountType,
-    UplinkGbpsType,
-    OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_outposts.literals import AddressTypeType
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/type_defs/).
+
 ```python
-from types_aiobotocore_outposts.type_defs import (
-    AddressTypeDef,
-    AssetLocationTypeDef,
-    ComputeAttributesTypeDef,
-    CancelOrderInputRequestTypeDef,
-    EC2CapacityTypeDef,
-    ConnectionDetailsTypeDef,
-    LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateOutpostInputRequestTypeDef,
-    OutpostTypeDef,
-    RackPhysicalPropertiesTypeDef,
-    DeleteOutpostInputRequestTypeDef,
-    DeleteSiteInputRequestTypeDef,
-    GetCatalogItemInputRequestTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    GetOrderInputRequestTypeDef,
-    GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputRequestTypeDef,
-    InstanceTypeItemTypeDef,
-    GetSiteAddressInputRequestTypeDef,
-    GetSiteInputRequestTypeDef,
-    LineItemAssetInformationTypeDef,
-    ShipmentInformationTypeDef,
-    ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputRequestTypeDef,
-    OrderSummaryTypeDef,
-    ListOutpostsInputRequestTypeDef,
-    ListSitesInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartConnectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateOutpostInputRequestTypeDef,
-    UpdateSiteInputRequestTypeDef,
-    UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    UpdateSiteAddressInputRequestTypeDef,
-    AssetInfoTypeDef,
-    CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
-    GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
-    CreateOutpostOutputTypeDef,
-    GetOutpostOutputTypeDef,
-    ListOutpostsOutputTypeDef,
-    UpdateOutpostOutputTypeDef,
-    CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
-    GetOutpostInstanceTypesOutputTypeDef,
-    LineItemTypeDef,
-    ListOrdersOutputTypeDef,
-    ListAssetsOutputTypeDef,
-    GetCatalogItemOutputTypeDef,
-    ListCatalogItemsOutputTypeDef,
-    CreateSiteOutputTypeDef,
-    GetSiteOutputTypeDef,
-    ListSitesOutputTypeDef,
-    UpdateSiteOutputTypeDef,
-    UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
-    CreateOrderOutputTypeDef,
-    GetOrderOutputTypeDef,
-)
+from types_aiobotocore_outposts.type_defs import AddressTypeDef
 
 
 def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/README.md` & `types-aiobotocore-outposts-2.5.2.post2/README.md`

 * *Files 15% similar despite different names*

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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -39,14 +39,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -226,132 +227,82 @@
 
 session = get_session()
 async with session.create_client("outposts") as client:
     client: OutpostsClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`types_aiobotocore_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from aiobotocore.session import get_session
+
+from types_aiobotocore_outposts import OutpostsClient
+from types_aiobotocore_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+session = get_session()
+async with session.create_client("outposts") as client:
+    client: OutpostsClient
+
+    # Explicit type annotations are optional here
+    # Types should be correctly discovered by mypy and IDEs
+    get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+        "get_outpost_instance_types"
+    )
+    list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator(
+        "list_catalog_items"
+    )
+    list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+    list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+    list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/literals/).
+
 ```python
-from types_aiobotocore_outposts.literals import (
-    AddressTypeType,
-    AssetStateType,
-    AssetTypeType,
-    CatalogItemClassType,
-    CatalogItemStatusType,
-    ComputeAssetStateType,
-    FiberOpticCableTypeType,
-    LineItemStatusType,
-    MaximumSupportedWeightLbsType,
-    OpticalStandardType,
-    OrderStatusType,
-    OrderTypeType,
-    PaymentOptionType,
-    PaymentTermType,
-    PowerConnectorType,
-    PowerDrawKvaType,
-    PowerFeedDropType,
-    PowerPhaseType,
-    ShipmentCarrierType,
-    SupportedHardwareTypeType,
-    SupportedStorageEnumType,
-    UplinkCountType,
-    UplinkGbpsType,
-    OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_outposts.literals import AddressTypeType
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/type_defs/).
+
 ```python
-from types_aiobotocore_outposts.type_defs import (
-    AddressTypeDef,
-    AssetLocationTypeDef,
-    ComputeAttributesTypeDef,
-    CancelOrderInputRequestTypeDef,
-    EC2CapacityTypeDef,
-    ConnectionDetailsTypeDef,
-    LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateOutpostInputRequestTypeDef,
-    OutpostTypeDef,
-    RackPhysicalPropertiesTypeDef,
-    DeleteOutpostInputRequestTypeDef,
-    DeleteSiteInputRequestTypeDef,
-    GetCatalogItemInputRequestTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    GetOrderInputRequestTypeDef,
-    GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputRequestTypeDef,
-    InstanceTypeItemTypeDef,
-    GetSiteAddressInputRequestTypeDef,
-    GetSiteInputRequestTypeDef,
-    LineItemAssetInformationTypeDef,
-    ShipmentInformationTypeDef,
-    ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputRequestTypeDef,
-    OrderSummaryTypeDef,
-    ListOutpostsInputRequestTypeDef,
-    ListSitesInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartConnectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateOutpostInputRequestTypeDef,
-    UpdateSiteInputRequestTypeDef,
-    UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    UpdateSiteAddressInputRequestTypeDef,
-    AssetInfoTypeDef,
-    CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
-    GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
-    CreateOutpostOutputTypeDef,
-    GetOutpostOutputTypeDef,
-    ListOutpostsOutputTypeDef,
-    UpdateOutpostOutputTypeDef,
-    CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
-    GetOutpostInstanceTypesOutputTypeDef,
-    LineItemTypeDef,
-    ListOrdersOutputTypeDef,
-    ListAssetsOutputTypeDef,
-    GetCatalogItemOutputTypeDef,
-    ListCatalogItemsOutputTypeDef,
-    CreateSiteOutputTypeDef,
-    GetSiteOutputTypeDef,
-    ListSitesOutputTypeDef,
-    UpdateSiteOutputTypeDef,
-    UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
-    CreateOrderOutputTypeDef,
-    GetOrderOutputTypeDef,
-)
+from types_aiobotocore_outposts.type_defs import AddressTypeDef
 
 
 def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/setup.py` & `types-aiobotocore-outposts-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-outposts",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__main__.py` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Outposts 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Outposts 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.py` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from types_aiobotocore_outposts.client import OutpostsClient
 
     session = get_session()
     async with session.create_client("outposts") as client:
         client: OutpostsClient
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
@@ -33,14 +34,22 @@
     PowerFeedDropType,
     PowerPhaseType,
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
+from .paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
@@ -60,14 +69,20 @@
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = ("OutpostsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -434,14 +449,60 @@
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_site_rack_physical_properties)
         """
 
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_instance_types"]
+    ) -> GetOutpostInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_catalog_items"]
+    ) -> ListCatalogItemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_outposts"]) -> ListOutpostsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_sites"]) -> ListSitesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+
     async def __aenter__(self) -> "OutpostsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/)
         """
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.pyi` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from types_aiobotocore_outposts.client import OutpostsClient
 
     session = get_session()
     async with session.create_client("outposts") as client:
         client: OutpostsClient
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AddressTypeType,
     AssetStateType,
@@ -33,14 +34,22 @@
     PowerFeedDropType,
     PowerPhaseType,
     SupportedHardwareTypeType,
     SupportedStorageEnumType,
     UplinkCountType,
     UplinkGbpsType,
 )
+from .paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
 from .type_defs import (
     AddressTypeDef,
     CreateOrderOutputTypeDef,
     CreateOutpostOutputTypeDef,
     CreateSiteOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     GetConnectionResponseTypeDef,
@@ -60,14 +69,19 @@
     StartConnectionResponseTypeDef,
     UpdateOutpostOutputTypeDef,
     UpdateSiteAddressOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("OutpostsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -401,14 +415,54 @@
     ) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:
         """
         Update the physical and logistical details for a rack at a site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#update_site_rack_physical_properties)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["get_outpost_instance_types"]
+    ) -> GetOutpostInstanceTypesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_assets"]) -> ListAssetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_catalog_items"]
+    ) -> ListCatalogItemsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_orders"]) -> ListOrdersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_outposts"]) -> ListOutpostsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_sites"]) -> ListSitesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/#get_paginator)
+        """
     async def __aenter__(self) -> "OutpostsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/client/)
         """
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.py` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,21 @@
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
+    "GetOutpostInstanceTypesPaginatorName",
     "LineItemStatusType",
+    "ListAssetsPaginatorName",
+    "ListCatalogItemsPaginatorName",
+    "ListOrdersPaginatorName",
+    "ListOutpostsPaginatorName",
+    "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
     "OrderTypeType",
     "PaymentOptionType",
     "PaymentTermType",
     "PowerConnectorType",
@@ -42,36 +48,43 @@
     "SupportedHardwareTypeType",
     "SupportedStorageEnumType",
     "UplinkCountType",
     "UplinkGbpsType",
     "OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
-AssetStateType = Literal["ACTIVE", "RETIRING"]
+AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
+GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
+ListAssetsPaginatorName = Literal["list_assets"]
+ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
+ListOrdersPaginatorName = Literal["list_orders"]
+ListOutpostsPaginatorName = Literal["list_outposts"]
+ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
 OpticalStandardType = Literal[
     "OPTIC_1000BASE_LX",
     "OPTIC_1000BASE_SX",
     "OPTIC_100GBASE_CWDM4",
@@ -133,14 +146,15 @@
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
@@ -236,14 +250,15 @@
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
@@ -322,26 +337,28 @@
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
@@ -481,14 +498,22 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "get_outpost_instance_types",
+    "list_assets",
+    "list_catalog_items",
+    "list_orders",
+    "list_outposts",
+    "list_sites",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.pyi` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,21 @@
     "AddressTypeType",
     "AssetStateType",
     "AssetTypeType",
     "CatalogItemClassType",
     "CatalogItemStatusType",
     "ComputeAssetStateType",
     "FiberOpticCableTypeType",
+    "GetOutpostInstanceTypesPaginatorName",
     "LineItemStatusType",
+    "ListAssetsPaginatorName",
+    "ListCatalogItemsPaginatorName",
+    "ListOrdersPaginatorName",
+    "ListOutpostsPaginatorName",
+    "ListSitesPaginatorName",
     "MaximumSupportedWeightLbsType",
     "OpticalStandardType",
     "OrderStatusType",
     "OrderTypeType",
     "PaymentOptionType",
     "PaymentTermType",
     "PowerConnectorType",
@@ -41,35 +47,42 @@
     "SupportedHardwareTypeType",
     "SupportedStorageEnumType",
     "UplinkCountType",
     "UplinkGbpsType",
     "OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 AddressTypeType = Literal["OPERATING_ADDRESS", "SHIPPING_ADDRESS"]
-AssetStateType = Literal["ACTIVE", "RETIRING"]
+AssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 AssetTypeType = Literal["COMPUTE"]
 CatalogItemClassType = Literal["RACK", "SERVER"]
 CatalogItemStatusType = Literal["AVAILABLE", "DISCONTINUED"]
 ComputeAssetStateType = Literal["ACTIVE", "ISOLATED", "RETIRING"]
 FiberOpticCableTypeType = Literal["MULTI_MODE", "SINGLE_MODE"]
+GetOutpostInstanceTypesPaginatorName = Literal["get_outpost_instance_types"]
 LineItemStatusType = Literal[
     "BUILDING",
     "CANCELLED",
     "DELIVERED",
     "ERROR",
     "INSTALLED",
     "INSTALLING",
     "PREPARING",
     "REPLACED",
     "SHIPPED",
 ]
+ListAssetsPaginatorName = Literal["list_assets"]
+ListCatalogItemsPaginatorName = Literal["list_catalog_items"]
+ListOrdersPaginatorName = Literal["list_orders"]
+ListOutpostsPaginatorName = Literal["list_outposts"]
+ListSitesPaginatorName = Literal["list_sites"]
 MaximumSupportedWeightLbsType = Literal[
     "MAX_1400_LBS", "MAX_1600_LBS", "MAX_1800_LBS", "MAX_2000_LBS", "NO_LIMIT"
 ]
 OpticalStandardType = Literal[
     "OPTIC_1000BASE_LX",
     "OPTIC_1000BASE_SX",
     "OPTIC_100GBASE_CWDM4",
@@ -131,14 +144,15 @@
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
@@ -234,14 +248,15 @@
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
@@ -320,26 +335,28 @@
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
@@ -479,14 +496,22 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "get_outpost_instance_types",
+    "list_assets",
+    "list_catalog_items",
+    "list_orders",
+    "list_outposts",
+    "list_sites",
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.py` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
     "ListAssetsInputRequestTypeDef",
@@ -98,14 +99,20 @@
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
     "CreateSiteOutputTypeDef",
@@ -312,14 +319,24 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -749,14 +766,102 @@
         "OperatingAddressStateOrRegion": str,
         "OperatingAddressCity": str,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
+
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.pyi` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetOrderInputRequestTypeDef",
     "GetOutpostInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "GetOutpostInstanceTypesInputRequestTypeDef",
     "InstanceTypeItemTypeDef",
     "GetSiteAddressInputRequestTypeDef",
     "GetSiteInputRequestTypeDef",
     "LineItemAssetInformationTypeDef",
     "ShipmentInformationTypeDef",
     "ListAssetsInputRequestTypeDef",
@@ -97,14 +98,20 @@
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
+    "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    "ListAssetsInputListAssetsPaginateTypeDef",
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
     "CreateSiteOutputTypeDef",
@@ -307,14 +314,24 @@
 GetOutpostInputRequestTypeDef = TypedDict(
     "GetOutpostInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputRequestTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputRequestTypeDef = TypedDict(
@@ -730,14 +747,98 @@
         "OperatingAddressStateOrRegion": str,
         "OperatingAddressCity": str,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "OutpostId": str,
+    },
+)
+_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
+    _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+    _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "OutpostIdentifier": str,
+    },
+)
+_OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListAssetsInputListAssetsPaginateTypeDef",
+    {
+        "HostIdFilter": Sequence[str],
+        "StatusFilter": Sequence[AssetStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssetsInputListAssetsPaginateTypeDef(
+    _RequiredListAssetsInputListAssetsPaginateTypeDef,
+    _OptionalListAssetsInputListAssetsPaginateTypeDef,
+):
+    pass
+
+ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
+    "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
+    {
+        "ItemClassFilter": Sequence[CatalogItemClassType],
+        "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
+        "EC2FamilyFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrdersInputListOrdersPaginateTypeDef = TypedDict(
+    "ListOrdersInputListOrdersPaginateTypeDef",
+    {
+        "OutpostIdentifierFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutpostsInputListOutpostsPaginateTypeDef = TypedDict(
+    "ListOutpostsInputListOutpostsPaginateTypeDef",
+    {
+        "LifeCycleStatusFilter": Sequence[str],
+        "AvailabilityZoneFilter": Sequence[str],
+        "AvailabilityZoneIdFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSitesInputListSitesPaginateTypeDef = TypedDict(
+    "ListSitesInputListSitesPaginateTypeDef",
+    {
+        "OperatingAddressCountryCodeFilter": Sequence[str],
+        "OperatingAddressStateOrRegionFilter": Sequence[str],
+        "OperatingAddressCityFilter": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/PKG-INFO` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +71,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -258,132 +259,82 @@
 
 session = get_session()
 async with session.create_client("outposts") as client:
     client: OutpostsClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`types_aiobotocore_outposts.paginator` module contains type annotations for all
+paginators.
+
+```python
+from aiobotocore.session import get_session
+
+from types_aiobotocore_outposts import OutpostsClient
+from types_aiobotocore_outposts.paginator import (
+    GetOutpostInstanceTypesPaginator,
+    ListAssetsPaginator,
+    ListCatalogItemsPaginator,
+    ListOrdersPaginator,
+    ListOutpostsPaginator,
+    ListSitesPaginator,
+)
+
+session = get_session()
+async with session.create_client("outposts") as client:
+    client: OutpostsClient
+
+    # Explicit type annotations are optional here
+    # Types should be correctly discovered by mypy and IDEs
+    get_outpost_instance_types_paginator: GetOutpostInstanceTypesPaginator = client.get_paginator(
+        "get_outpost_instance_types"
+    )
+    list_assets_paginator: ListAssetsPaginator = client.get_paginator("list_assets")
+    list_catalog_items_paginator: ListCatalogItemsPaginator = client.get_paginator(
+        "list_catalog_items"
+    )
+    list_orders_paginator: ListOrdersPaginator = client.get_paginator("list_orders")
+    list_outposts_paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")
+    list_sites_paginator: ListSitesPaginator = client.get_paginator("list_sites")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/literals/).
+
 ```python
-from types_aiobotocore_outposts.literals import (
-    AddressTypeType,
-    AssetStateType,
-    AssetTypeType,
-    CatalogItemClassType,
-    CatalogItemStatusType,
-    ComputeAssetStateType,
-    FiberOpticCableTypeType,
-    LineItemStatusType,
-    MaximumSupportedWeightLbsType,
-    OpticalStandardType,
-    OrderStatusType,
-    OrderTypeType,
-    PaymentOptionType,
-    PaymentTermType,
-    PowerConnectorType,
-    PowerDrawKvaType,
-    PowerFeedDropType,
-    PowerPhaseType,
-    ShipmentCarrierType,
-    SupportedHardwareTypeType,
-    SupportedStorageEnumType,
-    UplinkCountType,
-    UplinkGbpsType,
-    OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_outposts.literals import AddressTypeType
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/type_defs/).
+
 ```python
-from types_aiobotocore_outposts.type_defs import (
-    AddressTypeDef,
-    AssetLocationTypeDef,
-    ComputeAttributesTypeDef,
-    CancelOrderInputRequestTypeDef,
-    EC2CapacityTypeDef,
-    ConnectionDetailsTypeDef,
-    LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateOutpostInputRequestTypeDef,
-    OutpostTypeDef,
-    RackPhysicalPropertiesTypeDef,
-    DeleteOutpostInputRequestTypeDef,
-    DeleteSiteInputRequestTypeDef,
-    GetCatalogItemInputRequestTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    GetOrderInputRequestTypeDef,
-    GetOutpostInputRequestTypeDef,
-    GetOutpostInstanceTypesInputRequestTypeDef,
-    InstanceTypeItemTypeDef,
-    GetSiteAddressInputRequestTypeDef,
-    GetSiteInputRequestTypeDef,
-    LineItemAssetInformationTypeDef,
-    ShipmentInformationTypeDef,
-    ListAssetsInputRequestTypeDef,
-    ListCatalogItemsInputRequestTypeDef,
-    ListOrdersInputRequestTypeDef,
-    OrderSummaryTypeDef,
-    ListOutpostsInputRequestTypeDef,
-    ListSitesInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartConnectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateOutpostInputRequestTypeDef,
-    UpdateSiteInputRequestTypeDef,
-    UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    UpdateSiteAddressInputRequestTypeDef,
-    AssetInfoTypeDef,
-    CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
-    GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
-    CreateOutpostOutputTypeDef,
-    GetOutpostOutputTypeDef,
-    ListOutpostsOutputTypeDef,
-    UpdateOutpostOutputTypeDef,
-    CreateSiteInputRequestTypeDef,
-    SiteTypeDef,
-    GetOutpostInstanceTypesOutputTypeDef,
-    LineItemTypeDef,
-    ListOrdersOutputTypeDef,
-    ListAssetsOutputTypeDef,
-    GetCatalogItemOutputTypeDef,
-    ListCatalogItemsOutputTypeDef,
-    CreateSiteOutputTypeDef,
-    GetSiteOutputTypeDef,
-    ListSitesOutputTypeDef,
-    UpdateSiteOutputTypeDef,
-    UpdateSiteRackPhysicalPropertiesOutputTypeDef,
-    OrderTypeDef,
-    CreateOrderOutputTypeDef,
-    GetOrderOutputTypeDef,
-)
+from types_aiobotocore_outposts.type_defs import AddressTypeDef
 
 
 def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/SOURCES.txt` & `types-aiobotocore-outposts-2.5.2.post2/types_aiobotocore_outposts.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 types_aiobotocore_outposts/__init__.py
 types_aiobotocore_outposts/__init__.pyi
 types_aiobotocore_outposts/__main__.py
 types_aiobotocore_outposts/client.py
 types_aiobotocore_outposts/client.pyi
 types_aiobotocore_outposts/literals.py
 types_aiobotocore_outposts/literals.pyi
+types_aiobotocore_outposts/paginator.py
+types_aiobotocore_outposts/paginator.pyi
 types_aiobotocore_outposts/py.typed
 types_aiobotocore_outposts/type_defs.py
 types_aiobotocore_outposts/type_defs.pyi
 types_aiobotocore_outposts/version.py
 types_aiobotocore_outposts.egg-info/PKG-INFO
 types_aiobotocore_outposts.egg-info/SOURCES.txt
 types_aiobotocore_outposts.egg-info/dependency_links.txt
```

