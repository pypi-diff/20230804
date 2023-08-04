# Comparing `tmp/types-aiobotocore-iotfleetwise-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotfleetwise-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1.tar` & `types-aiobotocore-iotfleetwise-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.741562 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43360 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60490 2023-08-02 14:40:51.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60384 2023-08-02 14:40:51.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15159 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13621 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:41:05.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3445 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3444 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43340 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43268 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11527 2023-08-04 13:41:07.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11525 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16193 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16178 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58195 2023-08-04 13:41:08.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58094 2023-08-04 13:41:08.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15159 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/LICENSE` & `types-aiobotocore-iotfleetwise-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/setup.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleetwise",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__main__.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetWise 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTFleetWise 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeUnionTypeDef,
+    NodeTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
@@ -276,15 +276,15 @@
         """
 
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeUnionTypeDef] = ...,
+        nodes: Sequence[NodeTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -713,16 +713,16 @@
         """
 
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
+        nodesToAdd: Sequence[NodeTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeUnionTypeDef,
+    NodeTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
@@ -262,15 +262,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_model_manifest)
         """
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeUnionTypeDef] = ...,
+        nodes: Sequence[NodeTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -657,16 +657,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_model_manifest)
         """
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
+        nodesToAdd: Sequence[NodeTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.pyi`

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
     "CampaignStatusType",
     "CompressionType",
     "DataFormatType",
     "DiagnosticsModeType",
     "GetVehicleStatusPaginatorName",
     "ListCampaignsPaginatorName",
@@ -53,15 +52,14 @@
     "IoTFleetWiseServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CampaignStatusType = Literal["CREATING", "RUNNING", "SUSPENDED", "WAITING_FOR_APPROVAL"]
 CompressionType = Literal["OFF", "SNAPPY"]
 DataFormatType = Literal["JSON", "PARQUET"]
 DiagnosticsModeType = Literal["OFF", "SEND_ACTIVE_DTCS"]
 GetVehicleStatusPaginatorName = Literal["get_vehicle_status"]
 ListCampaignsPaginatorName = Literal["list_campaigns"]
 ListDecoderManifestNetworkInterfacesPaginatorName = Literal[
@@ -132,14 +130,15 @@
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
@@ -235,14 +234,15 @@
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
@@ -321,26 +321,28 @@
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.py`

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
     "CampaignStatusType",
     "CompressionType",
     "DataFormatType",
     "DiagnosticsModeType",
     "GetVehicleStatusPaginatorName",
     "ListCampaignsPaginatorName",
@@ -52,14 +53,15 @@
     "IoTFleetWiseServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CampaignStatusType = Literal["CREATING", "RUNNING", "SUSPENDED", "WAITING_FOR_APPROVAL"]
 CompressionType = Literal["OFF", "SNAPPY"]
 DataFormatType = Literal["JSON", "PARQUET"]
 DiagnosticsModeType = Literal["OFF", "SEND_ACTIVE_DTCS"]
 GetVehicleStatusPaginatorName = Literal["get_vehicle_status"]
 ListCampaignsPaginatorName = Literal["list_campaigns"]
 ListDecoderManifestNetworkInterfacesPaginatorName = Literal[
@@ -130,14 +132,15 @@
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
@@ -233,14 +236,15 @@
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
@@ -319,26 +323,28 @@
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.py` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotfleetwise.type_defs import ActuatorOutputTypeDef
+    from types_aiobotocore_iotfleetwise.type_defs import ActuatorTypeDef
 
-    data: ActuatorOutputTypeDef = ...
+    data: ActuatorTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -40,18 +40,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
@@ -104,15 +102,14 @@
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
     "ObdInterfaceTypeDef",
-    "SensorOutputTypeDef",
     "SensorTypeDef",
     "ObdSignalTypeDef",
     "TimestreamResourcesTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "UpdateModelManifestRequestRequestTypeDef",
@@ -177,62 +174,33 @@
     "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
-    "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "NodeUnionTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
-)
-
-_RequiredActuatorOutputTypeDef = TypedDict(
-    "_RequiredActuatorOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalActuatorOutputTypeDef = TypedDict(
-    "_OptionalActuatorOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "assignedValue": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
 )
 
-
-class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
-    pass
-
-
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -260,42 +228,14 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "assignedValue": str,
-        "defaultValue": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
-
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1126,40 +1066,14 @@
 )
 
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
 
-_RequiredSensorOutputTypeDef = TypedDict(
-    "_RequiredSensorOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalSensorOutputTypeDef = TypedDict(
-    "_OptionalSensorOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-
-class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
-    pass
-
-
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -2100,25 +2014,14 @@
 )
 
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
 
-NodeOutputTypeDef = TypedDict(
-    "NodeOutputTypeDef",
-    {
-        "branch": BranchTypeDef,
-        "sensor": SensorOutputTypeDef,
-        "actuator": ActuatorOutputTypeDef,
-        "attribute": AttributeOutputTypeDef,
-    },
-    total=False,
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
@@ -2250,33 +2153,81 @@
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
-        "nodes": List[NodeOutputTypeDef],
+        "nodes": List[NodeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
-        "nodes": List[NodeOutputTypeDef],
+        "nodes": List[NodeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeTypeDef],
+        "nodesToUpdate": Sequence[NodeTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2340,55 +2291,7 @@
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
     "ImportDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
     },
 )
-
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[NodeUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[NodeUnionTypeDef],
-        "nodesToUpdate": Sequence[NodeUnionTypeDef],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotfleetwise.type_defs import ActuatorOutputTypeDef
+    from types_aiobotocore_iotfleetwise.type_defs import ActuatorTypeDef
 
-    data: ActuatorOutputTypeDef = ...
+    data: ActuatorTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,18 +39,16 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
-    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
     "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
@@ -103,15 +101,14 @@
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
     "ObdInterfaceTypeDef",
-    "SensorOutputTypeDef",
     "SensorTypeDef",
     "ObdSignalTypeDef",
     "TimestreamResourcesTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "UpdateModelManifestRequestRequestTypeDef",
@@ -176,60 +173,33 @@
     "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
-    "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
     "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "NodeUnionTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
     "ImportDecoderManifestRequestRequestTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
-)
-
-_RequiredActuatorOutputTypeDef = TypedDict(
-    "_RequiredActuatorOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalActuatorOutputTypeDef = TypedDict(
-    "_OptionalActuatorOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "assignedValue": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
 )
 
-class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
-    pass
-
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -255,40 +225,14 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
-_RequiredAttributeOutputTypeDef = TypedDict(
-    "_RequiredAttributeOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalAttributeOutputTypeDef = TypedDict(
-    "_OptionalAttributeOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "assignedValue": str,
-        "defaultValue": str,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
-    pass
-
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1073,38 +1017,14 @@
     },
     total=False,
 )
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
-_RequiredSensorOutputTypeDef = TypedDict(
-    "_RequiredSensorOutputTypeDef",
-    {
-        "fullyQualifiedName": str,
-        "dataType": NodeDataTypeType,
-    },
-)
-_OptionalSensorOutputTypeDef = TypedDict(
-    "_OptionalSensorOutputTypeDef",
-    {
-        "description": str,
-        "unit": str,
-        "allowedValues": List[str],
-        "min": float,
-        "max": float,
-        "deprecationMessage": str,
-        "comment": str,
-    },
-    total=False,
-)
-
-class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
-    pass
-
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -2005,25 +1925,14 @@
     },
     total=False,
 )
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
-NodeOutputTypeDef = TypedDict(
-    "NodeOutputTypeDef",
-    {
-        "branch": BranchTypeDef,
-        "sensor": SensorOutputTypeDef,
-        "actuator": ActuatorOutputTypeDef,
-        "attribute": AttributeOutputTypeDef,
-    },
-    total=False,
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
@@ -2151,33 +2060,77 @@
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
-        "nodes": List[NodeOutputTypeDef],
+        "nodes": List[NodeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
-        "nodes": List[NodeOutputTypeDef],
+        "nodes": List[NodeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeTypeDef],
+        "nodesToUpdate": Sequence[NodeTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2237,52 +2190,7 @@
 ImportDecoderManifestRequestRequestTypeDef = TypedDict(
     "ImportDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
     },
 )
-
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[NodeUnionTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[NodeUnionTypeDef],
-        "nodesToUpdate": Sequence[NodeUnionTypeDef],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

