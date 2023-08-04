# Comparing `tmp/types-aiobotocore-iotsitewise-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotsitewise-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsitewise-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsitewise-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-iotsitewise-2.5.2.post1.tar` & `types-aiobotocore-iotsitewise-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.369557 types-aiobotocore-iotsitewise-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-08-02 14:52:28.369557 types-aiobotocore-iotsitewise-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27789 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.369557 types-aiobotocore-iotsitewise-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.361557 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65837 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    65732 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-08-02 14:40:56.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-08-02 14:40:56.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22753 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22733 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   109333 2023-08-02 14:40:58.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   109125 2023-08-02 14:40:57.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-02 14:40:56.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-02 14:40:55.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.369557 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:28.000000 types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16974 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15440 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5322 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5321 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    65807 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    65702 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15491 2023-08-04 13:41:14.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15489 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22753 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22733 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   105809 2023-08-04 13:41:17.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   105608 2023-08-04 13:41:15.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6730 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6724 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16974 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      970 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/LICENSE` & `types-aiobotocore-iotsitewise-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/setup.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsitewise",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTSiteWise 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__init__.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__init__.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/__main__.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSiteWise 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTSiteWise 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/client.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
-    AssetModelCompositeModelUnionTypeDef,
+    AssetModelCompositeModelTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
-    AssetModelPropertyUnionTypeDef,
+    AssetModelPropertyTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
@@ -107,15 +107,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
-    JobConfigurationUnionTypeDef,
+    JobConfigurationTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
@@ -358,15 +358,15 @@
     async def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: JobConfigurationUnionTypeDef
