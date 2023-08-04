# Comparing `tmp/types-aiobotocore-sagemaker-geospatial-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-geospatial-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-geospatial-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.109469 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-08-02 14:52:57.105469 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.109469 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.101469 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20162 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-02 14:49:00.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-08-02 14:49:00.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39729 2023-08-02 14:49:00.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39681 2023-08-02 14:49:00.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.105469 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.976643 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14272 2023-08-04 13:59:24.976643 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12691 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.976643 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2166 2023-08-04 13:52:27.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.966643 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1408 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1407 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1017 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20183 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20152 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11165 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11163 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5220 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5215 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34476 2023-08-04 13:52:29.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34433 2023-08-04 13:52:29.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:28.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.976643 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14272 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1060 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       39 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-geospatial",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2 service generated"
-        " with mypy-boto3-builder 7.17.1"
+        " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__init__.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__init__.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/__main__.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SageMakergeospatialcapabilities 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
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

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/client.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
     GetEarthObservationJobOutputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     GetTileOutputTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
     InputConfigInputTypeDef,
-    JobConfigInputUnionTypeDef,
+    JobConfigInputTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputConfigInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
@@ -295,15 +295,15 @@
         """
 
     async def start_earth_observation_job(
         self,
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
-        JobConfig: JobConfigInputUnionTypeDef,
+        JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/client.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
     GetEarthObservationJobOutputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     GetTileOutputTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
     InputConfigInputTypeDef,
-    JobConfigInputUnionTypeDef,
+    JobConfigInputTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputConfigInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
@@ -274,15 +274,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/client/#search_raster_data_collection)
         """
     async def start_earth_observation_job(
         self,
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
-        JobConfig: JobConfigInputUnionTypeDef,
+        JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/literals.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
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
@@ -245,14 +246,15 @@
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
@@ -331,26 +333,28 @@
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

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/literals.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
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
@@ -243,14 +244,15 @@
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
@@ -329,26 +331,28 @@
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

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/paginator.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/paginator.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/type_defs.py` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sagemaker-geospatial service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
+    from types_aiobotocore_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
 
-    data: MultiPolygonGeometryInputOutputTypeDef = ...
+    data: MultiPolygonGeometryInputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -47,44 +47,38 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "MultiPolygonGeometryInputOutputTypeDef",
-    "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
-    "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
     "EoCloudCoverInputTypeDef",
     "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
     "ExportS3DataInputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
-    "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
-    "TemporalStatisticsConfigInputOutputTypeDef",
-    "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
     "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
@@ -100,17 +94,15 @@
     "TimeRangeFilterOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
-    "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
     "OutputConfigInputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
@@ -123,101 +115,70 @@
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "TimeRangeFilterInputTypeDef",
-    "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
-    "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
     "ExportVectorEnrichmentJobOutputTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
-    "ResamplingConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
-    "StackConfigInputOutputTypeDef",
     "StackConfigInputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
-    "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
-    "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
-    "JobConfigInputUnionTypeDef",
-    "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
+    "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
-    "InputConfigOutputTypeDef",
     "InputConfigInputTypeDef",
+    "InputConfigOutputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
+    "StartEarthObservationJobInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
     "StartEarthObservationJobOutputTypeDef",
-    "StartEarthObservationJobInputRequestTypeDef",
-)
-
-MultiPolygonGeometryInputOutputTypeDef = TypedDict(
-    "MultiPolygonGeometryInputOutputTypeDef",
-    {
-        "Coordinates": List[List[List[List[float]]]],
-    },
-)
-
-PolygonGeometryInputOutputTypeDef = TypedDict(
-    "PolygonGeometryInputOutputTypeDef",
-    {
-        "Coordinates": List[List[List[float]]],
-    },
 )
 
 MultiPolygonGeometryInputTypeDef = TypedDict(
     "MultiPolygonGeometryInputTypeDef",
     {
-        "Coordinates": Sequence[Sequence[Sequence[Sequence[float]]]],
+        "Coordinates": List[List[List[List[float]]]],
     },
 )
 
 PolygonGeometryInputTypeDef = TypedDict(
     "PolygonGeometryInputTypeDef",
     {
-        "Coordinates": Sequence[Sequence[Sequence[float]]],
+        "Coordinates": List[List[List[float]]],
     },
 )
 
 AssetValueTypeDef = TypedDict(
     "AssetValueTypeDef",
     {
         "Href": str,
     },
     total=False,
 )
 
-CloudRemovalConfigInputOutputTypeDef = TypedDict(
-    "CloudRemovalConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": Literal["INTERPOLATION"],
-        "InterpolationValue": str,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 CloudRemovalConfigInputTypeDef = TypedDict(
     "CloudRemovalConfigInputTypeDef",
     {
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
@@ -348,28 +309,19 @@
 )
 
 
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
 
-GeoMosaicConfigInputOutputTypeDef = TypedDict(
-    "GeoMosaicConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 GeoMosaicConfigInputTypeDef = TypedDict(
     "GeoMosaicConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
@@ -465,94 +417,47 @@
         "ViewOffNadir": float,
         "ViewSunAzimuth": float,
         "ViewSunElevation": float,
     },
     total=False,
 )
 
-_RequiredTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_RequiredTemporalStatisticsConfigInputOutputTypeDef",
-    {
-        "Statistics": List[TemporalStatisticsType],
-    },
-)
-_OptionalTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_OptionalTemporalStatisticsConfigInputOutputTypeDef",
-    {
-        "GroupBy": GroupByType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
-
-class TemporalStatisticsConfigInputOutputTypeDef(
-    _RequiredTemporalStatisticsConfigInputOutputTypeDef,
-    _OptionalTemporalStatisticsConfigInputOutputTypeDef,
-):
-    pass
-
-
-_RequiredZonalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_RequiredZonalStatisticsConfigInputOutputTypeDef",
-    {
-        "Statistics": List[ZonalStatisticsType],
-        "ZoneS3Path": str,
-    },
-)
-_OptionalZonalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_OptionalZonalStatisticsConfigInputOutputTypeDef",
-    {
-        "TargetBands": List[str],
-        "ZoneS3PathKmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class ZonalStatisticsConfigInputOutputTypeDef(
-    _RequiredZonalStatisticsConfigInputOutputTypeDef,
-    _OptionalZonalStatisticsConfigInputOutputTypeDef,
-):
-    pass
-
-
 _RequiredTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredTemporalStatisticsConfigInputTypeDef",
     {
-        "Statistics": Sequence[TemporalStatisticsType],
+        "Statistics": List[TemporalStatisticsType],
     },
 )
 _OptionalTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalTemporalStatisticsConfigInputTypeDef",
     {
         "GroupBy": GroupByType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 
 class TemporalStatisticsConfigInputTypeDef(
     _RequiredTemporalStatisticsConfigInputTypeDef, _OptionalTemporalStatisticsConfigInputTypeDef
 ):
     pass
 
 
 _RequiredZonalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredZonalStatisticsConfigInputTypeDef",
     {
-        "Statistics": Sequence[ZonalStatisticsType],
+        "Statistics": List[ZonalStatisticsType],
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
         "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
 
 class ZonalStatisticsConfigInputTypeDef(
@@ -777,44 +682,27 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AreaOfInterestGeometryOutputTypeDef = TypedDict(
-    "AreaOfInterestGeometryOutputTypeDef",
-    {
-        "MultiPolygonGeometry": MultiPolygonGeometryInputOutputTypeDef,
-        "PolygonGeometry": PolygonGeometryInputOutputTypeDef,
-    },
-    total=False,
-)
-
 AreaOfInterestGeometryTypeDef = TypedDict(
     "AreaOfInterestGeometryTypeDef",
     {
         "MultiPolygonGeometry": MultiPolygonGeometryInputTypeDef,
         "PolygonGeometry": PolygonGeometryInputTypeDef,
     },
     total=False,
 )
 
-CustomIndicesInputOutputTypeDef = TypedDict(
-    "CustomIndicesInputOutputTypeDef",
-    {
-        "Operations": List[OperationTypeDef],
-    },
-    total=False,
-)
-
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
-        "Operations": Sequence[OperationTypeDef],
+        "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
 GetTileOutputTypeDef = TypedDict(
     "GetTileOutputTypeDef",
     {
@@ -1015,44 +903,27 @@
     "TimeRangeFilterInputTypeDef",
     {
         "EndTime": TimestampTypeDef,
         "StartTime": TimestampTypeDef,
     },
 )
 
-AreaOfInterestOutputTypeDef = TypedDict(
-    "AreaOfInterestOutputTypeDef",
-    {
-        "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
-    },
-    total=False,
-)
-
 AreaOfInterestTypeDef = TypedDict(
     "AreaOfInterestTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryTypeDef,
     },
     total=False,
 )
 
-BandMathConfigInputOutputTypeDef = TypedDict(
-    "BandMathConfigInputOutputTypeDef",
-    {
-        "CustomIndices": CustomIndicesInputOutputTypeDef,
-        "PredefinedIndices": List[str],
-    },
-    total=False,
-)
-
 BandMathConfigInputTypeDef = TypedDict(
     "BandMathConfigInputTypeDef",
     {
         "CustomIndices": CustomIndicesInputTypeDef,
-        "PredefinedIndices": Sequence[str],
+        "PredefinedIndices": List[str],
     },
     total=False,
 )
 
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
@@ -1150,72 +1021,41 @@
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResamplingConfigInputOutputTypeDef = TypedDict(
-    "_RequiredResamplingConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionResamplingInputTypeDef,
-    },
-)
-_OptionalResamplingConfigInputOutputTypeDef = TypedDict(
-    "_OptionalResamplingConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
-
-class ResamplingConfigInputOutputTypeDef(
-    _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
-):
-    pass
-
-
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
 
-StackConfigInputOutputTypeDef = TypedDict(
-    "StackConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 StackConfigInputTypeDef = TypedDict(
     "StackConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
@@ -1285,108 +1125,82 @@
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobConfigInputOutputTypeDef = TypedDict(
-    "JobConfigInputOutputTypeDef",
-    {
-        "BandMathConfig": BandMathConfigInputOutputTypeDef,
-        "CloudMaskingConfig": Dict[str, Any],
-        "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
-        "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
-        "LandCoverSegmentationConfig": Dict[str, Any],
-        "ResamplingConfig": ResamplingConfigInputOutputTypeDef,
-        "StackConfig": StackConfigInputOutputTypeDef,
-        "TemporalStatisticsConfig": TemporalStatisticsConfigInputOutputTypeDef,
-        "ZonalStatisticsConfig": ZonalStatisticsConfigInputOutputTypeDef,
-    },
-    total=False,
-)
-
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
-        "CloudMaskingConfig": Mapping[str, Any],
+        "CloudMaskingConfig": Dict[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputTypeDef,
-        "LandCoverSegmentationConfig": Mapping[str, Any],
+        "LandCoverSegmentationConfig": Dict[str, Any],
         "ResamplingConfig": ResamplingConfigInputTypeDef,
         "StackConfig": StackConfigInputTypeDef,
         "TemporalStatisticsConfig": TemporalStatisticsConfigInputTypeDef,
         "ZonalStatisticsConfig": ZonalStatisticsConfigInputTypeDef,
     },
     total=False,
 )
 
-PropertyFiltersOutputTypeDef = TypedDict(
-    "PropertyFiltersOutputTypeDef",
-    {
-        "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterTypeDef],
-    },
-    total=False,
-)
-
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": Sequence[PropertyFilterTypeDef],
+        "Properties": List[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-JobConfigInputUnionTypeDef = Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef]
-_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryOutputTypeDef",
+_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryInputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryOutputTypeDef",
+_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryInputTypeDef",
     {
-        "AreaOfInterest": AreaOfInterestOutputTypeDef,
-        "PropertyFilters": PropertyFiltersOutputTypeDef,
+        "AreaOfInterest": AreaOfInterestTypeDef,
+        "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
 
-class RasterDataCollectionQueryOutputTypeDef(
-    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
+class RasterDataCollectionQueryInputTypeDef(
+    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
 ):
     pass
 
 
-_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryInputTypeDef",
+_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "RasterDataCollectionName": str,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryInputTypeDef",
+_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
 
-class RasterDataCollectionQueryInputTypeDef(
-    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
+class RasterDataCollectionQueryOutputTypeDef(
+    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
 ):
     pass
 
 
 _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef",
     {
@@ -1407,28 +1221,28 @@
 class RasterDataCollectionQueryWithBandFilterInputTypeDef(
     _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef,
     _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef,
 ):
     pass
 
 
-InputConfigOutputTypeDef = TypedDict(
-    "InputConfigOutputTypeDef",
+InputConfigInputTypeDef = TypedDict(
+    "InputConfigInputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
-InputConfigInputTypeDef = TypedDict(
-    "InputConfigInputTypeDef",
+InputConfigOutputTypeDef = TypedDict(
+    "InputConfigOutputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
     "_RequiredSearchRasterDataCollectionInputRequestTypeDef",
     {
@@ -1448,26 +1262,53 @@
 class SearchRasterDataCollectionInputRequestTypeDef(
     _RequiredSearchRasterDataCollectionInputRequestTypeDef,
     _OptionalSearchRasterDataCollectionInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_RequiredStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+        "InputConfig": InputConfigInputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
+        "Name": str,
+    },
+)
+_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_OptionalStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartEarthObservationJobInputRequestTypeDef(
+    _RequiredStartEarthObservationJobInputRequestTypeDef,
+    _OptionalStartEarthObservationJobInputRequestTypeDef,
+):
+    pass
+
+
 GetEarthObservationJobOutputTypeDef = TypedDict(
     "GetEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": EarthObservationJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": ExportErrorDetailsTypeDef,
         "ExportStatus": EarthObservationJobExportStatusType,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputOutputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1477,41 +1318,15 @@
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputOutputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_RequiredStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-        "InputConfig": InputConfigInputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
-        "Name": str,
-    },
-)
-_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_OptionalStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartEarthObservationJobInputRequestTypeDef(
-    _RequiredStartEarthObservationJobInputRequestTypeDef,
-    _OptionalStartEarthObservationJobInputRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial/type_defs.pyi` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sagemaker-geospatial service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
+    from types_aiobotocore_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
 
-    data: MultiPolygonGeometryInputOutputTypeDef = ...
+    data: MultiPolygonGeometryInputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -46,44 +46,38 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "MultiPolygonGeometryInputOutputTypeDef",
-    "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
-    "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
     "EoCloudCoverInputTypeDef",
     "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
     "ExportS3DataInputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
-    "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
-    "TemporalStatisticsConfigInputOutputTypeDef",
-    "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
     "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
@@ -99,17 +93,15 @@
     "TimeRangeFilterOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
-    "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
     "OutputConfigInputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
@@ -122,101 +114,70 @@
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "TimeRangeFilterInputTypeDef",
-    "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
-    "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
     "ExportVectorEnrichmentJobOutputTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
-    "ResamplingConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
-    "StackConfigInputOutputTypeDef",
     "StackConfigInputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
-    "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
-    "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
-    "JobConfigInputUnionTypeDef",
-    "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
+    "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
-    "InputConfigOutputTypeDef",
     "InputConfigInputTypeDef",
+    "InputConfigOutputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
+    "StartEarthObservationJobInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
     "StartEarthObservationJobOutputTypeDef",
-    "StartEarthObservationJobInputRequestTypeDef",
-)
-
-MultiPolygonGeometryInputOutputTypeDef = TypedDict(
-    "MultiPolygonGeometryInputOutputTypeDef",
-    {
-        "Coordinates": List[List[List[List[float]]]],
-    },
-)
-
-PolygonGeometryInputOutputTypeDef = TypedDict(
-    "PolygonGeometryInputOutputTypeDef",
-    {
-        "Coordinates": List[List[List[float]]],
-    },
 )
 
 MultiPolygonGeometryInputTypeDef = TypedDict(
     "MultiPolygonGeometryInputTypeDef",
     {
-        "Coordinates": Sequence[Sequence[Sequence[Sequence[float]]]],
+        "Coordinates": List[List[List[List[float]]]],
     },
 )
 
 PolygonGeometryInputTypeDef = TypedDict(
     "PolygonGeometryInputTypeDef",
     {
-        "Coordinates": Sequence[Sequence[Sequence[float]]],
+        "Coordinates": List[List[List[float]]],
     },
 )
 
 AssetValueTypeDef = TypedDict(
     "AssetValueTypeDef",
     {
         "Href": str,
     },
     total=False,
 )
 
