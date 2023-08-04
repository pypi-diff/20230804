# Comparing `tmp/types-aiobotocore-lookoutvision-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lookoutvision-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutvision-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutvision-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-lookoutvision-2.5.2.post1.tar` & `types-aiobotocore-lookoutvision-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.969533 types-aiobotocore-lookoutvision-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-08-02 14:52:35.969533 types-aiobotocore-lookoutvision-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.969533 types-aiobotocore-lookoutvision-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 14:42:34.000000 types-aiobotocore-lookoutvision-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.945533 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27394 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.969533 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.296643 types-aiobotocore-lookoutvision-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13725 2023-08-04 13:59:16.276643 types-aiobotocore-lookoutvision-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12180 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.296643 types-aiobotocore-lookoutvision-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2117 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.266643 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1346 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1345 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20429 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20394 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9496 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9494 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5795 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5789 2023-08-04 13:43:30.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26238 2023-08-04 13:43:32.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26197 2023-08-04 13:43:31.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:29.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.266643 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13725 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/LICENSE` & `types-aiobotocore-lookoutvision-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/setup.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutvision",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LookoutforVision 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__init__.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__init__.pyi` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/__main__.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LookoutforVision 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
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

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/client.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModelPackagingConfigurationUnionTypeDef,
+    ModelPackagingConfigurationTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
@@ -328,15 +328,15 @@
         """
 
     async def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: ModelPackagingConfigurationUnionTypeDef,
+        Configuration: ModelPackagingConfigurationTypeDef,
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
```

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/client.pyi` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModelPackagingConfigurationUnionTypeDef,
+    ModelPackagingConfigurationTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
@@ -303,15 +303,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutvision/client/#start_model)
         """
     async def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: ModelPackagingConfigurationUnionTypeDef,