+        jobConfiguration: JobConfigurationTypeDef
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_bulk_import_job)
         """
@@ -1030,17 +1030,17 @@
 
     async def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,
+        assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[AssetModelCompositeModelUnionTypeDef] = ...,
+        assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model)
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/client.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     ListProjectAssetsPaginator,
     ListProjectsPaginator,
     ListTimeSeriesPaginator,
 )
 from .type_defs import (
     AlarmsTypeDef,
     AssetModelCompositeModelDefinitionTypeDef,
-    AssetModelCompositeModelUnionTypeDef,
+    AssetModelCompositeModelTypeDef,
     AssetModelHierarchyDefinitionTypeDef,
     AssetModelHierarchyTypeDef,
     AssetModelPropertyDefinitionTypeDef,
-    AssetModelPropertyUnionTypeDef,
+    AssetModelPropertyTypeDef,
     BatchAssociateProjectAssetsResponseTypeDef,
     BatchDisassociateProjectAssetsResponseTypeDef,
     BatchGetAssetPropertyAggregatesEntryTypeDef,
     BatchGetAssetPropertyAggregatesResponseTypeDef,
     BatchGetAssetPropertyValueEntryTypeDef,
     BatchGetAssetPropertyValueHistoryEntryTypeDef,
     BatchGetAssetPropertyValueHistoryResponseTypeDef,
@@ -107,15 +107,15 @@
     GetAssetPropertyAggregatesResponseTypeDef,
     GetAssetPropertyValueHistoryResponseTypeDef,
     GetAssetPropertyValueResponseTypeDef,
     GetInterpolatedAssetPropertyValuesResponseTypeDef,
     IdentityTypeDef,
     ImageFileTypeDef,
     ImageTypeDef,
-    JobConfigurationUnionTypeDef,
+    JobConfigurationTypeDef,
     ListAccessPoliciesResponseTypeDef,
     ListAssetModelPropertiesResponseTypeDef,
     ListAssetModelsResponseTypeDef,
     ListAssetPropertiesResponseTypeDef,
     ListAssetRelationshipsResponseTypeDef,
     ListAssetsResponseTypeDef,
     ListAssociatedAssetsResponseTypeDef,
@@ -340,15 +340,15 @@
     async def create_bulk_import_job(
         self,
         *,
         jobName: str,
         jobRoleArn: str,
         files: Sequence[FileTypeDef],
         errorReportLocation: ErrorReportLocationTypeDef,
-        jobConfiguration: JobConfigurationUnionTypeDef
+        jobConfiguration: JobConfigurationTypeDef
     ) -> CreateBulkImportJobResponseTypeDef:
         """
         Defines a job to ingest data to IoT SiteWise from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.create_bulk_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#create_bulk_import_job)
         """
@@ -956,17 +956,17 @@
         """
     async def update_asset_model(
         self,
         *,
         assetModelId: str,
         assetModelName: str,
         assetModelDescription: str = ...,
-        assetModelProperties: Sequence[AssetModelPropertyUnionTypeDef] = ...,
+        assetModelProperties: Sequence[AssetModelPropertyTypeDef] = ...,
         assetModelHierarchies: Sequence[AssetModelHierarchyTypeDef] = ...,
-        assetModelCompositeModels: Sequence[AssetModelCompositeModelUnionTypeDef] = ...,
+        assetModelCompositeModels: Sequence[AssetModelCompositeModelTypeDef] = ...,
         clientToken: str = ...
     ) -> UpdateAssetModelResponseTypeDef:
         """
         Updates an asset model and all of the assets that were created from the model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise.Client.update_asset_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/client/#update_asset_model)
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/literals.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -301,14 +302,15 @@
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
@@ -387,26 +389,28 @@
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

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/literals.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
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
@@ -299,14 +300,15 @@
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
@@ -385,26 +387,28 @@
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

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/paginator.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/paginator.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/type_defs.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AggregatesTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
@@ -94,15 +93,14 @@
     "BlobTypeDef",
     "ConfigurationErrorDetailsTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CsvOutputTypeDef",
     "CsvTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
@@ -200,15 +198,14 @@
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ImageFileTypeDef",
     "ConfigurationStatusTypeDef",
-    "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
@@ -259,28 +256,25 @@
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
-    "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
     "MeasurementTypeDef",
-    "TransformOutputTypeDef",
     "TransformTypeDef",
     "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
@@ -289,51 +283,45 @@
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "DescribeBulkImportJobResponseTypeDef",
     "CreateBulkImportJobRequestRequestTypeDef",
-    "JobConfigurationUnionTypeDef",
+    "DescribeBulkImportJobResponseTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
     "DeleteAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListGatewaysResponseTypeDef",
-    "PropertyTypeOutputTypeDef",
     "PropertyTypeTypeDef",
     "ListPortalsResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "ListAssetModelsResponseTypeDef",
     "ListAssetsResponseTypeDef",
     "ListAssociatedAssetsResponseTypeDef",
-    "AssetModelPropertyOutputTypeDef",
-    "AssetModelPropertySummaryTypeDef",
-    "PropertyTypeDef",
     "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertySummaryTypeDef",
     "AssetModelPropertyTypeDef",
-    "AssetModelCompositeModelOutputTypeDef",
-    "ListAssetModelPropertiesResponseTypeDef",
-    "CompositeModelPropertyTypeDef",
+    "PropertyTypeDef",
     "AssetModelCompositeModelDefinitionTypeDef",
+    "ListAssetModelPropertiesResponseTypeDef",
     "AssetModelCompositeModelTypeDef",
-    "AssetModelPropertyUnionTypeDef",
-    "DescribeAssetModelResponseTypeDef",
-    "DescribeAssetPropertyResponseTypeDef",
+    "CompositeModelPropertyTypeDef",
     "CreateAssetModelRequestRequestTypeDef",
-    "AssetModelCompositeModelUnionTypeDef",
+    "DescribeAssetModelResponseTypeDef",
     "UpdateAssetModelRequestRequestTypeDef",
+    "DescribeAssetPropertyResponseTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
         "count": float,
@@ -355,19 +343,17 @@
     "_OptionalAlarmsTypeDef",
     {
         "notificationLambdaArn": str,
     },
     total=False,
 )
 
-
 class AlarmsTypeDef(_RequiredAlarmsTypeDef, _OptionalAlarmsTypeDef):
     pass
 
-
 AssetErrorDetailsTypeDef = TypedDict(
     "AssetErrorDetailsTypeDef",
     {
         "assetId": str,
         "code": Literal["INTERNAL_FAILURE"],
         "message": str,
     },
@@ -392,19 +378,17 @@
     "_OptionalAssetHierarchyTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
-
 class AssetHierarchyTypeDef(_RequiredAssetHierarchyTypeDef, _OptionalAssetHierarchyTypeDef):
     pass
 
-
 AssetModelHierarchyDefinitionTypeDef = TypedDict(
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -420,21 +404,19 @@
     "_OptionalAssetModelHierarchyTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
-
 class AssetModelHierarchyTypeDef(
     _RequiredAssetModelHierarchyTypeDef, _OptionalAssetModelHierarchyTypeDef
 ):
     pass
 
-
 PropertyNotificationTypeDef = TypedDict(
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
@@ -449,19 +431,17 @@
     "_OptionalTimeInNanosTypeDef",
     {
         "offsetInNanos": int,
     },
     total=False,
 )
 
-
 class TimeInNanosTypeDef(_RequiredTimeInNanosTypeDef, _OptionalTimeInNanosTypeDef):
     pass
 
-
 VariantTypeDef = TypedDict(
     "VariantTypeDef",
     {
         "stringValue": str,
         "integerValue": int,
         "doubleValue": float,
         "booleanValue": bool,
@@ -481,21 +461,19 @@
     "_OptionalAssociateAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class AssociateAssetsRequestRequestTypeDef(
     _RequiredAssociateAssetsRequestRequestTypeDef, _OptionalAssociateAssetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
@@ -504,22 +482,20 @@
     "_OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
-
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -535,22 +511,20 @@
     "_OptionalBatchAssociateProjectAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class BatchAssociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchAssociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchAssociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -569,22 +543,20 @@
     "_OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class BatchDisassociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 TimestampTypeDef = Union[datetime, str]
 BatchGetAssetPropertyAggregatesErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyAggregatesErrorCodeType,
         "errorMessage": str,
         "entryId": str,
@@ -611,21 +583,19 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueEntryTypeDef, _OptionalBatchGetAssetPropertyValueEntryTypeDef
 ):
     pass
 
-
 BatchGetAssetPropertyValueErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -678,21 +648,19 @@
         "clientToken": str,
         "tags": Mapping[str, str],
         "assetDescription": str,
     },
     total=False,
 )
 
-
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
-
 ErrorReportLocationTypeDef = TypedDict(
     "ErrorReportLocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
 )
@@ -708,19 +676,17 @@
     "_OptionalFileTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class FileTypeDef(_RequiredFileTypeDef, _OptionalFileTypeDef):
     pass
 
-
 _RequiredCreateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDashboardRequestRequestTypeDef",
     {
         "projectId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -731,21 +697,19 @@
         "dashboardDescription": str,
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "portalId": str,
         "projectName": str,
     },
 )
@@ -755,29 +719,19 @@
         "projectDescription": str,
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
-CsvOutputTypeDef = TypedDict(
-    "CsvOutputTypeDef",
-    {
-        "columnNames": List[ColumnNameType],
-    },
-    total=False,
-)
-
 CsvTypeDef = TypedDict(
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
 )
@@ -803,104 +757,94 @@
         "description": str,
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
-
 class DashboardSummaryTypeDef(_RequiredDashboardSummaryTypeDef, _OptionalDashboardSummaryTypeDef):
     pass
 
-
 _RequiredDeleteAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
     },
 )
 _OptionalDeleteAccessPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAccessPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteAccessPolicyRequestRequestTypeDef(
     _RequiredDeleteAccessPolicyRequestRequestTypeDef,
     _OptionalDeleteAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalDeleteAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAssetModelRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteAssetModelRequestRequestTypeDef(
     _RequiredDeleteAssetModelRequestRequestTypeDef, _OptionalDeleteAssetModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteAssetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAssetRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDeleteAssetRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAssetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteAssetRequestRequestTypeDef(
     _RequiredDeleteAssetRequestRequestTypeDef, _OptionalDeleteAssetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 _OptionalDeleteDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDashboardRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteDashboardRequestRequestTypeDef(
     _RequiredDeleteDashboardRequestRequestTypeDef, _OptionalDeleteDashboardRequestRequestTypeDef
 ):
     pass
 
-
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
     },
 )
 
@@ -914,42 +858,38 @@
     "_OptionalDeletePortalRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeletePortalRequestRequestTypeDef(
     _RequiredDeletePortalRequestRequestTypeDef, _OptionalDeletePortalRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-
 DeleteTimeSeriesRequestRequestTypeDef = TypedDict(
     "DeleteTimeSeriesRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
         "clientToken": str,
@@ -983,22 +923,20 @@
     "_OptionalDescribeAssetModelRequestRequestTypeDef",
     {
         "excludeProperties": bool,
     },
     total=False,
 )
 
-
 class DescribeAssetModelRequestRequestTypeDef(
     _RequiredDescribeAssetModelRequestRequestTypeDef,
     _OptionalDescribeAssetModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAssetPropertyRequestRequestTypeDef = TypedDict(
     "DescribeAssetPropertyRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
     },
 )
@@ -1013,21 +951,19 @@
     "_OptionalDescribeAssetRequestRequestTypeDef",
     {
         "excludeProperties": bool,
     },
     total=False,
 )
 
-
 class DescribeAssetRequestRequestTypeDef(
     _RequiredDescribeAssetRequestRequestTypeDef, _OptionalDescribeAssetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -1129,22 +1065,20 @@
     "_OptionalDisassociateAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DisassociateAssetsRequestRequestTypeDef(
     _RequiredDisassociateAssetsRequestRequestTypeDef,
     _OptionalDisassociateAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
@@ -1153,41 +1087,37 @@
     "_OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef(
     _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     _OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
     "_OptionalVariableValueTypeDef",
     {
         "hierarchyId": str,
     },
     total=False,
 )
 
-
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
-
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
@@ -1246,22 +1176,20 @@
         "nextToken": str,
         "maxResults": int,
         "intervalWindowInSeconds": int,
     },
     total=False,
 )
 
-
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
-
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1321,22 +1249,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListAssetModelPropertiesFilterType,
     },
     total=False,
 )
 
-
 class ListAssetModelPropertiesRequestRequestTypeDef(
     _RequiredListAssetModelPropertiesRequestRequestTypeDef,
     _OptionalListAssetModelPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
 ListAssetModelsRequestRequestTypeDef = TypedDict(
     "ListAssetModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1354,22 +1280,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListAssetPropertiesFilterType,
     },
     total=False,
 )
 
-
 class ListAssetPropertiesRequestRequestTypeDef(
     _RequiredListAssetPropertiesRequestRequestTypeDef,
     _OptionalListAssetPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssetRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestRequestTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -1378,22 +1302,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssetRelationshipsRequestRequestTypeDef(
     _RequiredListAssetRelationshipsRequestRequestTypeDef,
     _OptionalListAssetRelationshipsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetModelId": str,
         "filter": ListAssetsFilterType,
@@ -1414,22 +1336,20 @@
         "traversalDirection": TraversalDirectionType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssociatedAssetsRequestRequestTypeDef(
     _RequiredListAssociatedAssetsRequestRequestTypeDef,
     _OptionalListAssociatedAssetsRequestRequestTypeDef,
 ):
     pass
 
-
 ListBulkImportJobsRequestRequestTypeDef = TypedDict(
     "ListBulkImportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filter": ListBulkImportJobsFilterType,
     },
@@ -1447,21 +1367,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDashboardsRequestRequestTypeDef(
     _RequiredListDashboardsRequestRequestTypeDef, _OptionalListDashboardsRequestRequestTypeDef
 ):
     pass
 
-
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1487,21 +1405,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListProjectAssetsRequestRequestTypeDef(
     _RequiredListProjectAssetsRequestRequestTypeDef, _OptionalListProjectAssetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -1509,21 +1425,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListProjectsRequestRequestTypeDef(
     _RequiredListProjectsRequestRequestTypeDef, _OptionalListProjectsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProjectSummaryTypeDef = TypedDict(
     "_RequiredProjectSummaryTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -1533,19 +1447,17 @@
         "description": str,
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
-
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1578,21 +1490,19 @@
         "propertyId": str,
         "alias": str,
         "dataTypeSpec": str,
     },
     total=False,
 )
 
-
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
-
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
@@ -1606,19 +1516,17 @@
     "_OptionalTumblingWindowTypeDef",
     {
         "offset": str,
     },
     total=False,
 )
 
-
 class TumblingWindowTypeDef(_RequiredTumblingWindowTypeDef, _OptionalTumblingWindowTypeDef):
     pass
 
-
 MonitorErrorDetailsTypeDef = TypedDict(
     "MonitorErrorDetailsTypeDef",
     {
         "code": MonitorErrorCodeType,
         "message": str,
     },
     total=False,
@@ -1648,22 +1556,20 @@
     "_OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
-
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1690,22 +1596,20 @@
         "propertyNotificationState": PropertyNotificationStateType,
         "clientToken": str,
         "propertyUnit": str,
     },
     total=False,
 )
 
-
 class UpdateAssetPropertyRequestRequestTypeDef(
     _RequiredUpdateAssetPropertyRequestRequestTypeDef,
     _OptionalUpdateAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetRequestRequestTypeDef",
     {
         "assetId": str,
         "assetName": str,
     },
 )
@@ -1714,21 +1618,19 @@
     {
         "clientToken": str,
         "assetDescription": str,
     },
     total=False,
 )
 
-
 class UpdateAssetRequestRequestTypeDef(
     _RequiredUpdateAssetRequestRequestTypeDef, _OptionalUpdateAssetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -1738,21 +1640,19 @@
     {
         "dashboardDescription": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDashboardRequestRequestTypeDef(
     _RequiredUpdateDashboardRequestRequestTypeDef, _OptionalUpdateDashboardRequestRequestTypeDef
 ):
     pass
 
-
 UpdateGatewayCapabilityConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
     {
         "gatewayId": str,
         "capabilityNamespace": str,
         "capabilityConfiguration": str,
     },
@@ -1778,21 +1678,19 @@
     {
         "projectDescription": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAggregatedValueTypeDef = TypedDict(
     "_RequiredAggregatedValueTypeDef",
     {
         "timestamp": datetime,
         "value": AggregatesTypeDef,
     },
 )
@@ -1800,40 +1698,36 @@
     "_OptionalAggregatedValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
-
 class AggregatedValueTypeDef(_RequiredAggregatedValueTypeDef, _OptionalAggregatedValueTypeDef):
     pass
 
-
 _RequiredAssetRelationshipSummaryTypeDef = TypedDict(
     "_RequiredAssetRelationshipSummaryTypeDef",
     {
         "relationshipType": Literal["HIERARCHY"],
     },
 )
 _OptionalAssetRelationshipSummaryTypeDef = TypedDict(
     "_OptionalAssetRelationshipSummaryTypeDef",
     {
         "hierarchyInfo": AssetHierarchyInfoTypeDef,
     },
     total=False,
 )
 
-
 class AssetRelationshipSummaryTypeDef(
     _RequiredAssetRelationshipSummaryTypeDef, _OptionalAssetRelationshipSummaryTypeDef
 ):
     pass
 
-
 AssetPropertySummaryTypeDef = TypedDict(
     "AssetPropertySummaryTypeDef",
     {
         "id": str,
         "alias": str,
         "unit": str,
         "notification": PropertyNotificationTypeDef,
@@ -1857,19 +1751,17 @@
         "notification": PropertyNotificationTypeDef,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
-
 class AssetPropertyTypeDef(_RequiredAssetPropertyTypeDef, _OptionalAssetPropertyTypeDef):
     pass
 
-
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
         "timestamps": List[TimeInNanosTypeDef],
     },
@@ -1886,21 +1778,19 @@
     "_OptionalAssetPropertyValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
-
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
-
 InterpolatedAssetPropertyValueTypeDef = TypedDict(
     "InterpolatedAssetPropertyValueTypeDef",
     {
         "timestamp": TimeInNanosTypeDef,
         "value": VariantTypeDef,
     },
 )
@@ -2074,22 +1964,20 @@
         "propertyAlias": str,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyAggregatesEntryTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
@@ -2102,22 +1990,20 @@
         "endDate": TimestampTypeDef,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueHistoryEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
 ):
     pass
 
-
 _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
         "startDate": TimestampTypeDef,
         "endDate": TimestampTypeDef,
@@ -2133,22 +2019,20 @@
         "timeOrdering": TimeOrderingType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
-
 GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": TimestampTypeDef,
@@ -2172,44 +2056,40 @@
     "_OptionalBatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyAggregatesSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyValueEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyValueRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyValueRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2217,22 +2097,20 @@
     "_OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyValueErrorInfoTypeDef,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2240,22 +2118,20 @@
     "_OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueHistorySkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
 ):
     pass
 
-
 ImageFileTypeDef = TypedDict(
     "ImageFileTypeDef",
     {
         "data": BlobTypeDef,
         "type": Literal["PNG"],
     },
 )
@@ -2270,29 +2146,19 @@
     "_OptionalConfigurationStatusTypeDef",
     {
         "error": ConfigurationErrorDetailsTypeDef,
     },
     total=False,
 )
 
-
 class ConfigurationStatusTypeDef(
     _RequiredConfigurationStatusTypeDef, _OptionalConfigurationStatusTypeDef
 ):
     pass
 
-
-FileFormatOutputTypeDef = TypedDict(
-    "FileFormatOutputTypeDef",
-    {
-        "csv": CsvOutputTypeDef,
-    },
-    total=False,
-)
-
 FileFormatTypeDef = TypedDict(
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
 )
@@ -2324,22 +2190,20 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssetModelRequestAssetModelActiveWaitTypeDef(
     _RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     _OptionalDescribeAssetModelRequestAssetModelActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef = TypedDict(
@@ -2347,22 +2211,20 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef(
     _RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     _OptionalDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAssetRequestAssetActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetRequestAssetActiveWaitTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDescribeAssetRequestAssetActiveWaitTypeDef = TypedDict(
@@ -2370,22 +2232,20 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssetRequestAssetActiveWaitTypeDef(
     _RequiredDescribeAssetRequestAssetActiveWaitTypeDef,
     _OptionalDescribeAssetRequestAssetActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDescribeAssetRequestAssetNotExistsWaitTypeDef = TypedDict(
@@ -2393,66 +2253,60 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssetRequestAssetNotExistsWaitTypeDef(
     _RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef,
     _OptionalDescribeAssetRequestAssetNotExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribePortalRequestPortalActiveWaitTypeDef = TypedDict(
     "_RequiredDescribePortalRequestPortalActiveWaitTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalDescribePortalRequestPortalActiveWaitTypeDef = TypedDict(
     "_OptionalDescribePortalRequestPortalActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribePortalRequestPortalActiveWaitTypeDef(
     _RequiredDescribePortalRequestPortalActiveWaitTypeDef,
     _OptionalDescribePortalRequestPortalActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribePortalRequestPortalNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribePortalRequestPortalNotExistsWaitTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribePortalRequestPortalNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribePortalRequestPortalNotExistsWaitTypeDef(
     _RequiredDescribePortalRequestPortalNotExistsWaitTypeDef,
     _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef,
 ):
     pass
 
-
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2475,19 +2329,17 @@
     "_OptionalErrorDetailsTypeDef",
     {
         "details": List[DetailedErrorTypeDef],
     },
     total=False,
 )
 
-
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
-
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
@@ -2509,21 +2361,19 @@
     "_OptionalTransformProcessingConfigTypeDef",
     {
         "forwardingConfig": ForwardingConfigTypeDef,
     },
     total=False,
 )
 
-
 class TransformProcessingConfigTypeDef(
     _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
-
 GatewayPlatformTypeDef = TypedDict(
     "GatewayPlatformTypeDef",
     {
         "greengrass": GreengrassTypeDef,
         "greengrassV2": GreengrassV2TypeDef,
     },
     total=False,
@@ -2547,22 +2397,20 @@
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
 ):
     pass
 
-
 GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": TimestampTypeDef,
@@ -2594,22 +2442,20 @@
         "endTimeOffsetInNanos": int,
         "intervalWindowInSeconds": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
 ):
     pass
 
-
 ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
     "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     {
         "identityType": IdentityTypeType,
         "identityId": str,
         "resourceType": ResourceTypeType,
         "resourceId": str,
@@ -2630,22 +2476,20 @@
     {
         "filter": ListAssetModelPropertiesFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
     _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
 ):
     pass
 
-
 ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
     "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2661,22 +2505,20 @@
     {
         "filter": ListAssetPropertiesFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
     _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
     _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -2684,22 +2526,20 @@
     "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
     _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
     _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
 ):
     pass
 
-
 ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsRequestListAssetsPaginateTypeDef",
     {
         "assetModelId": str,
         "filter": ListAssetsFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -2718,22 +2558,20 @@
         "hierarchyId": str,
         "traversalDirection": TraversalDirectionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
     _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
     _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
 ):
     pass
 
-
 ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
     "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
     {
         "filter": ListBulkImportJobsFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2749,22 +2587,20 @@
     "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDashboardsRequestListDashboardsPaginateTypeDef(
     _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
     _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
 ):
     pass
 
-
 ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
     "ListGatewaysRequestListGatewaysPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2787,44 +2623,40 @@
     "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
     _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
     _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
 ):
     pass
 
-
 ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
     "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     {
         "assetId": str,
         "aliasPrefix": str,
         "timeSeriesType": ListTimeSeriesTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2888,19 +2720,17 @@
     "_OptionalPortalStatusTypeDef",
     {
         "error": MonitorErrorDetailsTypeDef,
     },
     total=False,
 )
 
-
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -2954,21 +2784,19 @@
     {
         "description": str,
         "id": str,
     },
     total=False,
 )
 
-
 class AssetCompositeModelTypeDef(
     _RequiredAssetCompositeModelTypeDef, _OptionalAssetCompositeModelTypeDef
 ):
     pass
 
-
 BatchPutAssetPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorEntryTypeDef",
     {
         "entryId": str,
         "errors": List[BatchPutAssetPropertyErrorTypeDef],
     },
 )
@@ -2991,22 +2819,20 @@
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "assetPropertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef,
 ):
     pass
 
-
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
         "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3033,21 +2859,19 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
-
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
-
 GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     {
         "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3064,22 +2888,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
@@ -3087,22 +2909,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePortalRequestRequestTypeDef",
     {
         "portalName": str,
         "portalContactEmail": str,
         "roleArn": str,
     },
@@ -3117,21 +2937,19 @@
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
-
 class CreatePortalRequestRequestTypeDef(
     _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
 ):
     pass
 
-
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "id": str,
         "file": ImageFileTypeDef,
     },
     total=False,
@@ -3153,21 +2971,14 @@
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobConfigurationOutputTypeDef = TypedDict(
-    "JobConfigurationOutputTypeDef",
-    {
-        "fileFormat": FileFormatOutputTypeDef,
-    },
-)
-
 JobConfigurationTypeDef = TypedDict(
     "JobConfigurationTypeDef",
     {
         "fileFormat": FileFormatTypeDef,
     },
 )
 
@@ -3196,22 +3007,20 @@
         "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
-
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 PutStorageConfigurationResponseTypeDef = TypedDict(
     "PutStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
         "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
         "retentionPeriod": RetentionPeriodTypeDef,
@@ -3230,66 +3039,42 @@
     "_OptionalAssetModelStatusTypeDef",
     {
         "error": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-
 class AssetModelStatusTypeDef(_RequiredAssetModelStatusTypeDef, _OptionalAssetModelStatusTypeDef):
     pass
 
-
 _RequiredAssetStatusTypeDef = TypedDict(
     "_RequiredAssetStatusTypeDef",
     {
         "state": AssetStateType,
     },
 )
 _OptionalAssetStatusTypeDef = TypedDict(
     "_OptionalAssetStatusTypeDef",
     {
         "error": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
-
 MeasurementTypeDef = TypedDict(
     "MeasurementTypeDef",
     {
         "processingConfig": MeasurementProcessingConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredTransformOutputTypeDef = TypedDict(
-    "_RequiredTransformOutputTypeDef",
-    {
-        "expression": str,
-        "variables": List[ExpressionVariableTypeDef],
-    },
-)
-_OptionalTransformOutputTypeDef = TypedDict(
-    "_OptionalTransformOutputTypeDef",
-    {
-        "processingConfig": TransformProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
-    pass
-
-
 _RequiredTransformTypeDef = TypedDict(
     "_RequiredTransformTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
     },
 )
@@ -3297,19 +3082,17 @@
     "_OptionalTransformTypeDef",
     {
         "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
-
 class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
-
 _RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRequestRequestTypeDef",
     {
         "gatewayName": str,
         "gatewayPlatform": GatewayPlatformTypeDef,
     },
 )
@@ -3317,21 +3100,19 @@
     "_OptionalCreateGatewayRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGatewayRequestRequestTypeDef(
     _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
 ):
     pass
 
-
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
         "gatewayPlatform": GatewayPlatformTypeDef,
@@ -3356,40 +3137,17 @@
     {
         "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
-
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
-
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "expression": str,
-        "variables": List[ExpressionVariableTypeDef],
-        "window": MetricWindowTypeDef,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "processingConfig": MetricProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
-
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
         "window": MetricWindowTypeDef,
     },
@@ -3398,19 +3156,17 @@
     "_OptionalMetricTypeDef",
     {
         "processingConfig": MetricProcessingConfigTypeDef,
     },
     total=False,
 )
 
-
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
-
 CreatePortalResponseTypeDef = TypedDict(
     "CreatePortalResponseTypeDef",
     {
         "portalId": str,
         "portalArn": str,
         "portalStartUrl": str,
         "portalStatus": PortalStatusTypeDef,
@@ -3465,19 +3221,17 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
         "roleArn": str,
     },
     total=False,
 )
 
-
 class PortalSummaryTypeDef(_RequiredPortalSummaryTypeDef, _OptionalPortalSummaryTypeDef):
     pass
 
-
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3496,21 +3250,19 @@
     {
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
-
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
-
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3520,22 +3272,20 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAccessPolicyResponseTypeDef = TypedDict(
     "DescribeAccessPolicyResponseTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyArn": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
@@ -3559,22 +3309,20 @@
     "_OptionalUpdateAccessPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateAccessPolicyRequestRequestTypeDef(
     _RequiredUpdateAccessPolicyRequestRequestTypeDef,
     _OptionalUpdateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 BatchGetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyAggregatesErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyAggregatesSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyAggregatesSkippedEntryTypeDef],
         "nextToken": str,
@@ -3636,49 +3384,46 @@
         "clientToken": str,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
+CreateBulkImportJobRequestRequestTypeDef = TypedDict(
+    "CreateBulkImportJobRequestRequestTypeDef",
+    {
+        "jobName": str,
+        "jobRoleArn": str,
+        "files": Sequence[FileTypeDef],
+        "errorReportLocation": ErrorReportLocationTypeDef,
+        "jobConfiguration": JobConfigurationTypeDef,
+    },
+)
 
 DescribeBulkImportJobResponseTypeDef = TypedDict(
     "DescribeBulkImportJobResponseTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "jobRoleArn": str,
         "files": List[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
-        "jobConfiguration": JobConfigurationOutputTypeDef,
+        "jobConfiguration": JobConfigurationTypeDef,
         "jobCreationDate": datetime,
         "jobLastUpdateDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBulkImportJobRequestRequestTypeDef = TypedDict(
-    "CreateBulkImportJobRequestRequestTypeDef",
-    {
-        "jobName": str,
-        "jobRoleArn": str,
-        "files": Sequence[FileTypeDef],
-        "errorReportLocation": ErrorReportLocationTypeDef,
-        "jobConfiguration": JobConfigurationTypeDef,
-    },
-)
-
-JobConfigurationUnionTypeDef = Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
@@ -3731,19 +3476,17 @@
     "_OptionalAssetSummaryTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
     pass
 
-
 _RequiredAssociatedAssetsSummaryTypeDef = TypedDict(
     "_RequiredAssociatedAssetsSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "assetModelId": str,
@@ -3757,21 +3500,19 @@
     "_OptionalAssociatedAssetsSummaryTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class AssociatedAssetsSummaryTypeDef(
     _RequiredAssociatedAssetsSummaryTypeDef, _OptionalAssociatedAssetsSummaryTypeDef
 ):
     pass
 
-
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "assetId": str,
         "assetArn": str,
         "assetStatus": AssetStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3817,25 +3558,14 @@
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PropertyTypeOutputTypeDef = TypedDict(
-    "PropertyTypeOutputTypeDef",
-    {
-        "attribute": AttributeTypeDef,
-        "measurement": MeasurementTypeDef,
-        "transform": TransformOutputTypeDef,
-        "metric": MetricOutputTypeDef,
-    },
-    total=False,
-)
-
 PropertyTypeTypeDef = TypedDict(
     "PropertyTypeTypeDef",
     {
         "attribute": AttributeTypeDef,
         "measurement": MeasurementTypeDef,
         "transform": TransformTypeDef,
         "metric": MetricTypeDef,
@@ -3884,113 +3614,60 @@
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetModelPropertyOutputTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyOutputTypeDef",
+_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyDefinitionTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeOutputTypeDef,
+        "type": PropertyTypeTypeDef,
     },
 )
-_OptionalAssetModelPropertyOutputTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyOutputTypeDef",
+_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyDefinitionTypeDef",
     {
-        "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
-
-class AssetModelPropertyOutputTypeDef(
-    _RequiredAssetModelPropertyOutputTypeDef, _OptionalAssetModelPropertyOutputTypeDef
+class AssetModelPropertyDefinitionTypeDef(
+    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
 ):
     pass
 
-
 _RequiredAssetModelPropertySummaryTypeDef = TypedDict(
     "_RequiredAssetModelPropertySummaryTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeOutputTypeDef,
+        "type": PropertyTypeTypeDef,
     },
 )
 _OptionalAssetModelPropertySummaryTypeDef = TypedDict(
     "_OptionalAssetModelPropertySummaryTypeDef",
     {
         "id": str,
         "dataTypeSpec": str,
         "unit": str,
         "assetModelCompositeModelId": str,
     },
     total=False,
 )
 
-
 class AssetModelPropertySummaryTypeDef(
     _RequiredAssetModelPropertySummaryTypeDef, _OptionalAssetModelPropertySummaryTypeDef
 ):
     pass
 
-
-_RequiredPropertyTypeDef = TypedDict(
-    "_RequiredPropertyTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "dataType": PropertyDataTypeType,
-    },
-)
-_OptionalPropertyTypeDef = TypedDict(
-    "_OptionalPropertyTypeDef",
-    {
-        "alias": str,
-        "notification": PropertyNotificationTypeDef,
-        "unit": str,
-        "type": PropertyTypeOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
-    pass
-
-
-_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyDefinitionTypeDef",
-    {
-        "name": str,
-        "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
-    },
-)
-_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyDefinitionTypeDef",
-    {
-        "dataTypeSpec": str,
-        "unit": str,
-    },
-    total=False,
-)
-
-
-class AssetModelPropertyDefinitionTypeDef(
-    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
-):
-    pass
-
-
 _RequiredAssetModelPropertyTypeDef = TypedDict(
     "_RequiredAssetModelPropertyTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
         "type": PropertyTypeTypeDef,
     },
@@ -4001,77 +3678,41 @@
         "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
-
 class AssetModelPropertyTypeDef(
     _RequiredAssetModelPropertyTypeDef, _OptionalAssetModelPropertyTypeDef
 ):
     pass
 
-
-_RequiredAssetModelCompositeModelOutputTypeDef = TypedDict(
-    "_RequiredAssetModelCompositeModelOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-_OptionalAssetModelCompositeModelOutputTypeDef = TypedDict(
-    "_OptionalAssetModelCompositeModelOutputTypeDef",
+_RequiredPropertyTypeDef = TypedDict(
+    "_RequiredPropertyTypeDef",
     {
-        "description": str,
-        "properties": List[AssetModelPropertyOutputTypeDef],
         "id": str,
-    },
-    total=False,
-)
-
-
-class AssetModelCompositeModelOutputTypeDef(
-    _RequiredAssetModelCompositeModelOutputTypeDef, _OptionalAssetModelCompositeModelOutputTypeDef
-):
-    pass
-
-
-ListAssetModelPropertiesResponseTypeDef = TypedDict(
-    "ListAssetModelPropertiesResponseTypeDef",
-    {
-        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCompositeModelPropertyTypeDef = TypedDict(
-    "_RequiredCompositeModelPropertyTypeDef",
-    {
         "name": str,
-        "type": str,
-        "assetProperty": PropertyTypeDef,
+        "dataType": PropertyDataTypeType,
     },
 )
-_OptionalCompositeModelPropertyTypeDef = TypedDict(
-    "_OptionalCompositeModelPropertyTypeDef",
+_OptionalPropertyTypeDef = TypedDict(
+    "_OptionalPropertyTypeDef",
     {
-        "id": str,
+        "alias": str,
+        "notification": PropertyNotificationTypeDef,
+        "unit": str,
+        "type": PropertyTypeTypeDef,
     },
     total=False,
 )
 
-
-class CompositeModelPropertyTypeDef(
-    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
-):
+class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
     pass
 
-
 _RequiredAssetModelCompositeModelDefinitionTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
@@ -4080,76 +3721,72 @@
     {
         "description": str,
         "properties": Sequence[AssetModelPropertyDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class AssetModelCompositeModelDefinitionTypeDef(
     _RequiredAssetModelCompositeModelDefinitionTypeDef,
     _OptionalAssetModelCompositeModelDefinitionTypeDef,
 ):
     pass
 
+ListAssetModelPropertiesResponseTypeDef = TypedDict(
+    "ListAssetModelPropertiesResponseTypeDef",
+    {
+        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredAssetModelCompositeModelTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 _OptionalAssetModelCompositeModelTypeDef = TypedDict(
     "_OptionalAssetModelCompositeModelTypeDef",
     {
         "description": str,
-        "properties": Sequence[AssetModelPropertyTypeDef],
+        "properties": List[AssetModelPropertyTypeDef],
         "id": str,
     },
     total=False,
 )
 
-
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
-
-AssetModelPropertyUnionTypeDef = Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-DescribeAssetModelResponseTypeDef = TypedDict(
-    "DescribeAssetModelResponseTypeDef",
+_RequiredCompositeModelPropertyTypeDef = TypedDict(
+    "_RequiredCompositeModelPropertyTypeDef",
     {
-        "assetModelId": str,
-        "assetModelArn": str,
-        "assetModelName": str,
-        "assetModelDescription": str,
-        "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
-        "assetModelCreationDate": datetime,
-        "assetModelLastUpdateDate": datetime,
-        "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "type": str,
+        "assetProperty": PropertyTypeDef,
     },
 )
-
-DescribeAssetPropertyResponseTypeDef = TypedDict(
-    "DescribeAssetPropertyResponseTypeDef",
+_OptionalCompositeModelPropertyTypeDef = TypedDict(
+    "_OptionalCompositeModelPropertyTypeDef",
     {
-        "assetId": str,
-        "assetName": str,
-        "assetModelId": str,
-        "assetProperty": PropertyTypeDef,
-        "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
     },
+    total=False,
 )
 
+class CompositeModelPropertyTypeDef(
+    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
+):
+    pass
+
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
     },
 )
 _OptionalCreateAssetModelRequestRequestTypeDef = TypedDict(
@@ -4161,41 +3798,64 @@
         "assetModelCompositeModels": Sequence[AssetModelCompositeModelDefinitionTypeDef],
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
+DescribeAssetModelResponseTypeDef = TypedDict(
+    "DescribeAssetModelResponseTypeDef",
+    {
+        "assetModelId": str,
+        "assetModelArn": str,
+        "assetModelName": str,
+        "assetModelDescription": str,
+        "assetModelProperties": List[AssetModelPropertyTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
+        "assetModelCompositeModels": List[AssetModelCompositeModelTypeDef],
+        "assetModelCreationDate": datetime,
+        "assetModelLastUpdateDate": datetime,
+        "assetModelStatus": AssetModelStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-AssetModelCompositeModelUnionTypeDef = Union[
-    AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef
-]
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[AssetModelPropertyUnionTypeDef],
+        "assetModelProperties": Sequence[AssetModelPropertyTypeDef],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[AssetModelCompositeModelUnionTypeDef],
+        "assetModelCompositeModels": Sequence[AssetModelCompositeModelTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
 ):
     pass
+
+DescribeAssetPropertyResponseTypeDef = TypedDict(
+    "DescribeAssetPropertyResponseTypeDef",
+    {
+        "assetId": str,
+        "assetName": str,
+        "assetModelId": str,
+        "assetProperty": PropertyTypeDef,
+        "compositeModel": CompositeModelPropertyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/type_defs.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AggregatesTypeDef",
     "AlarmsTypeDef",
     "AssetErrorDetailsTypeDef",
     "AssetHierarchyInfoTypeDef",
     "AssetHierarchyTypeDef",
     "AssetModelHierarchyDefinitionTypeDef",
@@ -93,15 +94,14 @@
     "BlobTypeDef",
     "ConfigurationErrorDetailsTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "ErrorReportLocationTypeDef",
     "FileTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CsvOutputTypeDef",
     "CsvTypeDef",
     "CustomerManagedS3StorageTypeDef",
     "DashboardSummaryTypeDef",
     "DeleteAccessPolicyRequestRequestTypeDef",
     "DeleteAssetModelRequestRequestTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
@@ -199,15 +199,14 @@
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueRequestRequestTypeDef",
     "BatchGetAssetPropertyValueSkippedEntryTypeDef",
     "BatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     "ImageFileTypeDef",
     "ConfigurationStatusTypeDef",
-    "FileFormatOutputTypeDef",
     "FileFormatTypeDef",
     "MultiLayerStorageTypeDef",
     "ListDashboardsResponseTypeDef",
     "DescribeAssetModelRequestAssetModelActiveWaitTypeDef",
     "DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     "DescribeAssetRequestAssetActiveWaitTypeDef",
     "DescribeAssetRequestAssetNotExistsWaitTypeDef",
@@ -258,28 +257,25 @@
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     "BatchGetAssetPropertyAggregatesRequestRequestTypeDef",
     "BatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "ImageTypeDef",
     "DescribeDefaultEncryptionConfigurationResponseTypeDef",
     "PutDefaultEncryptionConfigurationResponseTypeDef",
-    "JobConfigurationOutputTypeDef",
     "JobConfigurationTypeDef",
     "DescribeStorageConfigurationResponseTypeDef",
     "PutStorageConfigurationRequestRequestTypeDef",
     "PutStorageConfigurationResponseTypeDef",
     "AssetModelStatusTypeDef",
     "AssetStatusTypeDef",
     "MeasurementTypeDef",
-    "TransformOutputTypeDef",
     "TransformTypeDef",
     "CreateGatewayRequestRequestTypeDef",
     "DescribeGatewayResponseTypeDef",
     "GatewaySummaryTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
     "CreatePortalResponseTypeDef",
     "DeletePortalResponseTypeDef",
     "DescribePortalResponseTypeDef",
     "PortalSummaryTypeDef",
     "UpdatePortalResponseTypeDef",
     "AccessPolicySummaryTypeDef",
@@ -288,51 +284,45 @@
     "UpdateAccessPolicyRequestRequestTypeDef",
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     "BatchPutAssetPropertyValueResponseTypeDef",
     "BatchGetAssetPropertyValueHistoryResponseTypeDef",
     "BatchGetAssetPropertyValueResponseTypeDef",
     "BatchPutAssetPropertyValueRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
-    "DescribeBulkImportJobResponseTypeDef",
     "CreateBulkImportJobRequestRequestTypeDef",
-    "JobConfigurationUnionTypeDef",
+    "DescribeBulkImportJobResponseTypeDef",
     "AssetModelSummaryTypeDef",
     "CreateAssetModelResponseTypeDef",
     "DeleteAssetModelResponseTypeDef",
     "UpdateAssetModelResponseTypeDef",
     "AssetSummaryTypeDef",
     "AssociatedAssetsSummaryTypeDef",
     "CreateAssetResponseTypeDef",
     "DeleteAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListGatewaysResponseTypeDef",
-    "PropertyTypeOutputTypeDef",
     "PropertyTypeTypeDef",
     "ListPortalsResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "ListAssetModelsResponseTypeDef",
     "ListAssetsResponseTypeDef",
     "ListAssociatedAssetsResponseTypeDef",
-    "AssetModelPropertyOutputTypeDef",
-    "AssetModelPropertySummaryTypeDef",
-    "PropertyTypeDef",
     "AssetModelPropertyDefinitionTypeDef",
+    "AssetModelPropertySummaryTypeDef",
     "AssetModelPropertyTypeDef",
-    "AssetModelCompositeModelOutputTypeDef",
-    "ListAssetModelPropertiesResponseTypeDef",
-    "CompositeModelPropertyTypeDef",
+    "PropertyTypeDef",
     "AssetModelCompositeModelDefinitionTypeDef",
+    "ListAssetModelPropertiesResponseTypeDef",
     "AssetModelCompositeModelTypeDef",
-    "AssetModelPropertyUnionTypeDef",
-    "DescribeAssetModelResponseTypeDef",
-    "DescribeAssetPropertyResponseTypeDef",
+    "CompositeModelPropertyTypeDef",
     "CreateAssetModelRequestRequestTypeDef",
-    "AssetModelCompositeModelUnionTypeDef",
+    "DescribeAssetModelResponseTypeDef",
     "UpdateAssetModelRequestRequestTypeDef",
+    "DescribeAssetPropertyResponseTypeDef",
 )
 
 AggregatesTypeDef = TypedDict(
     "AggregatesTypeDef",
     {
         "average": float,
         "count": float,
@@ -354,17 +344,19 @@
     "_OptionalAlarmsTypeDef",
     {
         "notificationLambdaArn": str,
     },
     total=False,
 )
 
+
 class AlarmsTypeDef(_RequiredAlarmsTypeDef, _OptionalAlarmsTypeDef):
     pass
 
+
 AssetErrorDetailsTypeDef = TypedDict(
     "AssetErrorDetailsTypeDef",
     {
         "assetId": str,
         "code": Literal["INTERNAL_FAILURE"],
         "message": str,
     },
@@ -389,17 +381,19 @@
     "_OptionalAssetHierarchyTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
+
 class AssetHierarchyTypeDef(_RequiredAssetHierarchyTypeDef, _OptionalAssetHierarchyTypeDef):
     pass
 
+
 AssetModelHierarchyDefinitionTypeDef = TypedDict(
     "AssetModelHierarchyDefinitionTypeDef",
     {
         "name": str,
         "childAssetModelId": str,
     },
 )
@@ -415,19 +409,21 @@
     "_OptionalAssetModelHierarchyTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
+
 class AssetModelHierarchyTypeDef(
     _RequiredAssetModelHierarchyTypeDef, _OptionalAssetModelHierarchyTypeDef
 ):
     pass
 
+
 PropertyNotificationTypeDef = TypedDict(
     "PropertyNotificationTypeDef",
     {
         "topic": str,
         "state": PropertyNotificationStateType,
     },
 )
@@ -442,17 +438,19 @@
     "_OptionalTimeInNanosTypeDef",
     {
         "offsetInNanos": int,
     },
     total=False,
 )
 
+
 class TimeInNanosTypeDef(_RequiredTimeInNanosTypeDef, _OptionalTimeInNanosTypeDef):
     pass
 
+
 VariantTypeDef = TypedDict(
     "VariantTypeDef",
     {
         "stringValue": str,
         "integerValue": int,
         "doubleValue": float,
         "booleanValue": bool,
@@ -472,19 +470,21 @@
     "_OptionalAssociateAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class AssociateAssetsRequestRequestTypeDef(
     _RequiredAssociateAssetsRequestRequestTypeDef, _OptionalAssociateAssetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
@@ -493,20 +493,22 @@
     "_OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(
     _RequiredAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
     _OptionalAssociateTimeSeriesToAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "defaultValue": str,
     },
     total=False,
 )
@@ -522,20 +524,22 @@
     "_OptionalBatchAssociateProjectAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class BatchAssociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchAssociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchAssociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -554,20 +558,22 @@
     "_OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class BatchDisassociateProjectAssetsRequestRequestTypeDef(
     _RequiredBatchDisassociateProjectAssetsRequestRequestTypeDef,
     _OptionalBatchDisassociateProjectAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 TimestampTypeDef = Union[datetime, str]
 BatchGetAssetPropertyAggregatesErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyAggregatesErrorCodeType,
         "errorMessage": str,
         "entryId": str,
@@ -594,19 +600,21 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueEntryTypeDef, _OptionalBatchGetAssetPropertyValueEntryTypeDef
 ):
     pass
 
+
 BatchGetAssetPropertyValueErrorEntryTypeDef = TypedDict(
     "BatchGetAssetPropertyValueErrorEntryTypeDef",
     {
         "errorCode": BatchGetAssetPropertyValueErrorCodeType,
         "errorMessage": str,
         "entryId": str,
     },
@@ -659,19 +667,21 @@
         "clientToken": str,
         "tags": Mapping[str, str],
         "assetDescription": str,
     },
     total=False,
 )
 
+
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
+
 ErrorReportLocationTypeDef = TypedDict(
     "ErrorReportLocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
 )
@@ -687,17 +697,19 @@
     "_OptionalFileTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class FileTypeDef(_RequiredFileTypeDef, _OptionalFileTypeDef):
     pass
 
+
 _RequiredCreateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDashboardRequestRequestTypeDef",
     {
         "projectId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -708,19 +720,21 @@
         "dashboardDescription": str,
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "portalId": str,
         "projectName": str,
     },
 )
@@ -730,26 +744,20 @@
         "projectDescription": str,
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-CsvOutputTypeDef = TypedDict(
-    "CsvOutputTypeDef",
-    {
-        "columnNames": List[ColumnNameType],
-    },
-    total=False,
-)
 
 CsvTypeDef = TypedDict(
     "CsvTypeDef",
     {
         "columnNames": Sequence[ColumnNameType],
     },
     total=False,
@@ -776,94 +784,104 @@
         "description": str,
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
+
 class DashboardSummaryTypeDef(_RequiredDashboardSummaryTypeDef, _OptionalDashboardSummaryTypeDef):
     pass
 
+
 _RequiredDeleteAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyId": str,
     },
 )
 _OptionalDeleteAccessPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAccessPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteAccessPolicyRequestRequestTypeDef(
     _RequiredDeleteAccessPolicyRequestRequestTypeDef,
     _OptionalDeleteAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalDeleteAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAssetModelRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteAssetModelRequestRequestTypeDef(
     _RequiredDeleteAssetModelRequestRequestTypeDef, _OptionalDeleteAssetModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteAssetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAssetRequestRequestTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDeleteAssetRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAssetRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteAssetRequestRequestTypeDef(
     _RequiredDeleteAssetRequestRequestTypeDef, _OptionalDeleteAssetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
     },
 )
 _OptionalDeleteDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDashboardRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteDashboardRequestRequestTypeDef(
     _RequiredDeleteDashboardRequestRequestTypeDef, _OptionalDeleteDashboardRequestRequestTypeDef
 ):
     pass
 
+
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "gatewayId": str,
     },
 )
 
@@ -877,38 +895,42 @@
     "_OptionalDeletePortalRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeletePortalRequestRequestTypeDef(
     _RequiredDeletePortalRequestRequestTypeDef, _OptionalDeletePortalRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
+
 DeleteTimeSeriesRequestRequestTypeDef = TypedDict(
     "DeleteTimeSeriesRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
         "clientToken": str,
@@ -942,20 +964,22 @@
     "_OptionalDescribeAssetModelRequestRequestTypeDef",
     {
         "excludeProperties": bool,
     },
     total=False,
 )
 
+
 class DescribeAssetModelRequestRequestTypeDef(
     _RequiredDescribeAssetModelRequestRequestTypeDef,
     _OptionalDescribeAssetModelRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAssetPropertyRequestRequestTypeDef = TypedDict(
     "DescribeAssetPropertyRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
     },
 )
@@ -970,19 +994,21 @@
     "_OptionalDescribeAssetRequestRequestTypeDef",
     {
         "excludeProperties": bool,
     },
     total=False,
 )
 
+
 class DescribeAssetRequestRequestTypeDef(
     _RequiredDescribeAssetRequestRequestTypeDef, _OptionalDescribeAssetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeBulkImportJobRequestRequestTypeDef = TypedDict(
     "DescribeBulkImportJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -1084,20 +1110,22 @@
     "_OptionalDisassociateAssetsRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DisassociateAssetsRequestRequestTypeDef(
     _RequiredDisassociateAssetsRequestRequestTypeDef,
     _OptionalDisassociateAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     {
         "alias": str,
         "assetId": str,
         "propertyId": str,
     },
@@ -1106,37 +1134,41 @@
     "_OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef(
     _RequiredDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
     _OptionalDisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredVariableValueTypeDef = TypedDict(
     "_RequiredVariableValueTypeDef",
     {
         "propertyId": str,
     },
 )
 _OptionalVariableValueTypeDef = TypedDict(
     "_OptionalVariableValueTypeDef",
     {
         "hierarchyId": str,
     },
     total=False,
 )
 
+
 class VariableValueTypeDef(_RequiredVariableValueTypeDef, _OptionalVariableValueTypeDef):
     pass
 
+
 ForwardingConfigTypeDef = TypedDict(
     "ForwardingConfigTypeDef",
     {
         "state": ForwardingConfigStateType,
     },
 )
 
@@ -1195,20 +1227,22 @@
         "nextToken": str,
         "maxResults": int,
         "intervalWindowInSeconds": int,
     },
     total=False,
 )
 
+
 class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestRequestTypeDef,
 ):
     pass
 
+
 GroupIdentityTypeDef = TypedDict(
     "GroupIdentityTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1268,20 +1302,22 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListAssetModelPropertiesFilterType,
     },
     total=False,
 )
 
+
 class ListAssetModelPropertiesRequestRequestTypeDef(
     _RequiredListAssetModelPropertiesRequestRequestTypeDef,
     _OptionalListAssetModelPropertiesRequestRequestTypeDef,
 ):
     pass
 
+
 ListAssetModelsRequestRequestTypeDef = TypedDict(
     "ListAssetModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1299,20 +1335,22 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListAssetPropertiesFilterType,
     },
     total=False,
 )
 
+
 class ListAssetPropertiesRequestRequestTypeDef(
     _RequiredListAssetPropertiesRequestRequestTypeDef,
     _OptionalListAssetPropertiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssetRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestRequestTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -1321,20 +1359,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssetRelationshipsRequestRequestTypeDef(
     _RequiredListAssetRelationshipsRequestRequestTypeDef,
     _OptionalListAssetRelationshipsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAssetsRequestRequestTypeDef = TypedDict(
     "ListAssetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "assetModelId": str,
         "filter": ListAssetsFilterType,
@@ -1355,20 +1395,22 @@
         "traversalDirection": TraversalDirectionType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssociatedAssetsRequestRequestTypeDef(
     _RequiredListAssociatedAssetsRequestRequestTypeDef,
     _OptionalListAssociatedAssetsRequestRequestTypeDef,
 ):
     pass
 
+
 ListBulkImportJobsRequestRequestTypeDef = TypedDict(
     "ListBulkImportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filter": ListBulkImportJobsFilterType,
     },
@@ -1386,19 +1428,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListDashboardsRequestRequestTypeDef(
     _RequiredListDashboardsRequestRequestTypeDef, _OptionalListDashboardsRequestRequestTypeDef
 ):
     pass
 
+
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1424,19 +1468,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListProjectAssetsRequestRequestTypeDef(
     _RequiredListProjectAssetsRequestRequestTypeDef, _OptionalListProjectAssetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListProjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectsRequestRequestTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestRequestTypeDef = TypedDict(
@@ -1444,19 +1490,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListProjectsRequestRequestTypeDef(
     _RequiredListProjectsRequestRequestTypeDef, _OptionalListProjectsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProjectSummaryTypeDef = TypedDict(
     "_RequiredProjectSummaryTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
@@ -1466,17 +1514,19 @@
         "description": str,
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
+
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1509,19 +1559,21 @@
         "propertyId": str,
         "alias": str,
         "dataTypeSpec": str,
     },
     total=False,
 )
 
+
 class TimeSeriesSummaryTypeDef(
     _RequiredTimeSeriesSummaryTypeDef, _OptionalTimeSeriesSummaryTypeDef
 ):
     pass
 
+
 MetricProcessingConfigTypeDef = TypedDict(
     "MetricProcessingConfigTypeDef",
     {
         "computeLocation": ComputeLocationType,
     },
 )
 
@@ -1535,17 +1587,19 @@
     "_OptionalTumblingWindowTypeDef",
     {
         "offset": str,
     },
     total=False,
 )
 
+
 class TumblingWindowTypeDef(_RequiredTumblingWindowTypeDef, _OptionalTumblingWindowTypeDef):
     pass
 
+
 MonitorErrorDetailsTypeDef = TypedDict(
     "MonitorErrorDetailsTypeDef",
     {
         "code": MonitorErrorCodeType,
         "message": str,
     },
     total=False,
@@ -1575,20 +1629,22 @@
     "_OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
+
 class PutDefaultEncryptionConfigurationRequestRequestTypeDef(
     _RequiredPutDefaultEncryptionConfigurationRequestRequestTypeDef,
     _OptionalPutDefaultEncryptionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1615,20 +1671,22 @@
         "propertyNotificationState": PropertyNotificationStateType,
         "clientToken": str,
         "propertyUnit": str,
     },
     total=False,
 )
 
+
 class UpdateAssetPropertyRequestRequestTypeDef(
     _RequiredUpdateAssetPropertyRequestRequestTypeDef,
     _OptionalUpdateAssetPropertyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetRequestRequestTypeDef",
     {
         "assetId": str,
         "assetName": str,
     },
 )
@@ -1637,19 +1695,21 @@
     {
         "clientToken": str,
         "assetDescription": str,
     },
     total=False,
 )
 
+
 class UpdateAssetRequestRequestTypeDef(
     _RequiredUpdateAssetRequestRequestTypeDef, _OptionalUpdateAssetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDashboardRequestRequestTypeDef",
     {
         "dashboardId": str,
         "dashboardName": str,
         "dashboardDefinition": str,
     },
@@ -1659,19 +1719,21 @@
     {
         "dashboardDescription": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDashboardRequestRequestTypeDef(
     _RequiredUpdateDashboardRequestRequestTypeDef, _OptionalUpdateDashboardRequestRequestTypeDef
 ):
     pass
 
+
 UpdateGatewayCapabilityConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGatewayCapabilityConfigurationRequestRequestTypeDef",
     {
         "gatewayId": str,
         "capabilityNamespace": str,
         "capabilityConfiguration": str,
     },
@@ -1697,19 +1759,21 @@
     {
         "projectDescription": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAggregatedValueTypeDef = TypedDict(
     "_RequiredAggregatedValueTypeDef",
     {
         "timestamp": datetime,
         "value": AggregatesTypeDef,
     },
 )
@@ -1717,36 +1781,40 @@
     "_OptionalAggregatedValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
+
 class AggregatedValueTypeDef(_RequiredAggregatedValueTypeDef, _OptionalAggregatedValueTypeDef):
     pass
 
+
 _RequiredAssetRelationshipSummaryTypeDef = TypedDict(
     "_RequiredAssetRelationshipSummaryTypeDef",
     {
         "relationshipType": Literal["HIERARCHY"],
     },
 )
 _OptionalAssetRelationshipSummaryTypeDef = TypedDict(
     "_OptionalAssetRelationshipSummaryTypeDef",
     {
         "hierarchyInfo": AssetHierarchyInfoTypeDef,
     },
     total=False,
 )
 
+
 class AssetRelationshipSummaryTypeDef(
     _RequiredAssetRelationshipSummaryTypeDef, _OptionalAssetRelationshipSummaryTypeDef
 ):
     pass
 
+
 AssetPropertySummaryTypeDef = TypedDict(
     "AssetPropertySummaryTypeDef",
     {
         "id": str,
         "alias": str,
         "unit": str,
         "notification": PropertyNotificationTypeDef,
@@ -1770,17 +1838,19 @@
         "notification": PropertyNotificationTypeDef,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
+
 class AssetPropertyTypeDef(_RequiredAssetPropertyTypeDef, _OptionalAssetPropertyTypeDef):
     pass
 
+
 BatchPutAssetPropertyErrorTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorTypeDef",
     {
         "errorCode": BatchPutAssetPropertyValueErrorCodeType,
         "errorMessage": str,
         "timestamps": List[TimeInNanosTypeDef],
     },
@@ -1797,19 +1867,21 @@
     "_OptionalAssetPropertyValueTypeDef",
     {
         "quality": QualityType,
     },
     total=False,
 )
 
+
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
+
 InterpolatedAssetPropertyValueTypeDef = TypedDict(
     "InterpolatedAssetPropertyValueTypeDef",
     {
         "timestamp": TimeInNanosTypeDef,
         "value": VariantTypeDef,
     },
 )
@@ -1983,20 +2055,22 @@
         "propertyAlias": str,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyAggregatesEntryTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesEntryTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesEntryTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef",
     {
         "entryId": str,
     },
 )
 _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef = TypedDict(
@@ -2009,20 +2083,22 @@
         "endDate": TimestampTypeDef,
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueHistoryEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistoryEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistoryEntryTypeDef,
 ):
     pass
 
+
 _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssetPropertyAggregatesRequestRequestTypeDef",
     {
         "aggregateTypes": Sequence[AggregateTypeType],
         "resolution": str,
         "startDate": TimestampTypeDef,
         "endDate": TimestampTypeDef,
@@ -2038,20 +2114,22 @@
         "timeOrdering": TimeOrderingType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
+
 GetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": TimestampTypeDef,
@@ -2075,40 +2153,44 @@
     "_OptionalBatchGetAssetPropertyAggregatesSkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyAggregatesErrorInfoTypeDef,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyAggregatesSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesSkippedEntryTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyValueEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyValueRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGetAssetPropertyValueRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyValueRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyValueRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2116,20 +2198,22 @@
     "_OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyValueErrorInfoTypeDef,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueSkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSkippedEntryTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "entryId": str,
         "completionStatus": BatchEntryCompletionStatusType,
     },
 )
@@ -2137,20 +2221,22 @@
     "_OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef",
     {
         "errorInfo": BatchGetAssetPropertyValueHistoryErrorInfoTypeDef,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueHistorySkippedEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueHistorySkippedEntryTypeDef,
 ):
     pass
 
+
 ImageFileTypeDef = TypedDict(
     "ImageFileTypeDef",
     {
         "data": BlobTypeDef,
         "type": Literal["PNG"],
     },
 )
@@ -2165,26 +2251,20 @@
     "_OptionalConfigurationStatusTypeDef",
     {
         "error": ConfigurationErrorDetailsTypeDef,
     },
     total=False,
 )
 
+
 class ConfigurationStatusTypeDef(
     _RequiredConfigurationStatusTypeDef, _OptionalConfigurationStatusTypeDef
 ):
     pass
 
-FileFormatOutputTypeDef = TypedDict(
-    "FileFormatOutputTypeDef",
-    {
-        "csv": CsvOutputTypeDef,
-    },
-    total=False,
-)
 
 FileFormatTypeDef = TypedDict(
     "FileFormatTypeDef",
     {
         "csv": CsvTypeDef,
     },
     total=False,
@@ -2217,20 +2297,22 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssetModelRequestAssetModelActiveWaitTypeDef(
     _RequiredDescribeAssetModelRequestAssetModelActiveWaitTypeDef,
     _OptionalDescribeAssetModelRequestAssetModelActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef",
     {
         "assetModelId": str,
     },
 )
 _OptionalDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef = TypedDict(
@@ -2238,20 +2320,22 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef(
     _RequiredDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
     _OptionalDescribeAssetModelRequestAssetModelNotExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAssetRequestAssetActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetRequestAssetActiveWaitTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDescribeAssetRequestAssetActiveWaitTypeDef = TypedDict(
@@ -2259,20 +2343,22 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssetRequestAssetActiveWaitTypeDef(
     _RequiredDescribeAssetRequestAssetActiveWaitTypeDef,
     _OptionalDescribeAssetRequestAssetActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef",
     {
         "assetId": str,
     },
 )
 _OptionalDescribeAssetRequestAssetNotExistsWaitTypeDef = TypedDict(
@@ -2280,60 +2366,66 @@
     {
         "excludeProperties": bool,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssetRequestAssetNotExistsWaitTypeDef(
     _RequiredDescribeAssetRequestAssetNotExistsWaitTypeDef,
     _OptionalDescribeAssetRequestAssetNotExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribePortalRequestPortalActiveWaitTypeDef = TypedDict(
     "_RequiredDescribePortalRequestPortalActiveWaitTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalDescribePortalRequestPortalActiveWaitTypeDef = TypedDict(
     "_OptionalDescribePortalRequestPortalActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribePortalRequestPortalActiveWaitTypeDef(
     _RequiredDescribePortalRequestPortalActiveWaitTypeDef,
     _OptionalDescribePortalRequestPortalActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribePortalRequestPortalNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribePortalRequestPortalNotExistsWaitTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribePortalRequestPortalNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribePortalRequestPortalNotExistsWaitTypeDef(
     _RequiredDescribePortalRequestPortalNotExistsWaitTypeDef,
     _OptionalDescribePortalRequestPortalNotExistsWaitTypeDef,
 ):
     pass
 
+
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2356,17 +2448,19 @@
     "_OptionalErrorDetailsTypeDef",
     {
         "details": List[DetailedErrorTypeDef],
     },
     total=False,
 )
 
+
 class ErrorDetailsTypeDef(_RequiredErrorDetailsTypeDef, _OptionalErrorDetailsTypeDef):
     pass
 
+
 ExpressionVariableTypeDef = TypedDict(
     "ExpressionVariableTypeDef",
     {
         "name": str,
         "value": VariableValueTypeDef,
     },
 )
@@ -2388,19 +2482,21 @@
     "_OptionalTransformProcessingConfigTypeDef",
     {
         "forwardingConfig": ForwardingConfigTypeDef,
     },
     total=False,
 )
 
+
 class TransformProcessingConfigTypeDef(
     _RequiredTransformProcessingConfigTypeDef, _OptionalTransformProcessingConfigTypeDef
 ):
     pass
 
+
 GatewayPlatformTypeDef = TypedDict(
     "GatewayPlatformTypeDef",
     {
         "greengrass": GreengrassTypeDef,
         "greengrassV2": GreengrassV2TypeDef,
     },
     total=False,
@@ -2424,20 +2520,22 @@
         "qualities": Sequence[QualityType],
         "timeOrdering": TimeOrderingType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(
     _RequiredGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
     _OptionalGetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef,
 ):
     pass
 
+
 GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef",
     {
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "startDate": TimestampTypeDef,
@@ -2469,20 +2567,22 @@
         "endTimeOffsetInNanos": int,
         "intervalWindowInSeconds": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(
     _RequiredGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
     _OptionalGetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef,
 ):
     pass
 
+
 ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef = TypedDict(
     "ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef",
     {
         "identityType": IdentityTypeType,
         "identityId": str,
         "resourceType": ResourceTypeType,
         "resourceId": str,
@@ -2503,20 +2603,22 @@
     {
         "filter": ListAssetModelPropertiesFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(
     _RequiredListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
     _OptionalListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef,
 ):
     pass
 
+
 ListAssetModelsRequestListAssetModelsPaginateTypeDef = TypedDict(
     "ListAssetModelsRequestListAssetModelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2532,20 +2634,22 @@
     {
         "filter": ListAssetPropertiesFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(
     _RequiredListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
     _OptionalListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef = TypedDict(
     "_RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     {
         "assetId": str,
         "traversalType": Literal["PATH_TO_ROOT"],
     },
 )
@@ -2553,20 +2657,22 @@
     "_OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(
     _RequiredListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
     _OptionalListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef,
 ):
     pass
 
+
 ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsRequestListAssetsPaginateTypeDef",
     {
         "assetModelId": str,
         "filter": ListAssetsFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -2585,20 +2691,22 @@
         "hierarchyId": str,
         "traversalDirection": TraversalDirectionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(
     _RequiredListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
     _OptionalListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef,
 ):
     pass
 
+
 ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef = TypedDict(
     "ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef",
     {
         "filter": ListBulkImportJobsFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2614,20 +2722,22 @@
     "_OptionalListDashboardsRequestListDashboardsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDashboardsRequestListDashboardsPaginateTypeDef(
     _RequiredListDashboardsRequestListDashboardsPaginateTypeDef,
     _OptionalListDashboardsRequestListDashboardsPaginateTypeDef,
 ):
     pass
 
+
 ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
     "ListGatewaysRequestListGatewaysPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2650,40 +2760,44 @@
     "_OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(
     _RequiredListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
     _OptionalListProjectAssetsRequestListProjectAssetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "portalId": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
 ):
     pass
 
+
 ListTimeSeriesRequestListTimeSeriesPaginateTypeDef = TypedDict(
     "ListTimeSeriesRequestListTimeSeriesPaginateTypeDef",
     {
         "assetId": str,
         "aliasPrefix": str,
         "timeSeriesType": ListTimeSeriesTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2747,17 +2861,19 @@
     "_OptionalPortalStatusTypeDef",
     {
         "error": MonitorErrorDetailsTypeDef,
     },
     total=False,
 )
 
+
 class PortalStatusTypeDef(_RequiredPortalStatusTypeDef, _OptionalPortalStatusTypeDef):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "portal": PortalResourceTypeDef,
         "project": ProjectResourceTypeDef,
     },
     total=False,
@@ -2811,19 +2927,21 @@
     {
         "description": str,
         "id": str,
     },
     total=False,
 )
 
+
 class AssetCompositeModelTypeDef(
     _RequiredAssetCompositeModelTypeDef, _OptionalAssetCompositeModelTypeDef
 ):
     pass
 
+
 BatchPutAssetPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutAssetPropertyErrorEntryTypeDef",
     {
         "entryId": str,
         "errors": List[BatchPutAssetPropertyErrorTypeDef],
     },
 )
@@ -2846,20 +2964,22 @@
     "_OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef",
     {
         "assetPropertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueSuccessEntryTypeDef(
     _RequiredBatchGetAssetPropertyValueSuccessEntryTypeDef,
     _OptionalBatchGetAssetPropertyValueSuccessEntryTypeDef,
 ):
     pass
 
+
 GetAssetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetAssetPropertyValueHistoryResponseTypeDef",
     {
         "assetPropertyValueHistory": List[AssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2886,19 +3006,21 @@
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
     },
     total=False,
 )
 
+
 class PutAssetPropertyValueEntryTypeDef(
     _RequiredPutAssetPropertyValueEntryTypeDef, _OptionalPutAssetPropertyValueEntryTypeDef
 ):
     pass
 
+
 GetInterpolatedAssetPropertyValuesResponseTypeDef = TypedDict(
     "GetInterpolatedAssetPropertyValuesResponseTypeDef",
     {
         "interpolatedAssetPropertyValues": List[InterpolatedAssetPropertyValueTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2915,20 +3037,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyAggregatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entries": Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],
     },
 )
 _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
@@ -2936,20 +3060,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalBatchGetAssetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePortalRequestRequestTypeDef",
     {
         "portalName": str,
         "portalContactEmail": str,
         "roleArn": str,
     },
@@ -2964,19 +3090,21 @@
         "portalAuthMode": AuthModeType,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
+
 class CreatePortalRequestRequestTypeDef(
     _RequiredCreatePortalRequestRequestTypeDef, _OptionalCreatePortalRequestRequestTypeDef
 ):
     pass
 
+
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "id": str,
         "file": ImageFileTypeDef,
     },
     total=False,
@@ -2998,21 +3126,14 @@
         "encryptionType": EncryptionTypeType,
         "kmsKeyArn": str,
         "configurationStatus": ConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobConfigurationOutputTypeDef = TypedDict(
-    "JobConfigurationOutputTypeDef",
-    {
-        "fileFormat": FileFormatOutputTypeDef,
-    },
-)
-
 JobConfigurationTypeDef = TypedDict(
     "JobConfigurationTypeDef",
     {
         "fileFormat": FileFormatTypeDef,
     },
 )
 
@@ -3041,20 +3162,22 @@
         "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
+
 class PutStorageConfigurationRequestRequestTypeDef(
     _RequiredPutStorageConfigurationRequestRequestTypeDef,
     _OptionalPutStorageConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 PutStorageConfigurationResponseTypeDef = TypedDict(
     "PutStorageConfigurationResponseTypeDef",
     {
         "storageType": StorageTypeType,
         "multiLayerStorage": MultiLayerStorageTypeDef,
         "disassociatedDataStorage": DisassociatedDataStorageStateType,
         "retentionPeriod": RetentionPeriodTypeDef,
@@ -3073,60 +3196,46 @@
     "_OptionalAssetModelStatusTypeDef",
     {
         "error": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
+
 class AssetModelStatusTypeDef(_RequiredAssetModelStatusTypeDef, _OptionalAssetModelStatusTypeDef):
     pass
 
+
 _RequiredAssetStatusTypeDef = TypedDict(
     "_RequiredAssetStatusTypeDef",
     {
         "state": AssetStateType,
     },
 )
 _OptionalAssetStatusTypeDef = TypedDict(
     "_OptionalAssetStatusTypeDef",
     {
         "error": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
+
 class AssetStatusTypeDef(_RequiredAssetStatusTypeDef, _OptionalAssetStatusTypeDef):
     pass
 
+
 MeasurementTypeDef = TypedDict(
     "MeasurementTypeDef",
     {
         "processingConfig": MeasurementProcessingConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredTransformOutputTypeDef = TypedDict(
-    "_RequiredTransformOutputTypeDef",
-    {
-        "expression": str,
-        "variables": List[ExpressionVariableTypeDef],
-    },
-)
-_OptionalTransformOutputTypeDef = TypedDict(
-    "_OptionalTransformOutputTypeDef",
-    {
-        "processingConfig": TransformProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
-class TransformOutputTypeDef(_RequiredTransformOutputTypeDef, _OptionalTransformOutputTypeDef):
-    pass
-
 _RequiredTransformTypeDef = TypedDict(
     "_RequiredTransformTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
     },
 )
@@ -3134,17 +3243,19 @@
     "_OptionalTransformTypeDef",
     {
         "processingConfig": TransformProcessingConfigTypeDef,
     },
     total=False,
 )
 
+
 class TransformTypeDef(_RequiredTransformTypeDef, _OptionalTransformTypeDef):
     pass
 
+
 _RequiredCreateGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRequestRequestTypeDef",
     {
         "gatewayName": str,
         "gatewayPlatform": GatewayPlatformTypeDef,
     },
 )
@@ -3152,19 +3263,21 @@
     "_OptionalCreateGatewayRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGatewayRequestRequestTypeDef(
     _RequiredCreateGatewayRequestRequestTypeDef, _OptionalCreateGatewayRequestRequestTypeDef
 ):
     pass
 
+
 DescribeGatewayResponseTypeDef = TypedDict(
     "DescribeGatewayResponseTypeDef",
     {
         "gatewayId": str,
         "gatewayName": str,
         "gatewayArn": str,
         "gatewayPlatform": GatewayPlatformTypeDef,
@@ -3189,35 +3302,18 @@
     {
         "gatewayPlatform": GatewayPlatformTypeDef,
         "gatewayCapabilitySummaries": List[GatewayCapabilitySummaryTypeDef],
     },
     total=False,
 )
 
+
 class GatewaySummaryTypeDef(_RequiredGatewaySummaryTypeDef, _OptionalGatewaySummaryTypeDef):
     pass
 
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "expression": str,
-        "variables": List[ExpressionVariableTypeDef],
-        "window": MetricWindowTypeDef,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "processingConfig": MetricProcessingConfigTypeDef,
-    },
-    total=False,
-)
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "expression": str,
         "variables": Sequence[ExpressionVariableTypeDef],
         "window": MetricWindowTypeDef,
@@ -3227,17 +3323,19 @@
     "_OptionalMetricTypeDef",
     {
         "processingConfig": MetricProcessingConfigTypeDef,
     },
     total=False,
 )
 
+
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
+
 CreatePortalResponseTypeDef = TypedDict(
     "CreatePortalResponseTypeDef",
     {
         "portalId": str,
         "portalArn": str,
         "portalStartUrl": str,
         "portalStatus": PortalStatusTypeDef,
@@ -3292,17 +3390,19 @@
         "creationDate": datetime,
         "lastUpdateDate": datetime,
         "roleArn": str,
     },
     total=False,
 )
 
+
 class PortalSummaryTypeDef(_RequiredPortalSummaryTypeDef, _OptionalPortalSummaryTypeDef):
     pass
 
+
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portalStatus": PortalStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3321,19 +3421,21 @@
     {
         "creationDate": datetime,
         "lastUpdateDate": datetime,
     },
     total=False,
 )
 
+
 class AccessPolicySummaryTypeDef(
     _RequiredAccessPolicySummaryTypeDef, _OptionalAccessPolicySummaryTypeDef
 ):
     pass
 
+
 _RequiredCreateAccessPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPolicyRequestRequestTypeDef",
     {
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
         "accessPolicyPermission": PermissionType,
     },
@@ -3343,20 +3445,22 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAccessPolicyRequestRequestTypeDef(
     _RequiredCreateAccessPolicyRequestRequestTypeDef,
     _OptionalCreateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAccessPolicyResponseTypeDef = TypedDict(
     "DescribeAccessPolicyResponseTypeDef",
     {
         "accessPolicyId": str,
         "accessPolicyArn": str,
         "accessPolicyIdentity": IdentityTypeDef,
         "accessPolicyResource": ResourceTypeDef,
@@ -3380,20 +3484,22 @@
     "_OptionalUpdateAccessPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateAccessPolicyRequestRequestTypeDef(
     _RequiredUpdateAccessPolicyRequestRequestTypeDef,
     _OptionalUpdateAccessPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 BatchGetAssetPropertyAggregatesResponseTypeDef = TypedDict(
     "BatchGetAssetPropertyAggregatesResponseTypeDef",
     {
         "errorEntries": List[BatchGetAssetPropertyAggregatesErrorEntryTypeDef],
         "successEntries": List[BatchGetAssetPropertyAggregatesSuccessEntryTypeDef],
         "skippedEntries": List[BatchGetAssetPropertyAggregatesSkippedEntryTypeDef],
         "nextToken": str,
@@ -3455,47 +3561,48 @@
         "clientToken": str,
         "notificationSenderEmail": str,
         "alarms": AlarmsTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
-DescribeBulkImportJobResponseTypeDef = TypedDict(
-    "DescribeBulkImportJobResponseTypeDef",
+
+CreateBulkImportJobRequestRequestTypeDef = TypedDict(
+    "CreateBulkImportJobRequestRequestTypeDef",
     {
-        "jobId": str,
         "jobName": str,
-        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": List[FileTypeDef],
+        "files": Sequence[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
-        "jobConfiguration": JobConfigurationOutputTypeDef,
-        "jobCreationDate": datetime,
-        "jobLastUpdateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "jobConfiguration": JobConfigurationTypeDef,
     },
 )
 
-CreateBulkImportJobRequestRequestTypeDef = TypedDict(
-    "CreateBulkImportJobRequestRequestTypeDef",
+DescribeBulkImportJobResponseTypeDef = TypedDict(
+    "DescribeBulkImportJobResponseTypeDef",
     {
+        "jobId": str,
         "jobName": str,
+        "jobStatus": JobStatusType,
         "jobRoleArn": str,
-        "files": Sequence[FileTypeDef],
+        "files": List[FileTypeDef],
         "errorReportLocation": ErrorReportLocationTypeDef,
         "jobConfiguration": JobConfigurationTypeDef,
+        "jobCreationDate": datetime,
+        "jobLastUpdateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobConfigurationUnionTypeDef = Union[JobConfigurationTypeDef, JobConfigurationOutputTypeDef]
 AssetModelSummaryTypeDef = TypedDict(
     "AssetModelSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
@@ -3548,17 +3655,19 @@
     "_OptionalAssetSummaryTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
     pass
 
+
 _RequiredAssociatedAssetsSummaryTypeDef = TypedDict(
     "_RequiredAssociatedAssetsSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "assetModelId": str,
@@ -3572,19 +3681,21 @@
     "_OptionalAssociatedAssetsSummaryTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class AssociatedAssetsSummaryTypeDef(
     _RequiredAssociatedAssetsSummaryTypeDef, _OptionalAssociatedAssetsSummaryTypeDef
 ):
     pass
 
+
 CreateAssetResponseTypeDef = TypedDict(
     "CreateAssetResponseTypeDef",
     {
         "assetId": str,
         "assetArn": str,
         "assetStatus": AssetStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3630,25 +3741,14 @@
     {
         "gatewaySummaries": List[GatewaySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PropertyTypeOutputTypeDef = TypedDict(
-    "PropertyTypeOutputTypeDef",
-    {
-        "attribute": AttributeTypeDef,
-        "measurement": MeasurementTypeDef,
-        "transform": TransformOutputTypeDef,
-        "metric": MetricOutputTypeDef,
-    },
-    total=False,
-)
-
 PropertyTypeTypeDef = TypedDict(
     "PropertyTypeTypeDef",
     {
         "attribute": AttributeTypeDef,
         "measurement": MeasurementTypeDef,
         "transform": TransformTypeDef,
         "metric": MetricTypeDef,
@@ -3697,104 +3797,63 @@
     {
         "assetSummaries": List[AssociatedAssetsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetModelPropertyOutputTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyOutputTypeDef",
+_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_RequiredAssetModelPropertyDefinitionTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeOutputTypeDef,
+        "type": PropertyTypeTypeDef,
     },
 )
-_OptionalAssetModelPropertyOutputTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyOutputTypeDef",
+_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
+    "_OptionalAssetModelPropertyDefinitionTypeDef",
     {
-        "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
-class AssetModelPropertyOutputTypeDef(
-    _RequiredAssetModelPropertyOutputTypeDef, _OptionalAssetModelPropertyOutputTypeDef
+
+class AssetModelPropertyDefinitionTypeDef(
+    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
 ):
     pass
 
+
 _RequiredAssetModelPropertySummaryTypeDef = TypedDict(
     "_RequiredAssetModelPropertySummaryTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
-        "type": PropertyTypeOutputTypeDef,
+        "type": PropertyTypeTypeDef,
     },
 )
 _OptionalAssetModelPropertySummaryTypeDef = TypedDict(
     "_OptionalAssetModelPropertySummaryTypeDef",
     {
         "id": str,
         "dataTypeSpec": str,
         "unit": str,
         "assetModelCompositeModelId": str,
     },
     total=False,
 )
 
+
 class AssetModelPropertySummaryTypeDef(
     _RequiredAssetModelPropertySummaryTypeDef, _OptionalAssetModelPropertySummaryTypeDef
 ):
     pass
 
-_RequiredPropertyTypeDef = TypedDict(
-    "_RequiredPropertyTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "dataType": PropertyDataTypeType,
-    },
-)
-_OptionalPropertyTypeDef = TypedDict(
-    "_OptionalPropertyTypeDef",
-    {
-        "alias": str,
-        "notification": PropertyNotificationTypeDef,
-        "unit": str,
-        "type": PropertyTypeOutputTypeDef,
-    },
-    total=False,
-)
-
-class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
-    pass
-
-_RequiredAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_RequiredAssetModelPropertyDefinitionTypeDef",
-    {
-        "name": str,
-        "dataType": PropertyDataTypeType,
-        "type": PropertyTypeTypeDef,
-    },
-)
-_OptionalAssetModelPropertyDefinitionTypeDef = TypedDict(
-    "_OptionalAssetModelPropertyDefinitionTypeDef",
-    {
-        "dataTypeSpec": str,
-        "unit": str,
-    },
-    total=False,
-)
-
-class AssetModelPropertyDefinitionTypeDef(
-    _RequiredAssetModelPropertyDefinitionTypeDef, _OptionalAssetModelPropertyDefinitionTypeDef
-):
-    pass
 
 _RequiredAssetModelPropertyTypeDef = TypedDict(
     "_RequiredAssetModelPropertyTypeDef",
     {
         "name": str,
         "dataType": PropertyDataTypeType,
         "type": PropertyTypeTypeDef,
@@ -3806,71 +3865,45 @@
         "id": str,
         "dataTypeSpec": str,
         "unit": str,
     },
     total=False,
 )
 
+
 class AssetModelPropertyTypeDef(
     _RequiredAssetModelPropertyTypeDef, _OptionalAssetModelPropertyTypeDef
 ):
     pass
 
-_RequiredAssetModelCompositeModelOutputTypeDef = TypedDict(
-    "_RequiredAssetModelCompositeModelOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-_OptionalAssetModelCompositeModelOutputTypeDef = TypedDict(
-    "_OptionalAssetModelCompositeModelOutputTypeDef",
-    {
-        "description": str,
-        "properties": List[AssetModelPropertyOutputTypeDef],
-        "id": str,
-    },
-    total=False,
-)
-
-class AssetModelCompositeModelOutputTypeDef(
-    _RequiredAssetModelCompositeModelOutputTypeDef, _OptionalAssetModelCompositeModelOutputTypeDef
-):
-    pass
-
-ListAssetModelPropertiesResponseTypeDef = TypedDict(
-    "ListAssetModelPropertiesResponseTypeDef",
-    {
-        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-_RequiredCompositeModelPropertyTypeDef = TypedDict(
-    "_RequiredCompositeModelPropertyTypeDef",
+_RequiredPropertyTypeDef = TypedDict(
+    "_RequiredPropertyTypeDef",
     {
+        "id": str,
         "name": str,
-        "type": str,
-        "assetProperty": PropertyTypeDef,
+        "dataType": PropertyDataTypeType,
     },
 )
-_OptionalCompositeModelPropertyTypeDef = TypedDict(
-    "_OptionalCompositeModelPropertyTypeDef",
+_OptionalPropertyTypeDef = TypedDict(
+    "_OptionalPropertyTypeDef",
     {
-        "id": str,
+        "alias": str,
+        "notification": PropertyNotificationTypeDef,
+        "unit": str,
+        "type": PropertyTypeTypeDef,
     },
     total=False,
 )
 
-class CompositeModelPropertyTypeDef(
-    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
-):
+
+class PropertyTypeDef(_RequiredPropertyTypeDef, _OptionalPropertyTypeDef):
     pass
 
+
 _RequiredAssetModelCompositeModelDefinitionTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
@@ -3879,72 +3912,78 @@
     {
         "description": str,
         "properties": Sequence[AssetModelPropertyDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class AssetModelCompositeModelDefinitionTypeDef(
     _RequiredAssetModelCompositeModelDefinitionTypeDef,
     _OptionalAssetModelCompositeModelDefinitionTypeDef,
 ):
     pass
 
+
+ListAssetModelPropertiesResponseTypeDef = TypedDict(
+    "ListAssetModelPropertiesResponseTypeDef",
+    {
+        "assetModelPropertySummaries": List[AssetModelPropertySummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssetModelCompositeModelTypeDef = TypedDict(
     "_RequiredAssetModelCompositeModelTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 _OptionalAssetModelCompositeModelTypeDef = TypedDict(
     "_OptionalAssetModelCompositeModelTypeDef",
     {
         "description": str,
-        "properties": Sequence[AssetModelPropertyTypeDef],
+        "properties": List[AssetModelPropertyTypeDef],
         "id": str,
     },
     total=False,
 )
 
+
 class AssetModelCompositeModelTypeDef(
     _RequiredAssetModelCompositeModelTypeDef, _OptionalAssetModelCompositeModelTypeDef
 ):
     pass
 
-AssetModelPropertyUnionTypeDef = Union[AssetModelPropertyTypeDef, AssetModelPropertyOutputTypeDef]
-DescribeAssetModelResponseTypeDef = TypedDict(
-    "DescribeAssetModelResponseTypeDef",
+
+_RequiredCompositeModelPropertyTypeDef = TypedDict(
+    "_RequiredCompositeModelPropertyTypeDef",
     {
-        "assetModelId": str,
-        "assetModelArn": str,
-        "assetModelName": str,
-        "assetModelDescription": str,
-        "assetModelProperties": List[AssetModelPropertyOutputTypeDef],
-        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": List[AssetModelCompositeModelOutputTypeDef],
-        "assetModelCreationDate": datetime,
-        "assetModelLastUpdateDate": datetime,
-        "assetModelStatus": AssetModelStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "type": str,
+        "assetProperty": PropertyTypeDef,
     },
 )
-
-DescribeAssetPropertyResponseTypeDef = TypedDict(
-    "DescribeAssetPropertyResponseTypeDef",
+_OptionalCompositeModelPropertyTypeDef = TypedDict(
+    "_OptionalCompositeModelPropertyTypeDef",
     {
-        "assetId": str,
-        "assetName": str,
-        "assetModelId": str,
-        "assetProperty": PropertyTypeDef,
-        "compositeModel": CompositeModelPropertyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
     },
+    total=False,
 )
 
+
+class CompositeModelPropertyTypeDef(
+    _RequiredCompositeModelPropertyTypeDef, _OptionalCompositeModelPropertyTypeDef
+):
+    pass
+
+
 _RequiredCreateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetModelRequestRequestTypeDef",
     {
         "assetModelName": str,
     },
 )
 _OptionalCreateAssetModelRequestRequestTypeDef = TypedDict(
@@ -3956,38 +3995,68 @@
         "assetModelCompositeModels": Sequence[AssetModelCompositeModelDefinitionTypeDef],
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAssetModelRequestRequestTypeDef(
     _RequiredCreateAssetModelRequestRequestTypeDef, _OptionalCreateAssetModelRequestRequestTypeDef
 ):
     pass
 
-AssetModelCompositeModelUnionTypeDef = Union[
-    AssetModelCompositeModelTypeDef, AssetModelCompositeModelOutputTypeDef
-]
+
+DescribeAssetModelResponseTypeDef = TypedDict(
+    "DescribeAssetModelResponseTypeDef",
+    {
+        "assetModelId": str,
+        "assetModelArn": str,
+        "assetModelName": str,
+        "assetModelDescription": str,
+        "assetModelProperties": List[AssetModelPropertyTypeDef],
+        "assetModelHierarchies": List[AssetModelHierarchyTypeDef],
+        "assetModelCompositeModels": List[AssetModelCompositeModelTypeDef],
+        "assetModelCreationDate": datetime,
+        "assetModelLastUpdateDate": datetime,
+        "assetModelStatus": AssetModelStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelId": str,
         "assetModelName": str,
     },
 )
 _OptionalUpdateAssetModelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateAssetModelRequestRequestTypeDef",
     {
         "assetModelDescription": str,
-        "assetModelProperties": Sequence[AssetModelPropertyUnionTypeDef],
+        "assetModelProperties": Sequence[AssetModelPropertyTypeDef],
         "assetModelHierarchies": Sequence[AssetModelHierarchyTypeDef],
-        "assetModelCompositeModels": Sequence[AssetModelCompositeModelUnionTypeDef],
+        "assetModelCompositeModels": Sequence[AssetModelCompositeModelTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateAssetModelRequestRequestTypeDef(
     _RequiredUpdateAssetModelRequestRequestTypeDef, _OptionalUpdateAssetModelRequestRequestTypeDef
 ):
     pass
+
+
+DescribeAssetPropertyResponseTypeDef = TypedDict(
+    "DescribeAssetPropertyResponseTypeDef",
+    {
+        "assetId": str,
+        "assetName": str,
+        "assetModelId": str,
+        "assetProperty": PropertyTypeDef,
+        "compositeModel": CompositeModelPropertyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/waiter.py` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise/waiter.pyi` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post1/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt` & `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

