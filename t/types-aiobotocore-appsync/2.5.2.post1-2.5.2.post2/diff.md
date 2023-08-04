# Comparing `tmp/types-aiobotocore-appsync-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appsync-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appsync-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-appsync-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-appsync-2.5.2.post1.tar` & `types-aiobotocore-appsync-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45944 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45868 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58030 2023-08-02 14:33:29.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57945 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.579117 types-aiobotocore-appsync-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-08-04 12:00:25.579117 types-aiobotocore-appsync-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.579117 types-aiobotocore-appsync-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.579117 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45914 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45838 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-04 11:40:37.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-08-04 11:40:38.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57075 2023-08-04 11:40:38.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:36.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.579117 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:25.000000 types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appsync-2.5.2.post1/LICENSE` & `types-aiobotocore-appsync-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/setup.py` & `types-aiobotocore-appsync-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appsync",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.pyi` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__main__.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppSync 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AppSync 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
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

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     BlobTypeDef,
-    CachingConfigUnionTypeDef,
+    CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -88,15 +88,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigUnionTypeDef,
+    PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -327,17 +327,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigUnionTypeDef = ...,
+        pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigUnionTypeDef = ...,
+        cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -860,17 +860,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigUnionTypeDef = ...,
+        pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigUnionTypeDef = ...,
+        cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.pyi` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     BlobTypeDef,
-    CachingConfigUnionTypeDef,
+    CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -88,15 +88,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigUnionTypeDef,
+    PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -311,17 +311,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigUnionTypeDef = ...,
+        pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigUnionTypeDef = ...,
+        cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -795,17 +795,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigUnionTypeDef = ...,
+        pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigUnionTypeDef = ...,
+        cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.pyi` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.pyi` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.py` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "BlobTypeDef",
-    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -114,15 +113,14 @@
     "ListResolversByFunctionRequestRequestTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
@@ -146,15 +144,14 @@
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
-    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -168,15 +165,14 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
-    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -355,35 +351,14 @@
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredCachingConfigOutputTypeDef = TypedDict(
-    "_RequiredCachingConfigOutputTypeDef",
-    {
-        "ttl": int,
-    },
-)
-_OptionalCachingConfigOutputTypeDef = TypedDict(
-    "_OptionalCachingConfigOutputTypeDef",
-    {
-        "cachingKeys": List[str],
-    },
-    total=False,
-)
-
-
-class CachingConfigOutputTypeDef(
-    _RequiredCachingConfigOutputTypeDef, _OptionalCachingConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredCachingConfigTypeDef = TypedDict(
     "_RequiredCachingConfigTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigTypeDef = TypedDict(
@@ -1047,22 +1022,14 @@
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
 
-PipelineConfigOutputTypeDef = TypedDict(
-    "PipelineConfigOutputTypeDef",
-    {
-        "functions": List[str],
-    },
-    total=False,
-)
-
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
         "awsRegion": str,
         "dbClusterIdentifier": str,
         "databaseName": str,
         "schema": str,
@@ -1443,15 +1410,14 @@
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": BlobTypeDef,
     },
 )
 
-CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
@@ -1727,15 +1693,14 @@
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1966,17 +1931,17 @@
         "typeName": str,
         "fieldName": str,
         "dataSourceName": str,
         "resolverArn": str,
         "requestMappingTemplate": str,
         "responseMappingTemplate": str,
         "kind": ResolverKindType,
-        "pipelineConfig": PipelineConfigOutputTypeDef,
+        "pipelineConfig": PipelineConfigTypeDef,
         "syncConfig": SyncConfigTypeDef,
-        "cachingConfig": CachingConfigOutputTypeDef,
+        "cachingConfig": CachingConfigTypeDef,
         "maxBatchSize": int,
         "runtime": AppSyncRuntimeTypeDef,
         "code": str,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.pyi` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "BlobTypeDef",
-    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -113,15 +112,14 @@
     "ListResolversByFunctionRequestRequestTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
@@ -145,15 +143,14 @@
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
-    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -167,15 +164,14 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
-    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -348,33 +344,14 @@
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredCachingConfigOutputTypeDef = TypedDict(
-    "_RequiredCachingConfigOutputTypeDef",
-    {
-        "ttl": int,
-    },
-)
-_OptionalCachingConfigOutputTypeDef = TypedDict(
-    "_OptionalCachingConfigOutputTypeDef",
-    {
-        "cachingKeys": List[str],
-    },
-    total=False,
-)
-
-class CachingConfigOutputTypeDef(
-    _RequiredCachingConfigOutputTypeDef, _OptionalCachingConfigOutputTypeDef
-):
-    pass
-
 _RequiredCachingConfigTypeDef = TypedDict(
     "_RequiredCachingConfigTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigTypeDef = TypedDict(
@@ -1008,22 +985,14 @@
 )
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
-PipelineConfigOutputTypeDef = TypedDict(
-    "PipelineConfigOutputTypeDef",
-    {
-        "functions": List[str],
-    },
-    total=False,
-)
-
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
         "awsRegion": str,
         "dbClusterIdentifier": str,
         "databaseName": str,
         "schema": str,
@@ -1388,15 +1357,14 @@
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": BlobTypeDef,
     },
 )
 
-CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
@@ -1658,15 +1626,14 @@
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1889,17 +1856,17 @@
         "typeName": str,
         "fieldName": str,
         "dataSourceName": str,
         "resolverArn": str,
         "requestMappingTemplate": str,
         "responseMappingTemplate": str,
         "kind": ResolverKindType,
-        "pipelineConfig": PipelineConfigOutputTypeDef,
+        "pipelineConfig": PipelineConfigTypeDef,
         "syncConfig": SyncConfigTypeDef,
-        "cachingConfig": CachingConfigOutputTypeDef,
+        "cachingConfig": CachingConfigTypeDef,
         "maxBatchSize": int,
         "runtime": AppSyncRuntimeTypeDef,
         "code": str,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/SOURCES.txt` & `types-aiobotocore-appsync-2.5.2.post2/types_aiobotocore_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