+        Configuration: ModelPackagingConfigurationTypeDef,
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
```

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/literals.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
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
@@ -190,14 +191,15 @@
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
@@ -276,26 +278,28 @@
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

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/literals.pyi` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -188,14 +189,15 @@
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
@@ -274,26 +276,28 @@
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

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/paginator.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/paginator.pyi` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/type_defs.py` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PixelAnomalyTypeDef",
     "BlobTypeDef",
     "DatasetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -83,15 +82,14 @@
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
-    "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelsRequestListModelsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
@@ -99,23 +97,21 @@
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
-    "ModelPackagingConfigurationOutputTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
-    "ModelPackagingConfigurationUnionTypeDef",
     "StartModelPackagingJobRequestRequestTypeDef",
     "DescribeModelPackagingJobResponseTypeDef",
 )
 
 PixelAnomalyTypeDef = TypedDict(
     "PixelAnomalyTypeDef",
     {
@@ -166,21 +162,19 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -209,19 +203,17 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
-
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
-
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -229,21 +221,19 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -251,42 +241,38 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -332,19 +318,17 @@
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -352,19 +336,17 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
-
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
-
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
@@ -393,22 +375,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
-
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -432,21 +412,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -490,21 +468,19 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -512,21 +488,19 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -562,22 +536,20 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 ProjectDescriptionTypeDef = TypedDict(
     "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
@@ -708,41 +680,14 @@
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
-_RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGreengrassConfigurationOutputTypeDef",
-    {
-        "S3OutputLocation": S3LocationTypeDef,
-        "ComponentName": str,
-    },
-)
-_OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGreengrassConfigurationOutputTypeDef",
-    {
-        "CompilerOptions": str,
-        "TargetDevice": Literal["jetson_xavier"],
-        "TargetPlatform": TargetPlatformTypeDef,
-        "ComponentVersion": str,
-        "ComponentDescription": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class GreengrassConfigurationOutputTypeDef(
-    _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredGreengrassConfigurationTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationTypeDef",
     {
         "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
 )
@@ -750,26 +695,24 @@
     "_OptionalGreengrassConfigurationTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
         "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
-
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
@@ -784,44 +727,40 @@
     "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
     _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
     "_RequiredListModelsRequestListModelsPaginateTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
     "_OptionalListModelsRequestListModelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListModelsRequestListModelsPaginateTypeDef(
     _RequiredListModelsRequestListModelsPaginateTypeDef,
     _OptionalListModelsRequestListModelsPaginateTypeDef,
 ):
     pass
 
-
 ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -842,22 +781,20 @@
         "AfterCreationDate": TimestampTypeDef,
         "SourceRefContains": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -871,22 +808,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -956,21 +891,19 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-
 ModelDescriptionTypeDef = TypedDict(
     "ModelDescriptionTypeDef",
     {
         "ModelVersion": str,
         "ModelArn": str,
         "CreationTimestamp": datetime,
         "Description": str,
@@ -984,21 +917,14 @@
         "KmsKeyId": str,
         "MinInferenceUnits": int,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-ModelPackagingConfigurationOutputTypeDef = TypedDict(
-    "ModelPackagingConfigurationOutputTypeDef",
-    {
-        "Greengrass": GreengrassConfigurationOutputTypeDef,
-    },
-)
-
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
 
@@ -1039,50 +965,45 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
-        "ModelPackagingConfiguration": ModelPackagingConfigurationOutputTypeDef,
+        "ModelPackagingConfiguration": ModelPackagingConfigurationTypeDef,
         "ModelPackagingJobDescription": str,
         "ModelPackagingMethod": str,
         "ModelPackagingOutputDetails": ModelPackagingOutputDetailsTypeDef,
         "Status": ModelPackagingJobStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ModelPackagingConfigurationUnionTypeDef = Union[
-    ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
-]
 _RequiredStartModelPackagingJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelPackagingJobRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "Configuration": ModelPackagingConfigurationTypeDef,
     },
@@ -1093,22 +1014,20 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision/type_defs.pyi` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "PixelAnomalyTypeDef",
     "BlobTypeDef",
     "DatasetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -82,15 +83,14 @@
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
-    "GreengrassConfigurationOutputTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelsRequestListModelsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
@@ -98,23 +98,21 @@
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
-    "ModelPackagingConfigurationOutputTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
-    "ModelPackagingConfigurationUnionTypeDef",
     "StartModelPackagingJobRequestRequestTypeDef",
     "DescribeModelPackagingJobResponseTypeDef",
 )
 
 PixelAnomalyTypeDef = TypedDict(
     "PixelAnomalyTypeDef",
     {
@@ -165,19 +163,21 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -206,17 +206,19 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
+
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
+
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -224,19 +226,21 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -244,38 +248,42 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -321,17 +329,19 @@
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -339,17 +349,19 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
+
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
+
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
@@ -378,20 +390,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
+
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -415,19 +429,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -471,19 +487,21 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
+
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -491,19 +509,21 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -539,20 +559,22 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 ProjectDescriptionTypeDef = TypedDict(
     "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
@@ -683,39 +705,14 @@
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
-_RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGreengrassConfigurationOutputTypeDef",
-    {
-        "S3OutputLocation": S3LocationTypeDef,
-        "ComponentName": str,
-    },
-)
-_OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGreengrassConfigurationOutputTypeDef",
-    {
-        "CompilerOptions": str,
-        "TargetDevice": Literal["jetson_xavier"],
-        "TargetPlatform": TargetPlatformTypeDef,
-        "ComponentVersion": str,
-        "ComponentDescription": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class GreengrassConfigurationOutputTypeDef(
-    _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredGreengrassConfigurationTypeDef = TypedDict(
     "_RequiredGreengrassConfigurationTypeDef",
     {
         "S3OutputLocation": S3LocationTypeDef,
         "ComponentName": str,
     },
 )
@@ -723,24 +720,26 @@
     "_OptionalGreengrassConfigurationTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
         "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
+
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
@@ -755,40 +754,44 @@
     "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
     _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
     "_RequiredListModelsRequestListModelsPaginateTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
     "_OptionalListModelsRequestListModelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListModelsRequestListModelsPaginateTypeDef(
     _RequiredListModelsRequestListModelsPaginateTypeDef,
     _OptionalListModelsRequestListModelsPaginateTypeDef,
 ):
     pass
 
+
 ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -809,20 +812,22 @@
         "AfterCreationDate": TimestampTypeDef,
         "SourceRefContains": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -836,20 +841,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -919,19 +926,21 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
+
 ModelDescriptionTypeDef = TypedDict(
     "ModelDescriptionTypeDef",
     {
         "ModelVersion": str,
         "ModelArn": str,
         "CreationTimestamp": datetime,
         "Description": str,
@@ -945,21 +954,14 @@
         "KmsKeyId": str,
         "MinInferenceUnits": int,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-ModelPackagingConfigurationOutputTypeDef = TypedDict(
-    "ModelPackagingConfigurationOutputTypeDef",
-    {
-        "Greengrass": GreengrassConfigurationOutputTypeDef,
-    },
-)
-
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
 
@@ -1000,48 +1002,47 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
-        "ModelPackagingConfiguration": ModelPackagingConfigurationOutputTypeDef,
+        "ModelPackagingConfiguration": ModelPackagingConfigurationTypeDef,
         "ModelPackagingJobDescription": str,
         "ModelPackagingMethod": str,
         "ModelPackagingOutputDetails": ModelPackagingOutputDetailsTypeDef,
         "Status": ModelPackagingJobStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-ModelPackagingConfigurationUnionTypeDef = Union[
-    ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
-]
 _RequiredStartModelPackagingJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelPackagingJobRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "Configuration": ModelPackagingConfigurationTypeDef,
     },
@@ -1052,20 +1053,22 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutvision-2.5.2.post1/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutvision-2.5.2.post2/types_aiobotocore_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

