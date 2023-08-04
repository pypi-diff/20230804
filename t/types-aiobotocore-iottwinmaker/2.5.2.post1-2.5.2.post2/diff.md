# Comparing `tmp/types-aiobotocore-iottwinmaker-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iottwinmaker-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1.tar` & `types-aiobotocore-iottwinmaker-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.805556 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26600 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-08-02 14:41:03.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-08-02 14:41:03.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12449 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10911 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      482 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      481 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26590 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26548 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9664 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9662 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43547 2023-08-04 13:41:23.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43474 2023-08-04 13:41:23.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12449 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/LICENSE` & `types-aiobotocore-iottwinmaker-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/setup.py` & `types-aiobotocore-iottwinmaker-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iottwinmaker",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__main__.py` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.py` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryUnionTypeDef,
+    PropertyValueEntryTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
     TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
@@ -107,15 +107,15 @@
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#exceptions)
         """
 
     async def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#batch_put_property_values)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryUnionTypeDef,
+    PropertyValueEntryTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
     TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
@@ -103,15 +103,15 @@
         """
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#exceptions)
         """
     async def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#batch_put_property_values)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.py` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ColumnTypeType",
     "ComponentUpdateTypeType",
     "ErrorCodeType",
     "GroupTypeType",
     "InterpolationTypeType",
     "OrderByTimeType",
@@ -42,15 +41,14 @@
     "UpdateReasonType",
     "IoTTwinMakerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ColumnTypeType = Literal["EDGE", "NODE", "VALUE"]
 ComponentUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
 ErrorCodeType = Literal[
     "INTERNAL_FAILURE",
     "SYNC_CREATING_ERROR",
     "SYNC_INITIALIZING_ERROR",
     "SYNC_PROCESSING_ERROR",
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
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.py`

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
     "ColumnTypeType",
     "ComponentUpdateTypeType",
     "ErrorCodeType",
     "GroupTypeType",
     "InterpolationTypeType",
     "OrderByTimeType",
@@ -41,14 +42,15 @@
     "UpdateReasonType",
     "IoTTwinMakerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ColumnTypeType = Literal["EDGE", "NODE", "VALUE"]
 ComponentUpdateTypeType = Literal["CREATE", "DELETE", "UPDATE"]
 ErrorCodeType = Literal[
     "INTERNAL_FAILURE",
     "SYNC_CREATING_ERROR",
     "SYNC_INITIALIZING_ERROR",
     "SYNC_PROCESSING_ERROR",
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
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.py` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
     "DeleteEntityRequestRequestTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
-    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
@@ -87,15 +86,14 @@
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
-    "PropertyValueOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "CreateComponentTypeResponseTypeDef",
     "CreateEntityResponseTypeDef",
@@ -110,17 +108,15 @@
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
     "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
-    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
-    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
@@ -129,46 +125,44 @@
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryOutputTypeDef",
-    "PropertyValueHistoryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "PropertyValueEntryTypeDef",
+    "PropertyValueHistoryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
-    "BatchPutPropertyErrorTypeDef",
-    "GetPropertyValueHistoryResponseTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
-    "PropertyValueEntryUnionTypeDef",
-    "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyErrorTypeDef",
     "BatchPutPropertyValuesRequestRequestTypeDef",
+    "GetPropertyValueHistoryResponseTypeDef",
+    "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -399,37 +393,14 @@
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
-    "_RequiredEntityPropertyReferenceOutputTypeDef",
-    {
-        "propertyName": str,
-    },
-)
-_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
-    "_OptionalEntityPropertyReferenceOutputTypeDef",
-    {
-        "componentName": str,
-        "externalIdProperty": Dict[str, str],
-        "entityId": str,
-    },
-    total=False,
-)
-
-
-class EntityPropertyReferenceOutputTypeDef(
-    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
-):
-    pass
-
-
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -496,28 +467,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeOutputTypeDef",
+        "dataType": "DataTypeTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueOutputTypeDef",
+        "defaultValue": "DataValueTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 
@@ -797,36 +768,14 @@
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
 
-_RequiredPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredPropertyValueOutputTypeDef",
-    {
-        "value": "DataValueOutputTypeDef",
-    },
-)
-_OptionalPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalPropertyValueOutputTypeDef",
-    {
-        "timestamp": datetime,
-        "time": str,
-    },
-    total=False,
-)
-
-
-class PropertyValueOutputTypeDef(
-    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
-):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1077,36 +1026,14 @@
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
-_RequiredDataTypeOutputTypeDef = TypedDict(
-    "_RequiredDataTypeOutputTypeDef",
-    {
-        "type": TypeType,
-    },
-)
-_OptionalDataTypeOutputTypeDef = TypedDict(
-    "_OptionalDataTypeOutputTypeDef",
-    {
-        "nestedType": Dict[str, Any],
-        "allowedValues": List["DataValueOutputTypeDef"],
-        "unitOfMeasure": str,
-        "relationship": RelationshipTypeDef,
-    },
-    total=False,
-)
-
-
-class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
-    pass
-
-
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1121,30 +1048,14 @@
 )
 
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
 
-DataValueOutputTypeDef = TypedDict(
-    "DataValueOutputTypeDef",
-    {
-        "booleanValue": bool,
-        "doubleValue": float,
-        "integerValue": int,
-        "longValue": int,
-        "stringValue": str,
-        "listValue": List[Dict[str, Any]],
-        "mapValue": Dict[str, Dict[str, Any]],
-        "relationshipValue": RelationshipValueTypeDef,
-        "expression": str,
-    },
-    total=False,
-)
-
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1156,21 +1067,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceOutputTypeDef,
+        "propertyReference": EntityPropertyReferenceTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueOutputTypeDef",
+        "propertyValue": "DataValueTypeDef",
     },
     total=False,
 )
 
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
@@ -1215,15 +1126,15 @@
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueOutputTypeDef",
+        "value": "DataValueTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1390,56 +1301,14 @@
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryOutputTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
-    },
-)
-_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryOutputTypeDef",
-    {
-        "propertyValues": List[PropertyValueOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class PropertyValueEntryOutputTypeDef(
-    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
-):
-    pass
-
-
-_RequiredPropertyValueHistoryTypeDef = TypedDict(
-    "_RequiredPropertyValueHistoryTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
-    },
-)
-_OptionalPropertyValueHistoryTypeDef = TypedDict(
-    "_OptionalPropertyValueHistoryTypeDef",
-    {
-        "values": List[PropertyValueOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class PropertyValueHistoryTypeDef(
-    _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
-):
-    pass
-
-
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1499,15 +1368,15 @@
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
+        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
@@ -1631,14 +1500,35 @@
 
 class PropertyValueEntryTypeDef(
     _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
 ):
     pass
 
 
+_RequiredPropertyValueHistoryTypeDef = TypedDict(
+    "_RequiredPropertyValueHistoryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueHistoryTypeDef = TypedDict(
+    "_OptionalPropertyValueHistoryTypeDef",
+    {
+        "values": List[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PropertyValueHistoryTypeDef(
+    _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
+):
+    pass
+
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1659,32 +1549,14 @@
 
 class GetPropertyValueRequestRequestTypeDef(
     _RequiredGetPropertyValueRequestRequestTypeDef, _OptionalGetPropertyValueRequestRequestTypeDef
 ):
     pass
 
 
-BatchPutPropertyErrorTypeDef = TypedDict(
-    "BatchPutPropertyErrorTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "entry": PropertyValueEntryOutputTypeDef,
-    },
-)
-
-GetPropertyValueHistoryResponseTypeDef = TypedDict(
-    "GetPropertyValueHistoryResponseTypeDef",
-    {
-        "propertyValues": List[PropertyValueHistoryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1867,27 +1739,44 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
-BatchPutPropertyErrorEntryTypeDef = TypedDict(
-    "BatchPutPropertyErrorEntryTypeDef",
+BatchPutPropertyErrorTypeDef = TypedDict(
+    "BatchPutPropertyErrorTypeDef",
     {
-        "errors": List[BatchPutPropertyErrorTypeDef],
+        "errorCode": str,
+        "errorMessage": str,
+        "entry": PropertyValueEntryTypeDef,
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+        "entries": Sequence[PropertyValueEntryTypeDef],
+    },
+)
+
+GetPropertyValueHistoryResponseTypeDef = TypedDict(
+    "GetPropertyValueHistoryResponseTypeDef",
+    {
+        "propertyValues": List[PropertyValueHistoryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPutPropertyErrorEntryTypeDef = TypedDict(
+    "BatchPutPropertyErrorEntryTypeDef",
+    {
+        "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
     "DeleteEntityRequestRequestTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
-    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
@@ -86,15 +85,14 @@
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
-    "PropertyValueOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "CreateComponentTypeResponseTypeDef",
     "CreateEntityResponseTypeDef",
@@ -109,17 +107,15 @@
     "UpdateComponentTypeResponseTypeDef",
     "UpdateEntityResponseTypeDef",
     "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
-    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
-    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
@@ -128,46 +124,44 @@
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryOutputTypeDef",
-    "PropertyValueHistoryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "PropertyValueEntryTypeDef",
+    "PropertyValueHistoryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
-    "BatchPutPropertyErrorTypeDef",
-    "GetPropertyValueHistoryResponseTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
-    "PropertyValueEntryUnionTypeDef",
-    "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyErrorTypeDef",
     "BatchPutPropertyValuesRequestRequestTypeDef",
+    "GetPropertyValueHistoryResponseTypeDef",
+    "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -388,35 +382,14 @@
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
-    "_RequiredEntityPropertyReferenceOutputTypeDef",
-    {
-        "propertyName": str,
-    },
-)
-_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
-    "_OptionalEntityPropertyReferenceOutputTypeDef",
-    {
-        "componentName": str,
-        "externalIdProperty": Dict[str, str],
-        "entityId": str,
-    },
-    total=False,
-)
-
-class EntityPropertyReferenceOutputTypeDef(
-    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
-):
-    pass
-
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -479,28 +452,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeOutputTypeDef",
+        "dataType": "DataTypeTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueOutputTypeDef",
+        "defaultValue": "DataValueTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 class PropertyDefinitionResponseTypeDef(
@@ -762,34 +735,14 @@
 )
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
-_RequiredPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredPropertyValueOutputTypeDef",
-    {
-        "value": "DataValueOutputTypeDef",
-    },
-)
-_OptionalPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalPropertyValueOutputTypeDef",
-    {
-        "timestamp": datetime,
-        "time": str,
-    },
-    total=False,
-)
-
-class PropertyValueOutputTypeDef(
-    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
-):
-    pass
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1032,34 +985,14 @@
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
-_RequiredDataTypeOutputTypeDef = TypedDict(
-    "_RequiredDataTypeOutputTypeDef",
-    {
-        "type": TypeType,
-    },
-)
-_OptionalDataTypeOutputTypeDef = TypedDict(
-    "_OptionalDataTypeOutputTypeDef",
-    {
-        "nestedType": Dict[str, Any],
-        "allowedValues": List["DataValueOutputTypeDef"],
-        "unitOfMeasure": str,
-        "relationship": RelationshipTypeDef,
-    },
-    total=False,
-)
-
-class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
-    pass
-
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1072,30 +1005,14 @@
     },
     total=False,
 )
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
-DataValueOutputTypeDef = TypedDict(
-    "DataValueOutputTypeDef",
-    {
-        "booleanValue": bool,
-        "doubleValue": float,
-        "integerValue": int,
-        "longValue": int,
-        "stringValue": str,
-        "listValue": List[Dict[str, Any]],
-        "mapValue": Dict[str, Dict[str, Any]],
-        "relationshipValue": RelationshipValueTypeDef,
-        "expression": str,
-    },
-    total=False,
-)
-
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1107,21 +1024,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceOutputTypeDef,
+        "propertyReference": EntityPropertyReferenceTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueOutputTypeDef",
+        "propertyValue": "DataValueTypeDef",
     },
     total=False,
 )
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
 ):
@@ -1164,15 +1081,15 @@
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueOutputTypeDef",
+        "value": "DataValueTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1329,52 +1246,14 @@
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryOutputTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
-    },
-)
-_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryOutputTypeDef",
-    {
-        "propertyValues": List[PropertyValueOutputTypeDef],
-    },
-    total=False,
-)
-
-class PropertyValueEntryOutputTypeDef(
-    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
-):
-    pass
-
-_RequiredPropertyValueHistoryTypeDef = TypedDict(
-    "_RequiredPropertyValueHistoryTypeDef",
-    {
-        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
-    },
-)
-_OptionalPropertyValueHistoryTypeDef = TypedDict(
-    "_OptionalPropertyValueHistoryTypeDef",
-    {
-        "values": List[PropertyValueOutputTypeDef],
-    },
-    total=False,
-)
-
-class PropertyValueHistoryTypeDef(
-    _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
-):
-    pass
-
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1434,15 +1313,15 @@
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
+        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
@@ -1560,14 +1439,33 @@
 )
 
 class PropertyValueEntryTypeDef(
     _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
 ):
     pass
 
+_RequiredPropertyValueHistoryTypeDef = TypedDict(
+    "_RequiredPropertyValueHistoryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueHistoryTypeDef = TypedDict(
+    "_OptionalPropertyValueHistoryTypeDef",
+    {
+        "values": List[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+class PropertyValueHistoryTypeDef(
+    _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
+):
+    pass
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1586,32 +1484,14 @@
 )
 
 class GetPropertyValueRequestRequestTypeDef(
     _RequiredGetPropertyValueRequestRequestTypeDef, _OptionalGetPropertyValueRequestRequestTypeDef
 ):
     pass
 
-BatchPutPropertyErrorTypeDef = TypedDict(
-    "BatchPutPropertyErrorTypeDef",
-    {
-        "errorCode": str,
-        "errorMessage": str,
-        "entry": PropertyValueEntryOutputTypeDef,
-    },
-)
-
-GetPropertyValueHistoryResponseTypeDef = TypedDict(
-    "GetPropertyValueHistoryResponseTypeDef",
-    {
-        "propertyValues": List[PropertyValueHistoryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityName": str,
     },
 )
@@ -1786,27 +1666,44 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
-BatchPutPropertyErrorEntryTypeDef = TypedDict(
-    "BatchPutPropertyErrorEntryTypeDef",
+BatchPutPropertyErrorTypeDef = TypedDict(
+    "BatchPutPropertyErrorTypeDef",
     {
-        "errors": List[BatchPutPropertyErrorTypeDef],
+        "errorCode": str,
+        "errorMessage": str,
+        "entry": PropertyValueEntryTypeDef,
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+        "entries": Sequence[PropertyValueEntryTypeDef],
+    },
+)
+
+GetPropertyValueHistoryResponseTypeDef = TypedDict(
+    "GetPropertyValueHistoryResponseTypeDef",
+    {
+        "propertyValues": List[PropertyValueHistoryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPutPropertyErrorEntryTypeDef = TypedDict(
+    "BatchPutPropertyErrorEntryTypeDef",
+    {
+        "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt` & `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