-CloudRemovalConfigInputOutputTypeDef = TypedDict(
-    "CloudRemovalConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": Literal["INTERPOLATION"],
-        "InterpolationValue": str,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 CloudRemovalConfigInputTypeDef = TypedDict(
     "CloudRemovalConfigInputTypeDef",
     {
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
@@ -339,28 +300,19 @@
     },
     total=False,
 )
 
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
-GeoMosaicConfigInputOutputTypeDef = TypedDict(
-    "GeoMosaicConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 GeoMosaicConfigInputTypeDef = TypedDict(
     "GeoMosaicConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
@@ -454,88 +406,45 @@
         "ViewOffNadir": float,
         "ViewSunAzimuth": float,
         "ViewSunElevation": float,
     },
     total=False,
 )
 
-_RequiredTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_RequiredTemporalStatisticsConfigInputOutputTypeDef",
-    {
-        "Statistics": List[TemporalStatisticsType],
-    },
-)
-_OptionalTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_OptionalTemporalStatisticsConfigInputOutputTypeDef",
-    {
-        "GroupBy": GroupByType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
-class TemporalStatisticsConfigInputOutputTypeDef(
-    _RequiredTemporalStatisticsConfigInputOutputTypeDef,
-    _OptionalTemporalStatisticsConfigInputOutputTypeDef,
-):
-    pass
-
-_RequiredZonalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_RequiredZonalStatisticsConfigInputOutputTypeDef",
-    {
-        "Statistics": List[ZonalStatisticsType],
-        "ZoneS3Path": str,
-    },
-)
-_OptionalZonalStatisticsConfigInputOutputTypeDef = TypedDict(
-    "_OptionalZonalStatisticsConfigInputOutputTypeDef",
-    {
-        "TargetBands": List[str],
-        "ZoneS3PathKmsKeyId": str,
-    },
-    total=False,
-)
-
-class ZonalStatisticsConfigInputOutputTypeDef(
-    _RequiredZonalStatisticsConfigInputOutputTypeDef,
-    _OptionalZonalStatisticsConfigInputOutputTypeDef,
-):
-    pass
-
 _RequiredTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredTemporalStatisticsConfigInputTypeDef",
     {
-        "Statistics": Sequence[TemporalStatisticsType],
+        "Statistics": List[TemporalStatisticsType],
     },
 )
 _OptionalTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalTemporalStatisticsConfigInputTypeDef",
     {
         "GroupBy": GroupByType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 class TemporalStatisticsConfigInputTypeDef(
     _RequiredTemporalStatisticsConfigInputTypeDef, _OptionalTemporalStatisticsConfigInputTypeDef
 ):
     pass
 
 _RequiredZonalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredZonalStatisticsConfigInputTypeDef",
     {
-        "Statistics": Sequence[ZonalStatisticsType],
+        "Statistics": List[ZonalStatisticsType],
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
         "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
@@ -752,44 +661,27 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AreaOfInterestGeometryOutputTypeDef = TypedDict(
-    "AreaOfInterestGeometryOutputTypeDef",
-    {
-        "MultiPolygonGeometry": MultiPolygonGeometryInputOutputTypeDef,
-        "PolygonGeometry": PolygonGeometryInputOutputTypeDef,
-    },
-    total=False,
-)
-
 AreaOfInterestGeometryTypeDef = TypedDict(
     "AreaOfInterestGeometryTypeDef",
     {
         "MultiPolygonGeometry": MultiPolygonGeometryInputTypeDef,
         "PolygonGeometry": PolygonGeometryInputTypeDef,
     },
     total=False,
 )
 
-CustomIndicesInputOutputTypeDef = TypedDict(
-    "CustomIndicesInputOutputTypeDef",
-    {
-        "Operations": List[OperationTypeDef],
-    },
-    total=False,
-)
-
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
-        "Operations": Sequence[OperationTypeDef],
+        "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
 GetTileOutputTypeDef = TypedDict(
     "GetTileOutputTypeDef",
     {
@@ -986,44 +878,27 @@
     "TimeRangeFilterInputTypeDef",
     {
         "EndTime": TimestampTypeDef,
         "StartTime": TimestampTypeDef,
     },
 )
 
-AreaOfInterestOutputTypeDef = TypedDict(
-    "AreaOfInterestOutputTypeDef",
-    {
-        "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
-    },
-    total=False,
-)
-
 AreaOfInterestTypeDef = TypedDict(
     "AreaOfInterestTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryTypeDef,
     },
     total=False,
 )
 
-BandMathConfigInputOutputTypeDef = TypedDict(
-    "BandMathConfigInputOutputTypeDef",
-    {
-        "CustomIndices": CustomIndicesInputOutputTypeDef,
-        "PredefinedIndices": List[str],
-    },
-    total=False,
-)
-
 BandMathConfigInputTypeDef = TypedDict(
     "BandMathConfigInputTypeDef",
     {
         "CustomIndices": CustomIndicesInputTypeDef,
-        "PredefinedIndices": Sequence[str],
+        "PredefinedIndices": List[str],
     },
     total=False,
 )
 
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
@@ -1117,68 +992,39 @@
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResamplingConfigInputOutputTypeDef = TypedDict(
-    "_RequiredResamplingConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionResamplingInputTypeDef,
-    },
-)
-_OptionalResamplingConfigInputOutputTypeDef = TypedDict(
-    "_OptionalResamplingConfigInputOutputTypeDef",
-    {
-        "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
-class ResamplingConfigInputOutputTypeDef(
-    _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
-):
-    pass
-
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
-StackConfigInputOutputTypeDef = TypedDict(
-    "StackConfigInputOutputTypeDef",
-    {
-        "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": List[str],
-    },
-    total=False,
-)
-
 StackConfigInputTypeDef = TypedDict(
     "StackConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": Sequence[str],
+        "TargetBands": List[str],
     },
     total=False,
 )
 
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
@@ -1246,105 +1092,79 @@
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobConfigInputOutputTypeDef = TypedDict(
-    "JobConfigInputOutputTypeDef",
-    {
-        "BandMathConfig": BandMathConfigInputOutputTypeDef,
-        "CloudMaskingConfig": Dict[str, Any],
-        "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
-        "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
-        "LandCoverSegmentationConfig": Dict[str, Any],
-        "ResamplingConfig": ResamplingConfigInputOutputTypeDef,
-        "StackConfig": StackConfigInputOutputTypeDef,
-        "TemporalStatisticsConfig": TemporalStatisticsConfigInputOutputTypeDef,
-        "ZonalStatisticsConfig": ZonalStatisticsConfigInputOutputTypeDef,
-    },
-    total=False,
-)
-
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
-        "CloudMaskingConfig": Mapping[str, Any],
+        "CloudMaskingConfig": Dict[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputTypeDef,
-        "LandCoverSegmentationConfig": Mapping[str, Any],
+        "LandCoverSegmentationConfig": Dict[str, Any],
         "ResamplingConfig": ResamplingConfigInputTypeDef,
         "StackConfig": StackConfigInputTypeDef,
         "TemporalStatisticsConfig": TemporalStatisticsConfigInputTypeDef,
         "ZonalStatisticsConfig": ZonalStatisticsConfigInputTypeDef,
     },
     total=False,
 )
 
-PropertyFiltersOutputTypeDef = TypedDict(
-    "PropertyFiltersOutputTypeDef",
-    {
-        "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterTypeDef],
-    },
-    total=False,
-)
-
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": Sequence[PropertyFilterTypeDef],
+        "Properties": List[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-JobConfigInputUnionTypeDef = Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef]
-_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryOutputTypeDef",
+_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryInputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryOutputTypeDef",
+_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryInputTypeDef",
     {
-        "AreaOfInterest": AreaOfInterestOutputTypeDef,
-        "PropertyFilters": PropertyFiltersOutputTypeDef,
+        "AreaOfInterest": AreaOfInterestTypeDef,
+        "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
-class RasterDataCollectionQueryOutputTypeDef(
-    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
+class RasterDataCollectionQueryInputTypeDef(
+    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
 ):
     pass
 
-_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryInputTypeDef",
+_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "RasterDataCollectionName": str,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryInputTypeDef",
+_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
-class RasterDataCollectionQueryInputTypeDef(
-    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
+class RasterDataCollectionQueryOutputTypeDef(
+    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
 ):
     pass
 
 _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef",
     {
         "TimeRangeFilter": TimeRangeFilterInputTypeDef,
@@ -1362,28 +1182,28 @@
 
 class RasterDataCollectionQueryWithBandFilterInputTypeDef(
     _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef,
     _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef,
 ):
     pass
 
-InputConfigOutputTypeDef = TypedDict(
-    "InputConfigOutputTypeDef",
+InputConfigInputTypeDef = TypedDict(
+    "InputConfigInputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
-InputConfigInputTypeDef = TypedDict(
-    "InputConfigInputTypeDef",
+InputConfigOutputTypeDef = TypedDict(
+    "InputConfigOutputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
     "_RequiredSearchRasterDataCollectionInputRequestTypeDef",
     {
@@ -1401,26 +1221,51 @@
 
 class SearchRasterDataCollectionInputRequestTypeDef(
     _RequiredSearchRasterDataCollectionInputRequestTypeDef,
     _OptionalSearchRasterDataCollectionInputRequestTypeDef,
 ):
     pass
 
+_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_RequiredStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+        "InputConfig": InputConfigInputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
+        "Name": str,
+    },
+)
+_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_OptionalStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartEarthObservationJobInputRequestTypeDef(
+    _RequiredStartEarthObservationJobInputRequestTypeDef,
+    _OptionalStartEarthObservationJobInputRequestTypeDef,
+):
+    pass
+
 GetEarthObservationJobOutputTypeDef = TypedDict(
     "GetEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": EarthObservationJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": ExportErrorDetailsTypeDef,
         "ExportStatus": EarthObservationJobExportStatusType,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputOutputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1430,40 +1275,15 @@
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputOutputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_RequiredStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-        "InputConfig": InputConfigInputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
-        "Name": str,
-    },
-)
-_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_OptionalStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartEarthObservationJobInputRequestTypeDef(
-    _RequiredStartEarthObservationJobInputRequestTypeDef,
-    _OptionalStartEarthObservationJobInputRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-sagemaker-geospatial-2.5.2.post1/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-geospatial-2.5.2.post2/types_aiobotocore_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

