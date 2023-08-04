# Comparing `tmp/types-aiobotocore-kendra-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kendra-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kendra-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-kendra-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-kendra-2.5.2.post1.tar` & `types-aiobotocore-kendra-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.757553 types-aiobotocore-kendra-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26422 2023-08-02 14:52:29.757553 types-aiobotocore-kendra-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24908 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:29.757553 types-aiobotocore-kendra-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:41:18.000000 types-aiobotocore-kendra-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.753553 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50713 2023-08-02 14:41:21.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50639 2023-08-02 14:41:21.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-08-02 14:41:21.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-08-02 14:41:21.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   145516 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   145305 2023-08-02 14:41:22.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:19.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.757553 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26422 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:29.000000 types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12213 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10699 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.426643 types-aiobotocore-kendra-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      434 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      433 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50591 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50517 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15441 2023-08-04 13:41:49.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15439 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   110892 2023-08-04 13:41:52.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   110739 2023-08-04 13:41:50.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12213 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      717 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kendra-2.5.2.post1/LICENSE` & `types-aiobotocore-kendra-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post1/setup.py` & `types-aiobotocore-kendra-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kendra",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.kendra 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/__main__.py` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.kendra 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.kendra 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/client.py` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,44 +48,44 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
-    CustomDocumentEnrichmentConfigurationUnionTypeDef,
-    DataSourceConfigurationUnionTypeDef,
+    CustomDocumentEnrichmentConfigurationTypeDef,
+    DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
-    DataSourceVpcConfigurationUnionTypeDef,
+    DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
-    DocumentMetadataConfigurationUnionTypeDef,
+    DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
-    ExperienceConfigurationUnionTypeDef,
+    ExperienceConfigurationTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
-    HierarchicalPrincipalUnionTypeDef,
+    HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
@@ -101,15 +101,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
@@ -216,15 +216,15 @@
 
     async def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_put_document)
         """
@@ -256,15 +256,15 @@
     async def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...,
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_access_control_configuration)
@@ -272,23 +272,23 @@
 
     async def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: DataSourceConfigurationUnionTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
+        Configuration: DataSourceConfigurationTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_data_source)
@@ -296,15 +296,15 @@
 
     async def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationUnionTypeDef = ...,
+        Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -659,15 +659,15 @@
     async def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: TimeRangeUnionTypeDef = ...,
+        StartTimeFilter: TimeRangeTypeDef = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#list_data_source_sync_jobs)
@@ -913,36 +913,36 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_access_control_configuration)
         """
 
     async def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: DataSourceConfigurationUnionTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
+        Configuration: DataSourceConfigurationTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_data_source)
         """
@@ -950,15 +950,15 @@
     async def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationUnionTypeDef = ...,
+        Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_experience)
@@ -985,17 +985,15 @@
     async def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        DocumentMetadataConfigurationUpdates: Sequence[
-            DocumentMetadataConfigurationUnionTypeDef
-        ] = ...,
+        DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
```

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/client.pyi` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,44 +48,44 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
-    CustomDocumentEnrichmentConfigurationUnionTypeDef,
-    DataSourceConfigurationUnionTypeDef,
+    CustomDocumentEnrichmentConfigurationTypeDef,
+    DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
-    DataSourceVpcConfigurationUnionTypeDef,
+    DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
-    DocumentMetadataConfigurationUnionTypeDef,
+    DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
-    ExperienceConfigurationUnionTypeDef,
+    ExperienceConfigurationTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
-    HierarchicalPrincipalUnionTypeDef,
+    HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
@@ -101,15 +101,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
@@ -207,15 +207,15 @@
         """
     async def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#batch_put_document)
         """
@@ -243,53 +243,53 @@
     async def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...,
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_access_control_configuration)
         """
     async def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: DataSourceConfigurationUnionTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
+        Configuration: DataSourceConfigurationTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#create_data_source)
         """
     async def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationUnionTypeDef = ...,
+        Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -614,15 +614,15 @@
     async def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: TimeRangeUnionTypeDef = ...,
+        StartTimeFilter: TimeRangeTypeDef = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#list_data_source_sync_jobs)
@@ -848,50 +848,50 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_access_control_configuration)
         """
     async def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: DataSourceConfigurationUnionTypeDef = ...,
-        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
+        Configuration: DataSourceConfigurationTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_data_source)
         """
     async def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: ExperienceConfigurationUnionTypeDef = ...,
+        Configuration: ExperienceConfigurationTypeDef = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/client/#update_experience)
@@ -916,17 +916,15 @@
     async def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        DocumentMetadataConfigurationUpdates: Sequence[
-            DocumentMetadataConfigurationUnionTypeDef
-        ] = ...,
+        DocumentMetadataConfigurationUpdates: Sequence[DocumentMetadataConfigurationTypeDef] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
```

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/literals.py` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,15 @@
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
@@ -385,14 +386,15 @@
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
@@ -471,26 +473,28 @@
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

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/literals.pyi` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
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
@@ -383,14 +384,15 @@
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
@@ -469,26 +471,28 @@
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

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/type_defs.py` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,17 +88,16 @@
 
 
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
     "AccessControlListConfigurationTypeDef",
     "AclConfigurationTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
-    "DataSourceVpcConfigurationOutputTypeDef",
-    "S3PathTypeDef",
     "DataSourceVpcConfigurationTypeDef",
+    "S3PathTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
     "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
     "SuggestableConfigTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
@@ -114,23 +113,21 @@
     "TimestampTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
-    "ContentSourceConfigurationOutputTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
     "TagTypeDef",
     "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
-    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -151,28 +148,26 @@
     "DescribeIndexRequestRequestTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
-    "DocumentAttributeValueOutputTypeDef",
-    "RelevanceOutputTypeDef",
-    "SearchTypeDef",
     "RelevanceTypeDef",
+    "SearchTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
     "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
-    "TimeRangeOutputTypeDef",
+    "TimeRangeTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
@@ -195,61 +190,41 @@
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
-    "SeedUrlConfigurationOutputTypeDef",
     "SeedUrlConfigurationTypeDef",
-    "SiteMapsConfigurationOutputTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
-    "GoogleDriveConfigurationOutputTypeDef",
     "GoogleDriveConfigurationTypeDef",
-    "SalesforceChatterFeedConfigurationOutputTypeDef",
     "SalesforceChatterFeedConfigurationTypeDef",
-    "SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    "SalesforceStandardObjectConfigurationOutputTypeDef",
     "SalesforceStandardObjectConfigurationTypeDef",
-    "ServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     "ServiceNowKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowServiceCatalogConfigurationOutputTypeDef",
     "ServiceNowServiceCatalogConfigurationTypeDef",
-    "WorkDocsConfigurationOutputTypeDef",
     "WorkDocsConfigurationTypeDef",
-    "BoxConfigurationOutputTypeDef",
-    "FsxConfigurationOutputTypeDef",
-    "JiraConfigurationOutputTypeDef",
-    "QuipConfigurationOutputTypeDef",
-    "SlackConfigurationOutputTypeDef",
-    "AlfrescoConfigurationOutputTypeDef",
-    "OnPremiseConfigurationTypeDef",
-    "OneDriveUsersOutputTypeDef",
-    "OneDriveUsersTypeDef",
-    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
-    "UpdateThesaurusRequestRequestTypeDef",
-    "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
-    "DataSourceVpcConfigurationUnionTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
+    "AlfrescoConfigurationTypeDef",
+    "OnPremiseConfigurationTypeDef",
+    "OneDriveUsersTypeDef",
+    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+    "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
     "CreateAccessControlConfigurationResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
     "CreateExperienceResponseTypeDef",
@@ -264,36 +239,28 @@
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAccessControlConfigurationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     "AttributeSuggestionsDescribeConfigTypeDef",
     "AttributeSuggestionsUpdateConfigTypeDef",
-    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "ClickFeedbackTypeDef",
     "DocumentAttributeValueTypeDef",
-    "TimeRangeTypeDef",
-    "ConfluenceAttachmentConfigurationOutputTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
-    "ConfluenceBlogConfigurationOutputTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
-    "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
-    "ConfluencePageConfigurationOutputTypeDef",
     "ConfluencePageConfigurationTypeDef",
-    "ConfluenceSpaceConfigurationOutputTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
-    "HierarchicalPrincipalOutputTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFeaturedResultsSetRequestRequestTypeDef",
@@ -301,117 +268,92 @@
     "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
-    "DocumentAttributeConditionOutputTypeDef",
-    "DocumentAttributeOutputTypeDef",
-    "DocumentAttributeTargetOutputTypeDef",
-    "DocumentAttributeValueCountPairTypeDef",
-    "DocumentMetadataConfigurationOutputTypeDef",
-    "DocumentMetadataConfigurationTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
-    "S3DataSourceConfigurationOutputTypeDef",
+    "DocumentMetadataConfigurationTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
-    "ExperienceConfigurationOutputTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
     "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
+    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
     "UserTokenConfigurationTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     "ListThesauriResponseTypeDef",
-    "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
-    "DatabaseConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
-    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowConfigurationOutputTypeDef",
     "ServiceNowConfigurationTypeDef",
-    "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
-    "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
-    "ListDataSourceSyncJobsRequestRequestTypeDef",
-    "TimeRangeUnionTypeDef",
-    "ConfluenceConfigurationOutputTypeDef",
+    "DocumentAttributeValueCountPairTypeDef",
     "ConfluenceConfigurationTypeDef",
+    "CreateAccessControlConfigurationRequestRequestTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
-    "HierarchicalPrincipalUnionTypeDef",
+    "UpdateAccessControlConfigurationRequestRequestTypeDef",
     "CreateFeaturedResultsSetResponseTypeDef",
     "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
-    "HookConfigurationOutputTypeDef",
-    "RetrieveResultItemTypeDef",
-    "SourceDocumentTypeDef",
-    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "DocumentMetadataConfigurationUnionTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
-    "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
-    "ExperienceConfigurationUnionTypeDef",
+    "DescribeExperienceResponseTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
-    "WebCrawlerConfigurationOutputTypeDef",
+    "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
-    "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "DocumentInfoTypeDef",
     "DocumentTypeDef",
-    "CreateAccessControlConfigurationRequestRequestTypeDef",
-    "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "RetrieveResultItemTypeDef",
+    "SourceDocumentTypeDef",
     "GetQuerySuggestionsRequestRequestTypeDef",
-    "RetrieveResultTypeDef",
-    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "UpdateIndexRequestRequestTypeDef",
     "AdditionalResultAttributeTypeDef",
-    "SuggestionTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "CustomDocumentEnrichmentConfigurationTypeDef",
     "BatchGetDocumentStatusRequestRequestTypeDef",
+    "RetrieveResultTypeDef",
+    "SuggestionTypeDef",
     "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
-    "GetQuerySuggestionsResponseTypeDef",
-    "DescribeDataSourceResponseTypeDef",
-    "DataSourceConfigurationUnionTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
-    "CustomDocumentEnrichmentConfigurationUnionTypeDef",
+    "DescribeDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
+    "GetQuerySuggestionsResponseTypeDef",
     "QueryResultTypeDef",
 )
 
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
         "Id": str,
@@ -451,38 +393,30 @@
 
 class DataSourceToIndexFieldMappingTypeDef(
     _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
 ):
     pass
 
 
-DataSourceVpcConfigurationOutputTypeDef = TypedDict(
-    "DataSourceVpcConfigurationOutputTypeDef",
+DataSourceVpcConfigurationTypeDef = TypedDict(
+    "DataSourceVpcConfigurationTypeDef",
     {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
     },
 )
 
 S3PathTypeDef = TypedDict(
     "S3PathTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-DataSourceVpcConfigurationTypeDef = TypedDict(
-    "DataSourceVpcConfigurationTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-)
-
 EntityConfigurationTypeDef = TypedDict(
     "EntityConfigurationTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
     },
 )
@@ -698,24 +632,14 @@
         "DatabasePort": int,
         "DatabaseName": str,
         "TableName": str,
         "SecretArn": str,
     },
 )
 
-ContentSourceConfigurationOutputTypeDef = TypedDict(
-    "ContentSourceConfigurationOutputTypeDef",
-    {
-        "DataSourceIds": List[str],
-        "FaqIds": List[str],
-        "DirectPutContent": bool,
-    },
-    total=False,
-)
-
 ContentSourceConfigurationTypeDef = TypedDict(
     "ContentSourceConfigurationTypeDef",
     {
         "DataSourceIds": Sequence[str],
         "FaqIds": Sequence[str],
         "DirectPutContent": bool,
     },
@@ -781,22 +705,14 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
-TemplateConfigurationOutputTypeDef = TypedDict(
-    "TemplateConfigurationOutputTypeDef",
-    {
-        "Template": Dict[str, Any],
-    },
-    total=False,
-)
-
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "Template": Mapping[str, Any],
     },
     total=False,
 )
@@ -1059,27 +975,16 @@
     {
         "Id": str,
         "IndexId": str,
         "EntityIds": Sequence[str],
     },
 )
 
-DocumentAttributeValueOutputTypeDef = TypedDict(
-    "DocumentAttributeValueOutputTypeDef",
-    {
-        "StringValue": str,
-        "StringListValue": List[str],
-        "LongValue": int,
-        "DateValue": datetime,
-    },
-    total=False,
-)
-
-RelevanceOutputTypeDef = TypedDict(
-    "RelevanceOutputTypeDef",
+RelevanceTypeDef = TypedDict(
+    "RelevanceTypeDef",
     {
         "Freshness": bool,
         "Importance": int,
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Dict[str, int],
     },
@@ -1093,26 +998,14 @@
         "Searchable": bool,
         "Displayable": bool,
         "Sortable": bool,
     },
     total=False,
 )
 
-RelevanceTypeDef = TypedDict(
-    "RelevanceTypeDef",
-    {
-        "Freshness": bool,
-        "Importance": int,
-        "Duration": str,
-        "RankOrder": OrderType,
-        "ValueImportanceMap": Mapping[str, int],
-    },
-    total=False,
-)
-
 DocumentsMetadataConfigurationTypeDef = TypedDict(
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
     },
     total=False,
 )
@@ -1210,16 +1103,16 @@
 
 class GetSnapshotsRequestRequestTypeDef(
     _RequiredGetSnapshotsRequestRequestTypeDef, _OptionalGetSnapshotsRequestRequestTypeDef
 ):
     pass
 
 
-TimeRangeOutputTypeDef = TypedDict(
-    "TimeRangeOutputTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
@@ -1685,35 +1578,14 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
     },
 )
 
-_RequiredSeedUrlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSeedUrlConfigurationOutputTypeDef",
-    {
-        "SeedUrls": List[str],
-    },
-)
-_OptionalSeedUrlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSeedUrlConfigurationOutputTypeDef",
-    {
-        "WebCrawlerMode": WebCrawlerModeType,
-    },
-    total=False,
-)
-
-
-class SeedUrlConfigurationOutputTypeDef(
-    _RequiredSeedUrlConfigurationOutputTypeDef, _OptionalSeedUrlConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
@@ -1727,21 +1599,14 @@
 
 class SeedUrlConfigurationTypeDef(
     _RequiredSeedUrlConfigurationTypeDef, _OptionalSeedUrlConfigurationTypeDef
 ):
     pass
 
 
-SiteMapsConfigurationOutputTypeDef = TypedDict(
-    "SiteMapsConfigurationOutputTypeDef",
-    {
-        "SiteMaps": List[str],
-    },
-)
-
 SiteMapsConfigurationTypeDef = TypedDict(
     "SiteMapsConfigurationTypeDef",
     {
         "SiteMaps": Sequence[str],
     },
 )
 
@@ -1785,38 +1650,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredColumnConfigurationOutputTypeDef = TypedDict(
-    "_RequiredColumnConfigurationOutputTypeDef",
-    {
-        "DocumentIdColumnName": str,
-        "DocumentDataColumnName": str,
-        "ChangeDetectingColumns": List[str],
-    },
-)
-_OptionalColumnConfigurationOutputTypeDef = TypedDict(
-    "_OptionalColumnConfigurationOutputTypeDef",
-    {
-        "DocumentTitleColumnName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class ColumnConfigurationOutputTypeDef(
-    _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": Sequence[str],
     },
@@ -1833,40 +1674,14 @@
 
 class ColumnConfigurationTypeDef(
     _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
 ):
     pass
 
 
-_RequiredGoogleDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGoogleDriveConfigurationOutputTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGoogleDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGoogleDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "ExcludeMimeTypes": List[str],
-        "ExcludeUserAccounts": List[str],
-        "ExcludeSharedDrives": List[str],
-    },
-    total=False,
-)
-
-
-class GoogleDriveConfigurationOutputTypeDef(
-    _RequiredGoogleDriveConfigurationOutputTypeDef, _OptionalGoogleDriveConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredGoogleDriveConfigurationTypeDef = TypedDict(
     "_RequiredGoogleDriveConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGoogleDriveConfigurationTypeDef = TypedDict(
@@ -1885,38 +1700,14 @@
 
 class GoogleDriveConfigurationTypeDef(
     _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
 ):
     pass
 
 
-_RequiredSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceChatterFeedConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceChatterFeedConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "IncludeFilterTypes": List[SalesforceChatterFeedIncludeFilterTypeType],
-    },
-    total=False,
-)
-
-
-class SalesforceChatterFeedConfigurationOutputTypeDef(
-    _RequiredSalesforceChatterFeedConfigurationOutputTypeDef,
-    _OptionalSalesforceChatterFeedConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceChatterFeedConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
@@ -1933,38 +1724,14 @@
 class SalesforceChatterFeedConfigurationTypeDef(
     _RequiredSalesforceChatterFeedConfigurationTypeDef,
     _OptionalSalesforceChatterFeedConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(
-    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
-    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     {
         "Name": str,
         "DocumentDataFieldName": str,
     },
 )
@@ -1981,37 +1748,14 @@
 class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(
-    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
-    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
@@ -2027,56 +1771,23 @@
 class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
 
-SalesforceStandardObjectAttachmentConfigurationOutputTypeDef = TypedDict(
-    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-_RequiredSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceStandardObjectConfigurationOutputTypeDef",
-    {
-        "Name": SalesforceStandardObjectNameType,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceStandardObjectConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SalesforceStandardObjectConfigurationOutputTypeDef(
-    _RequiredSalesforceStandardObjectConfigurationOutputTypeDef,
-    _OptionalSalesforceStandardObjectConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceStandardObjectConfigurationTypeDef",
     {
         "Name": SalesforceStandardObjectNameType,
         "DocumentDataFieldName": str,
     },
 )
@@ -2093,41 +1804,14 @@
 class SalesforceStandardObjectConfigurationTypeDef(
     _RequiredSalesforceStandardObjectConfigurationTypeDef,
     _OptionalSalesforceStandardObjectConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "FilterQuery": str,
-    },
-    total=False,
-)
-
-
-class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(
-    _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-    _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -2147,40 +1831,14 @@
 class ServiceNowKnowledgeArticleConfigurationTypeDef(
     _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
     _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class ServiceNowServiceCatalogConfigurationOutputTypeDef(
-    _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef,
-    _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
@@ -2199,39 +1857,14 @@
 class ServiceNowServiceCatalogConfigurationTypeDef(
     _RequiredServiceNowServiceCatalogConfigurationTypeDef,
     _OptionalServiceNowServiceCatalogConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredWorkDocsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredWorkDocsConfigurationOutputTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalWorkDocsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalWorkDocsConfigurationOutputTypeDef",
-    {
-        "CrawlComments": bool,
-        "UseChangeLog": bool,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class WorkDocsConfigurationOutputTypeDef(
-    _RequiredWorkDocsConfigurationOutputTypeDef, _OptionalWorkDocsConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredWorkDocsConfigurationTypeDef = TypedDict(
     "_RequiredWorkDocsConfigurationTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalWorkDocsConfigurationTypeDef = TypedDict(
@@ -2249,220 +1882,207 @@
 
 class WorkDocsConfigurationTypeDef(
     _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
 ):
     pass
 
 
-_RequiredBoxConfigurationOutputTypeDef = TypedDict(
-    "_RequiredBoxConfigurationOutputTypeDef",
+_RequiredBoxConfigurationTypeDef = TypedDict(
+    "_RequiredBoxConfigurationTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
-_OptionalBoxConfigurationOutputTypeDef = TypedDict(
-    "_OptionalBoxConfigurationOutputTypeDef",
+_OptionalBoxConfigurationTypeDef = TypedDict(
+    "_OptionalBoxConfigurationTypeDef",
     {
         "UseChangeLog": bool,
         "CrawlComments": bool,
         "CrawlTasks": bool,
         "CrawlWebLinks": bool,
-        "FileFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "TaskFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "FileFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "TaskFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WebLinkFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class BoxConfigurationOutputTypeDef(
-    _RequiredBoxConfigurationOutputTypeDef, _OptionalBoxConfigurationOutputTypeDef
-):
+class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
 
-_RequiredFsxConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFsxConfigurationOutputTypeDef",
+_RequiredFsxConfigurationTypeDef = TypedDict(
+    "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
 )
-_OptionalFsxConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFsxConfigurationOutputTypeDef",
+_OptionalFsxConfigurationTypeDef = TypedDict(
+    "_OptionalFsxConfigurationTypeDef",
     {
         "SecretArn": str,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 
-class FsxConfigurationOutputTypeDef(
-    _RequiredFsxConfigurationOutputTypeDef, _OptionalFsxConfigurationOutputTypeDef
-):
+class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
     pass
 
 
-_RequiredJiraConfigurationOutputTypeDef = TypedDict(
-    "_RequiredJiraConfigurationOutputTypeDef",
+_RequiredJiraConfigurationTypeDef = TypedDict(
+    "_RequiredJiraConfigurationTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
-_OptionalJiraConfigurationOutputTypeDef = TypedDict(
-    "_OptionalJiraConfigurationOutputTypeDef",
+_OptionalJiraConfigurationTypeDef = TypedDict(
+    "_OptionalJiraConfigurationTypeDef",
     {
         "UseChangeLog": bool,
-        "Project": List[str],
-        "IssueType": List[str],
-        "Status": List[str],
-        "IssueSubEntityFilter": List[IssueSubEntityType],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "IssueFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "Project": Sequence[str],
+        "IssueType": Sequence[str],
+        "Status": Sequence[str],
+        "IssueSubEntityFilter": Sequence[IssueSubEntityType],
+        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "IssueFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "ProjectFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WorkLogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class JiraConfigurationOutputTypeDef(
-    _RequiredJiraConfigurationOutputTypeDef, _OptionalJiraConfigurationOutputTypeDef
+class JiraConfigurationTypeDef(
+    _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
 ):
     pass
 
 
-_RequiredQuipConfigurationOutputTypeDef = TypedDict(
-    "_RequiredQuipConfigurationOutputTypeDef",
+_RequiredQuipConfigurationTypeDef = TypedDict(
+    "_RequiredQuipConfigurationTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
-_OptionalQuipConfigurationOutputTypeDef = TypedDict(
-    "_OptionalQuipConfigurationOutputTypeDef",
+_OptionalQuipConfigurationTypeDef = TypedDict(
+    "_OptionalQuipConfigurationTypeDef",
     {
         "CrawlFileComments": bool,
         "CrawlChatRooms": bool,
         "CrawlAttachments": bool,
-        "FolderIds": List[str],
-        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "MessageFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "FolderIds": Sequence[str],
+        "ThreadFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "MessageFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class QuipConfigurationOutputTypeDef(
-    _RequiredQuipConfigurationOutputTypeDef, _OptionalQuipConfigurationOutputTypeDef
+class QuipConfigurationTypeDef(
+    _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
 ):
     pass
 
 
-_RequiredSlackConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSlackConfigurationOutputTypeDef",
+_RequiredSlackConfigurationTypeDef = TypedDict(
+    "_RequiredSlackConfigurationTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
-        "SlackEntityList": List[SlackEntityType],
+        "SlackEntityList": Sequence[SlackEntityType],
         "SinceCrawlDate": str,
     },
 )
-_OptionalSlackConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSlackConfigurationOutputTypeDef",
+_OptionalSlackConfigurationTypeDef = TypedDict(
+    "_OptionalSlackConfigurationTypeDef",
     {
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
         "UseChangeLog": bool,
         "CrawlBotMessage": bool,
         "ExcludeArchived": bool,
         "LookBackPeriod": int,
-        "PrivateChannelFilter": List[str],
-        "PublicChannelFilter": List[str],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "PrivateChannelFilter": Sequence[str],
+        "PublicChannelFilter": Sequence[str],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
 
-class SlackConfigurationOutputTypeDef(
-    _RequiredSlackConfigurationOutputTypeDef, _OptionalSlackConfigurationOutputTypeDef
+class SlackConfigurationTypeDef(
+    _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
 ):
     pass
 
 
-_RequiredAlfrescoConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationOutputTypeDef",
+_RequiredAlfrescoConfigurationTypeDef = TypedDict(
+    "_RequiredAlfrescoConfigurationTypeDef",
     {
         "SiteUrl": str,
         "SiteId": str,
         "SecretArn": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
 )
-_OptionalAlfrescoConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationOutputTypeDef",
+_OptionalAlfrescoConfigurationTypeDef = TypedDict(
+    "_OptionalAlfrescoConfigurationTypeDef",
     {
         "CrawlSystemFolders": bool,
         "CrawlComments": bool,
-        "EntityFilter": List[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "EntityFilter": Sequence[AlfrescoEntityType],
+        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class AlfrescoConfigurationOutputTypeDef(
-    _RequiredAlfrescoConfigurationOutputTypeDef, _OptionalAlfrescoConfigurationOutputTypeDef
+class AlfrescoConfigurationTypeDef(
+    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
 
 OnPremiseConfigurationTypeDef = TypedDict(
     "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 
-OneDriveUsersOutputTypeDef = TypedDict(
-    "OneDriveUsersOutputTypeDef",
-    {
-        "OneDriveUserList": List[str],
-        "OneDriveUserS3Path": S3PathTypeDef,
-    },
-    total=False,
-)
-
 OneDriveUsersTypeDef = TypedDict(
     "OneDriveUsersTypeDef",
     {
         "OneDriveUserList": Sequence[str],
         "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
@@ -2515,201 +2135,14 @@
 
 class UpdateThesaurusRequestRequestTypeDef(
     _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAlfrescoConfigurationTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationTypeDef",
-    {
-        "SiteUrl": str,
-        "SiteId": str,
-        "SecretArn": str,
-        "SslCertificateS3Path": S3PathTypeDef,
-    },
-)
-_OptionalAlfrescoConfigurationTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationTypeDef",
-    {
-        "CrawlSystemFolders": bool,
-        "CrawlComments": bool,
-        "EntityFilter": Sequence[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class AlfrescoConfigurationTypeDef(
-    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
-):
-    pass
-
-
-_RequiredBoxConfigurationTypeDef = TypedDict(
-    "_RequiredBoxConfigurationTypeDef",
-    {
-        "EnterpriseId": str,
-        "SecretArn": str,
-    },
-)
-_OptionalBoxConfigurationTypeDef = TypedDict(
-    "_OptionalBoxConfigurationTypeDef",
-    {
-        "UseChangeLog": bool,
-        "CrawlComments": bool,
-        "CrawlTasks": bool,
-        "CrawlWebLinks": bool,
-        "FileFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "TaskFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WebLinkFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
-    pass
-
-
-DataSourceVpcConfigurationUnionTypeDef = Union[
-    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-]
-_RequiredFsxConfigurationTypeDef = TypedDict(
-    "_RequiredFsxConfigurationTypeDef",
-    {
-        "FileSystemId": str,
-        "FileSystemType": Literal["WINDOWS"],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-)
-_OptionalFsxConfigurationTypeDef = TypedDict(
-    "_OptionalFsxConfigurationTypeDef",
-    {
-        "SecretArn": str,
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
-    pass
-
-
-_RequiredJiraConfigurationTypeDef = TypedDict(
-    "_RequiredJiraConfigurationTypeDef",
-    {
-        "JiraAccountUrl": str,
-        "SecretArn": str,
-    },
-)
-_OptionalJiraConfigurationTypeDef = TypedDict(
-    "_OptionalJiraConfigurationTypeDef",
-    {
-        "UseChangeLog": bool,
-        "Project": Sequence[str],
-        "IssueType": Sequence[str],
-        "Status": Sequence[str],
-        "IssueSubEntityFilter": Sequence[IssueSubEntityType],
-        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "IssueFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "ProjectFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WorkLogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class JiraConfigurationTypeDef(
-    _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
-):
-    pass
-
-
-_RequiredQuipConfigurationTypeDef = TypedDict(
-    "_RequiredQuipConfigurationTypeDef",
-    {
-        "Domain": str,
-        "SecretArn": str,
-    },
-)
-_OptionalQuipConfigurationTypeDef = TypedDict(
-    "_OptionalQuipConfigurationTypeDef",
-    {
-        "CrawlFileComments": bool,
-        "CrawlChatRooms": bool,
-        "CrawlAttachments": bool,
-        "FolderIds": Sequence[str],
-        "ThreadFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "MessageFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class QuipConfigurationTypeDef(
-    _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
-):
-    pass
-
-
-_RequiredSlackConfigurationTypeDef = TypedDict(
-    "_RequiredSlackConfigurationTypeDef",
-    {
-        "TeamId": str,
-        "SecretArn": str,
-        "SlackEntityList": Sequence[SlackEntityType],
-        "SinceCrawlDate": str,
-    },
-)
-_OptionalSlackConfigurationTypeDef = TypedDict(
-    "_OptionalSlackConfigurationTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "UseChangeLog": bool,
-        "CrawlBotMessage": bool,
-        "ExcludeArchived": bool,
-        "LookBackPeriod": int,
-        "PrivateChannelFilter": Sequence[str],
-        "PublicChannelFilter": Sequence[str],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class SlackConfigurationTypeDef(
-    _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
-):
-    pass
-
-
 AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
         "EntityList": Sequence[EntityConfigurationTypeDef],
     },
@@ -2917,22 +2350,14 @@
     {
         "SuggestableConfigList": Sequence[SuggestableConfigTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
-AuthenticationConfigurationOutputTypeDef = TypedDict(
-    "AuthenticationConfigurationOutputTypeDef",
-    {
-        "BasicAuthentication": List[BasicAuthenticationConfigurationTypeDef],
-    },
-    total=False,
-)
-
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "BasicAuthentication": Sequence[BasicAuthenticationConfigurationTypeDef],
     },
     total=False,
 )
@@ -3008,90 +2433,31 @@
         "StringListValue": Sequence[str],
         "LongValue": int,
         "DateValue": TimestampTypeDef,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceAttachmentConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
         "CrawlAttachments": bool,
         "AttachmentFieldMappings": Sequence[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-ConfluenceBlogConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceBlogConfigurationOutputTypeDef",
-    {
-        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceBlogConfigurationTypeDef = TypedDict(
     "ConfluenceBlogConfigurationTypeDef",
     {
         "BlogFieldMappings": Sequence[ConfluenceBlogToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-_RequiredSharePointConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSharePointConfigurationOutputTypeDef",
-    {
-        "SharePointVersion": SharePointVersionType,
-        "Urls": List[str],
-        "SecretArn": str,
-    },
-)
-_OptionalSharePointConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSharePointConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "UseChangeLog": bool,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "DocumentTitleFieldName": str,
-        "DisableLocalGroups": bool,
-        "SslCertificateS3Path": S3PathTypeDef,
-        "AuthenticationType": SharePointOnlineAuthenticationTypeType,
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SharePointConfigurationOutputTypeDef(
-    _RequiredSharePointConfigurationOutputTypeDef, _OptionalSharePointConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSharePointConfigurationTypeDef = TypedDict(
     "_RequiredSharePointConfigurationTypeDef",
     {
         "SharePointVersion": SharePointVersionType,
         "Urls": Sequence[str],
         "SecretArn": str,
     },
@@ -3117,42 +2483,22 @@
 
 class SharePointConfigurationTypeDef(
     _RequiredSharePointConfigurationTypeDef, _OptionalSharePointConfigurationTypeDef
 ):
     pass
 
 
-ConfluencePageConfigurationOutputTypeDef = TypedDict(
-    "ConfluencePageConfigurationOutputTypeDef",
-    {
-        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluencePageConfigurationTypeDef = TypedDict(
     "ConfluencePageConfigurationTypeDef",
     {
         "PageFieldMappings": Sequence[ConfluencePageToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-ConfluenceSpaceConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceSpaceConfigurationOutputTypeDef",
-    {
-        "CrawlPersonalSpaces": bool,
-        "CrawlArchivedSpaces": bool,
-        "IncludeSpaces": List[str],
-        "ExcludeSpaces": List[str],
-        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceSpaceConfigurationTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationTypeDef",
     {
         "CrawlPersonalSpaces": bool,
         "CrawlArchivedSpaces": bool,
         "IncludeSpaces": Sequence[str],
         "ExcludeSpaces": Sequence[str],
@@ -3166,21 +2512,14 @@
     {
         "SuggestedQueryText": str,
         "Corrections": List[CorrectionTypeDef],
     },
     total=False,
 )
 
-HierarchicalPrincipalOutputTypeDef = TypedDict(
-    "HierarchicalPrincipalOutputTypeDef",
-    {
-        "PrincipalList": List[PrincipalTypeDef],
-    },
-)
-
 HierarchicalPrincipalTypeDef = TypedDict(
     "HierarchicalPrincipalTypeDef",
     {
         "PrincipalList": Sequence[PrincipalTypeDef],
     },
 )
 
@@ -3421,89 +2760,22 @@
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDocumentAttributeConditionOutputTypeDef = TypedDict(
-    "_RequiredDocumentAttributeConditionOutputTypeDef",
-    {
-        "ConditionDocumentAttributeKey": str,
-        "Operator": ConditionOperatorType,
-    },
-)
-_OptionalDocumentAttributeConditionOutputTypeDef = TypedDict(
-    "_OptionalDocumentAttributeConditionOutputTypeDef",
-    {
-        "ConditionOnValue": DocumentAttributeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DocumentAttributeConditionOutputTypeDef(
-    _RequiredDocumentAttributeConditionOutputTypeDef,
-    _OptionalDocumentAttributeConditionOutputTypeDef,
-):
-    pass
-
-
-DocumentAttributeOutputTypeDef = TypedDict(
-    "DocumentAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": DocumentAttributeValueOutputTypeDef,
-    },
-)
-
-DocumentAttributeTargetOutputTypeDef = TypedDict(
-    "DocumentAttributeTargetOutputTypeDef",
-    {
-        "TargetDocumentAttributeKey": str,
-        "TargetDocumentAttributeValueDeletion": bool,
-        "TargetDocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-DocumentAttributeValueCountPairTypeDef = TypedDict(
-    "DocumentAttributeValueCountPairTypeDef",
-    {
-        "DocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
-        "Count": int,
-        "FacetResults": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
-_RequiredDocumentMetadataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDocumentMetadataConfigurationOutputTypeDef",
+DocumentRelevanceConfigurationTypeDef = TypedDict(
+    "DocumentRelevanceConfigurationTypeDef",
     {
         "Name": str,
-        "Type": DocumentAttributeValueTypeType,
-    },
-)
-_OptionalDocumentMetadataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDocumentMetadataConfigurationOutputTypeDef",
-    {
-        "Relevance": RelevanceOutputTypeDef,
-        "Search": SearchTypeDef,
+        "Relevance": RelevanceTypeDef,
     },
-    total=False,
 )
 
-
-class DocumentMetadataConfigurationOutputTypeDef(
-    _RequiredDocumentMetadataConfigurationOutputTypeDef,
-    _OptionalDocumentMetadataConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredDocumentMetadataConfigurationTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
 )
@@ -3519,47 +2791,14 @@
 
 class DocumentMetadataConfigurationTypeDef(
     _RequiredDocumentMetadataConfigurationTypeDef, _OptionalDocumentMetadataConfigurationTypeDef
 ):
     pass
 
 
-DocumentRelevanceConfigurationTypeDef = TypedDict(
-    "DocumentRelevanceConfigurationTypeDef",
-    {
-        "Name": str,
-        "Relevance": RelevanceTypeDef,
-    },
-)
-
-_RequiredS3DataSourceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3DataSourceConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3DataSourceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3DataSourceConfigurationOutputTypeDef",
-    {
-        "InclusionPrefixes": List[str],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
-        "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DataSourceConfigurationOutputTypeDef(
-    _RequiredS3DataSourceConfigurationOutputTypeDef, _OptionalS3DataSourceConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3DataSourceConfigurationTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationTypeDef = TypedDict(
@@ -3587,23 +2826,14 @@
         "EntityId": str,
         "EntityType": EntityTypeType,
         "DisplayData": EntityDisplayDataTypeDef,
     },
     total=False,
 )
 
-ExperienceConfigurationOutputTypeDef = TypedDict(
-    "ExperienceConfigurationOutputTypeDef",
-    {
-        "ContentSourceConfiguration": ContentSourceConfigurationOutputTypeDef,
-        "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ExperienceConfigurationTypeDef = TypedDict(
     "ExperienceConfigurationTypeDef",
     {
         "ContentSourceConfiguration": ContentSourceConfigurationTypeDef,
         "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
     },
     total=False,
@@ -3626,22 +2856,48 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
-        "SnapShotTimeFilter": TimeRangeOutputTypeDef,
+        "SnapShotTimeFilter": TimeRangeTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+    },
+)
+_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTimeFilter": TimeRangeTypeDef,
+        "StatusFilter": DataSourceSyncJobStatusType,
+    },
+    total=False,
+)
+
+
+class ListDataSourceSyncJobsRequestRequestTypeDef(
+    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
+    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
+):
+    pass
+
+
 GroupMembersTypeDef = TypedDict(
     "GroupMembersTypeDef",
     {
         "MemberGroups": Sequence[MemberGroupTypeDef],
         "MemberUsers": Sequence[MemberUserTypeDef],
         "S3PathforGroupMembers": S3PathTypeDef,
     },
@@ -3715,23 +2971,14 @@
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UrlsOutputTypeDef = TypedDict(
-    "UrlsOutputTypeDef",
-    {
-        "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
-        "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 UrlsTypeDef = TypedDict(
     "UrlsTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationTypeDef,
     },
     total=False,
@@ -3750,39 +2997,14 @@
     "TableRowTypeDef",
     {
         "Cells": List[TableCellTypeDef],
     },
     total=False,
 )
 
-_RequiredDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDatabaseConfigurationOutputTypeDef",
-    {
-        "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
-        "ColumnConfiguration": ColumnConfigurationOutputTypeDef,
-    },
-)
-_OptionalDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDatabaseConfigurationOutputTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "AclConfiguration": AclConfigurationTypeDef,
-        "SqlConfiguration": SqlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class DatabaseConfigurationOutputTypeDef(
-    _RequiredDatabaseConfigurationOutputTypeDef, _OptionalDatabaseConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredDatabaseConfigurationTypeDef",
     {
         "DatabaseEngineType": DatabaseEngineTypeType,
         "ConnectionConfiguration": ConnectionConfigurationTypeDef,
         "ColumnConfiguration": ColumnConfigurationTypeDef,
     },
@@ -3800,41 +3022,14 @@
 
 class DatabaseConfigurationTypeDef(
     _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
 ):
     pass
 
 
-_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "IncludedStates": List[SalesforceKnowledgeArticleStateType],
-    },
-)
-_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "StandardKnowledgeArticleTypeConfiguration": (
-            SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef
-        ),
-        "CustomKnowledgeArticleTypeConfigurations": List[
-            SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef
-        ],
-    },
-    total=False,
-)
-
-
-class SalesforceKnowledgeArticleConfigurationOutputTypeDef(
-    _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef,
-    _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
     {
         "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -3854,39 +3049,14 @@
 class SalesforceKnowledgeArticleConfigurationTypeDef(
     _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
     _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredServiceNowConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowConfigurationOutputTypeDef",
-    {
-        "HostUrl": str,
-        "SecretArn": str,
-        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
-    },
-)
-_OptionalServiceNowConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowConfigurationOutputTypeDef",
-    {
-        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationOutputTypeDef,
-        "AuthenticationType": ServiceNowAuthenticationTypeType,
-    },
-    total=False,
-)
-
-
-class ServiceNowConfigurationOutputTypeDef(
-    _RequiredServiceNowConfigurationOutputTypeDef, _OptionalServiceNowConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredServiceNowConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowConfigurationTypeDef",
     {
         "HostUrl": str,
         "SecretArn": str,
         "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
     },
@@ -3904,63 +3074,14 @@
 
 class ServiceNowConfigurationTypeDef(
     _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
 ):
     pass
 
 
-_RequiredGitHubConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGitHubConfigurationOutputTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGitHubConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGitHubConfigurationOutputTypeDef",
-    {
-        "SaaSConfiguration": SaaSConfigurationTypeDef,
-        "OnPremiseConfiguration": OnPremiseConfigurationTypeDef,
-        "Type": TypeType,
-        "UseChangeLog": bool,
-        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesTypeDef,
-        "RepositoryFilter": List[str],
-        "InclusionFolderNamePatterns": List[str],
-        "InclusionFileTypePatterns": List[str],
-        "InclusionFileNamePatterns": List[str],
-        "ExclusionFolderNamePatterns": List[str],
-        "ExclusionFileTypePatterns": List[str],
-        "ExclusionFileNamePatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "GitHubRepositoryConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueDocumentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueCommentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-    },
-    total=False,
-)
-
-
-class GitHubConfigurationOutputTypeDef(
-    _RequiredGitHubConfigurationOutputTypeDef, _OptionalGitHubConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredGitHubConfigurationTypeDef = TypedDict(
     "_RequiredGitHubConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationTypeDef = TypedDict(
@@ -4008,40 +3129,14 @@
 
 class GitHubConfigurationTypeDef(
     _RequiredGitHubConfigurationTypeDef, _OptionalGitHubConfigurationTypeDef
 ):
     pass
 
 
-_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOneDriveConfigurationOutputTypeDef",
-    {
-        "TenantDomain": str,
-        "SecretArn": str,
-        "OneDriveUsers": OneDriveUsersOutputTypeDef,
-    },
-)
-_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOneDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "DisableLocalGroups": bool,
-    },
-    total=False,
-)
-
-
-class OneDriveConfigurationOutputTypeDef(
-    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredOneDriveConfigurationTypeDef = TypedDict(
     "_RequiredOneDriveConfigurationTypeDef",
     {
         "TenantDomain": str,
         "SecretArn": str,
         "OneDriveUsers": OneDriveUsersTypeDef,
     },
@@ -4167,72 +3262,24 @@
     "DocumentAttributeTypeDef",
     {
         "Key": str,
         "Value": DocumentAttributeValueTypeDef,
     },
 )
 
-_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-    },
-)
-_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTimeFilter": TimeRangeTypeDef,
-        "StatusFilter": DataSourceSyncJobStatusType,
-    },
-    total=False,
-)
-
-
-class ListDataSourceSyncJobsRequestRequestTypeDef(
-    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
-    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
-):
-    pass
-
-
-TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
-_RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredConfluenceConfigurationOutputTypeDef",
-    {
-        "ServerUrl": str,
-        "SecretArn": str,
-        "Version": ConfluenceVersionType,
-    },
-)
-_OptionalConfluenceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalConfluenceConfigurationOutputTypeDef",
+DocumentAttributeValueCountPairTypeDef = TypedDict(
+    "DocumentAttributeValueCountPairTypeDef",
     {
-        "SpaceConfiguration": ConfluenceSpaceConfigurationOutputTypeDef,
-        "PageConfiguration": ConfluencePageConfigurationOutputTypeDef,
-        "BlogConfiguration": ConfluenceBlogConfigurationOutputTypeDef,
-        "AttachmentConfiguration": ConfluenceAttachmentConfigurationOutputTypeDef,
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-        "AuthenticationType": ConfluenceAuthenticationTypeType,
+        "DocumentAttributeValue": DocumentAttributeValueTypeDef,
+        "Count": int,
+        "FacetResults": List[Dict[str, Any]],
     },
     total=False,
 )
 
-
-class ConfluenceConfigurationOutputTypeDef(
-    _RequiredConfluenceConfigurationOutputTypeDef, _OptionalConfluenceConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4256,29 +3303,78 @@
 
 class ConfluenceConfigurationTypeDef(
     _RequiredConfluenceConfigurationTypeDef, _OptionalConfluenceConfigurationTypeDef
 ):
     pass
 
 
+_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
     "DescribeAccessControlConfigurationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
-        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
+        "HierarchicalAccessControlList": List[HierarchicalPrincipalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HierarchicalPrincipalUnionTypeDef = Union[
-    HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef
-]
+_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+    },
+)
+_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 CreateFeaturedResultsSetResponseTypeDef = TypedDict(
     "CreateFeaturedResultsSetResponseTypeDef",
     {
         "FeaturedResultsSet": FeaturedResultsSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4316,72 +3412,14 @@
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHookConfigurationOutputTypeDef = TypedDict(
-    "_RequiredHookConfigurationOutputTypeDef",
-    {
-        "LambdaArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalHookConfigurationOutputTypeDef = TypedDict(
-    "_OptionalHookConfigurationOutputTypeDef",
-    {
-        "InvocationCondition": DocumentAttributeConditionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HookConfigurationOutputTypeDef(
-    _RequiredHookConfigurationOutputTypeDef, _OptionalHookConfigurationOutputTypeDef
-):
-    pass
-
-
-RetrieveResultItemTypeDef = TypedDict(
-    "RetrieveResultItemTypeDef",
-    {
-        "Id": str,
-        "DocumentId": str,
-        "DocumentTitle": str,
-        "Content": str,
-        "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
-    },
-    total=False,
-)
-
-SourceDocumentTypeDef = TypedDict(
-    "SourceDocumentTypeDef",
-    {
-        "DocumentId": str,
-        "SuggestionAttributes": List[str],
-        "AdditionalAttributes": List[DocumentAttributeOutputTypeDef],
-    },
-    total=False,
-)
-
-InlineCustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
-    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    {
-        "Condition": DocumentAttributeConditionOutputTypeDef,
-        "Target": DocumentAttributeTargetOutputTypeDef,
-        "DocumentContentDeletion": bool,
-    },
-    total=False,
-)
-
-DocumentMetadataConfigurationUnionTypeDef = Union[
-    DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef
-]
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4442,32 +3480,14 @@
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeExperienceResponseTypeDef = TypedDict(
-    "DescribeExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Endpoints": List[ExperienceEndpointTypeDef],
-        "Configuration": ExperienceConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": ExperienceStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
     },
 )
@@ -4485,17 +3505,32 @@
 
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
 
-ExperienceConfigurationUnionTypeDef = Union[
-    ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-]
+DescribeExperienceResponseTypeDef = TypedDict(
+    "DescribeExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Endpoints": List[ExperienceEndpointTypeDef],
+        "Configuration": ExperienceConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": ExperienceStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4588,49 +3623,49 @@
         "Edition": IndexEditionType,
         "RoleArn": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "Status": IndexStatusType,
         "Description": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
+        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationTypeDef],
         "IndexStatistics": IndexStatisticsTypeDef,
         "ErrorMessage": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
-    "_RequiredWebCrawlerConfigurationOutputTypeDef",
+_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIndexRequestRequestTypeDef",
     {
-        "Urls": UrlsOutputTypeDef,
+        "Id": str,
     },
 )
-_OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
-    "_OptionalWebCrawlerConfigurationOutputTypeDef",
+_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIndexRequestRequestTypeDef",
     {
-        "CrawlDepth": int,
-        "MaxLinksPerPage": int,
-        "MaxContentSizePerPageInMegaBytes": float,
-        "MaxUrlsPerMinuteCrawlRate": int,
-        "UrlInclusionPatterns": List[str],
-        "UrlExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "Description": str,
+        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationTypeDef],
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class WebCrawlerConfigurationOutputTypeDef(
-    _RequiredWebCrawlerConfigurationOutputTypeDef, _OptionalWebCrawlerConfigurationOutputTypeDef
+class UpdateIndexRequestRequestTypeDef(
+    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredWebCrawlerConfigurationTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationTypeDef",
     {
@@ -4672,44 +3707,14 @@
     {
         "Rows": List[TableRowTypeDef],
         "TotalNumberOfRows": int,
     },
     total=False,
 )
 
-_RequiredSalesforceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceConfigurationOutputTypeDef",
-    {
-        "ServerUrl": str,
-        "SecretArn": str,
-    },
-)
-_OptionalSalesforceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceConfigurationOutputTypeDef",
-    {
-        "StandardObjectConfigurations": List[SalesforceStandardObjectConfigurationOutputTypeDef],
-        "KnowledgeArticleConfiguration": SalesforceKnowledgeArticleConfigurationOutputTypeDef,
-        "ChatterFeedConfiguration": SalesforceChatterFeedConfigurationOutputTypeDef,
-        "CrawlAttachments": bool,
-        "StandardObjectAttachmentConfiguration": (
-            SalesforceStandardObjectAttachmentConfigurationOutputTypeDef
-        ),
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-    },
-    total=False,
-)
-
-
-class SalesforceConfigurationOutputTypeDef(
-    _RequiredSalesforceConfigurationOutputTypeDef, _OptionalSalesforceConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSalesforceConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
     },
 )
@@ -4826,66 +3831,37 @@
 )
 
 
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
 
-_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+RetrieveResultItemTypeDef = TypedDict(
+    "RetrieveResultItemTypeDef",
     {
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
-        "ClientToken": str,
+        "Id": str,
+        "DocumentId": str,
+        "DocumentTitle": str,
+        "Content": str,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-
-class CreateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-    },
-)
-_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+SourceDocumentTypeDef = TypedDict(
+    "SourceDocumentTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+        "DocumentId": str,
+        "SuggestionAttributes": List[str],
+        "AdditionalAttributes": List[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-
-class UpdateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4903,106 +3879,23 @@
 class GetQuerySuggestionsRequestRequestTypeDef(
     _RequiredGetQuerySuggestionsRequestRequestTypeDef,
     _OptionalGetQuerySuggestionsRequestRequestTypeDef,
 ):
     pass
 
 
-RetrieveResultTypeDef = TypedDict(
-    "RetrieveResultTypeDef",
-    {
-        "QueryId": str,
-        "ResultItems": List[RetrieveResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
-    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    {
-        "InlineConfigurations": List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef],
-        "PreExtractionHookConfiguration": HookConfigurationOutputTypeDef,
-        "PostExtractionHookConfiguration": HookConfigurationOutputTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIndexRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIndexRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-        "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationUnionTypeDef],
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateIndexRequestRequestTypeDef(
-    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
-):
-    pass
-
-
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
 )
 
-SuggestionTypeDef = TypedDict(
-    "SuggestionTypeDef",
-    {
-        "Id": str,
-        "Value": SuggestionValueTypeDef,
-        "SourceDocuments": List[SourceDocumentTypeDef],
-    },
-    total=False,
-)
-
-DataSourceConfigurationOutputTypeDef = TypedDict(
-    "DataSourceConfigurationOutputTypeDef",
-    {
-        "S3Configuration": S3DataSourceConfigurationOutputTypeDef,
-        "SharePointConfiguration": SharePointConfigurationOutputTypeDef,
-        "DatabaseConfiguration": DatabaseConfigurationOutputTypeDef,
-        "SalesforceConfiguration": SalesforceConfigurationOutputTypeDef,
-        "OneDriveConfiguration": OneDriveConfigurationOutputTypeDef,
-        "ServiceNowConfiguration": ServiceNowConfigurationOutputTypeDef,
-        "ConfluenceConfiguration": ConfluenceConfigurationOutputTypeDef,
-        "GoogleDriveConfiguration": GoogleDriveConfigurationOutputTypeDef,
-        "WebCrawlerConfiguration": WebCrawlerConfigurationOutputTypeDef,
-        "WorkDocsConfiguration": WorkDocsConfigurationOutputTypeDef,
-        "FsxConfiguration": FsxConfigurationOutputTypeDef,
-        "SlackConfiguration": SlackConfigurationOutputTypeDef,
-        "BoxConfiguration": BoxConfigurationOutputTypeDef,
-        "QuipConfiguration": QuipConfigurationOutputTypeDef,
-        "JiraConfiguration": JiraConfigurationOutputTypeDef,
-        "GitHubConfiguration": GitHubConfigurationOutputTypeDef,
-        "AlfrescoConfiguration": AlfrescoConfigurationOutputTypeDef,
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "S3Configuration": S3DataSourceConfigurationTypeDef,
         "SharePointConfiguration": SharePointConfigurationTypeDef,
         "DatabaseConfiguration": DatabaseConfigurationTypeDef,
         "SalesforceConfiguration": SalesforceConfigurationTypeDef,
@@ -5039,25 +3932,44 @@
     "BatchGetDocumentStatusRequestRequestTypeDef",
     {
         "IndexId": str,
         "DocumentInfoList": Sequence[DocumentInfoTypeDef],
     },
 )
 
+RetrieveResultTypeDef = TypedDict(
+    "RetrieveResultTypeDef",
+    {
+        "QueryId": str,
+        "ResultItems": List[RetrieveResultItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SuggestionTypeDef = TypedDict(
+    "SuggestionTypeDef",
+    {
+        "Id": str,
+        "Value": SuggestionValueTypeDef,
+        "SourceDocuments": List[SourceDocumentTypeDef],
+    },
+    total=False,
+)
+
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
         "FeedbackToken": str,
     },
     total=False,
 )
 
 QueryResultItemTypeDef = TypedDict(
     "QueryResultItemTypeDef",
@@ -5066,56 +3978,22 @@
         "Type": QueryResultTypeType,
         "Format": QueryResultFormatType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
         "ScoreAttributes": ScoreAttributesTypeDef,
         "FeedbackToken": str,
         "TableExcerpt": TableExcerptTypeDef,
     },
     total=False,
 )
 
-GetQuerySuggestionsResponseTypeDef = TypedDict(
-    "GetQuerySuggestionsResponseTypeDef",
-    {
-        "QuerySuggestionsId": str,
-        "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourceResponseTypeDef = TypedDict(
-    "DescribeDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Type": DataSourceTypeType,
-        "Configuration": DataSourceConfigurationOutputTypeDef,
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": DataSourceStatusType,
-        "Schedule": str,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "LanguageCode": str,
-        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataSourceConfigurationUnionTypeDef = Union[
-    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-]
 _RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredBatchPutDocumentRequestRequestTypeDef",
     {
         "IndexId": str,
         "Documents": Sequence[DocumentTypeDef],
     },
 )
@@ -5162,17 +4040,36 @@
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
 
-CustomDocumentEnrichmentConfigurationUnionTypeDef = Union[
-    CustomDocumentEnrichmentConfigurationTypeDef, CustomDocumentEnrichmentConfigurationOutputTypeDef
-]
+DescribeDataSourceResponseTypeDef = TypedDict(
+    "DescribeDataSourceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Type": DataSourceTypeType,
+        "Configuration": DataSourceConfigurationTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": DataSourceStatusType,
+        "Schedule": str,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "LanguageCode": str,
+        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -5194,14 +4091,23 @@
 
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
     pass
 
 
+GetQuerySuggestionsResponseTypeDef = TypedDict(
+    "GetQuerySuggestionsResponseTypeDef",
+    {
+        "QuerySuggestionsId": str,
+        "Suggestions": List[SuggestionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 QueryResultTypeDef = TypedDict(
     "QueryResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
```

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra/type_defs.pyi` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -87,17 +87,16 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessControlConfigurationSummaryTypeDef",
     "AccessControlListConfigurationTypeDef",
     "AclConfigurationTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
-    "DataSourceVpcConfigurationOutputTypeDef",
-    "S3PathTypeDef",
     "DataSourceVpcConfigurationTypeDef",
+    "S3PathTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
     "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
     "SuggestableConfigTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
@@ -113,23 +112,21 @@
     "TimestampTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
-    "ContentSourceConfigurationOutputTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
     "TagTypeDef",
     "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
-    "TemplateConfigurationOutputTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -150,28 +147,26 @@
     "DescribeIndexRequestRequestTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
-    "DocumentAttributeValueOutputTypeDef",
-    "RelevanceOutputTypeDef",
-    "SearchTypeDef",
     "RelevanceTypeDef",
+    "SearchTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
     "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
-    "TimeRangeOutputTypeDef",
+    "TimeRangeTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
@@ -194,61 +189,41 @@
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
-    "SeedUrlConfigurationOutputTypeDef",
     "SeedUrlConfigurationTypeDef",
-    "SiteMapsConfigurationOutputTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
-    "GoogleDriveConfigurationOutputTypeDef",
     "GoogleDriveConfigurationTypeDef",
-    "SalesforceChatterFeedConfigurationOutputTypeDef",
     "SalesforceChatterFeedConfigurationTypeDef",
-    "SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
-    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
-    "SalesforceStandardObjectConfigurationOutputTypeDef",
     "SalesforceStandardObjectConfigurationTypeDef",
-    "ServiceNowKnowledgeArticleConfigurationOutputTypeDef",
     "ServiceNowKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowServiceCatalogConfigurationOutputTypeDef",
     "ServiceNowServiceCatalogConfigurationTypeDef",
-    "WorkDocsConfigurationOutputTypeDef",
     "WorkDocsConfigurationTypeDef",
-    "BoxConfigurationOutputTypeDef",
-    "FsxConfigurationOutputTypeDef",
-    "JiraConfigurationOutputTypeDef",
-    "QuipConfigurationOutputTypeDef",
-    "SlackConfigurationOutputTypeDef",
-    "AlfrescoConfigurationOutputTypeDef",
-    "OnPremiseConfigurationTypeDef",
-    "OneDriveUsersOutputTypeDef",
-    "OneDriveUsersTypeDef",
-    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
-    "UpdateThesaurusRequestRequestTypeDef",
-    "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
-    "DataSourceVpcConfigurationUnionTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
+    "AlfrescoConfigurationTypeDef",
+    "OnPremiseConfigurationTypeDef",
+    "OneDriveUsersTypeDef",
+    "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
+    "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
     "CreateAccessControlConfigurationResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
     "CreateExperienceResponseTypeDef",
@@ -263,36 +238,28 @@
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAccessControlConfigurationsResponseTypeDef",
     "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
     "AttributeSuggestionsDescribeConfigTypeDef",
     "AttributeSuggestionsUpdateConfigTypeDef",
-    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "ClickFeedbackTypeDef",
     "DocumentAttributeValueTypeDef",
-    "TimeRangeTypeDef",
-    "ConfluenceAttachmentConfigurationOutputTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
-    "ConfluenceBlogConfigurationOutputTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
-    "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
-    "ConfluencePageConfigurationOutputTypeDef",
     "ConfluencePageConfigurationTypeDef",
-    "ConfluenceSpaceConfigurationOutputTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
-    "HierarchicalPrincipalOutputTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFeaturedResultsSetRequestRequestTypeDef",
@@ -300,117 +267,92 @@
     "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
-    "DocumentAttributeConditionOutputTypeDef",
-    "DocumentAttributeOutputTypeDef",
-    "DocumentAttributeTargetOutputTypeDef",
-    "DocumentAttributeValueCountPairTypeDef",
-    "DocumentMetadataConfigurationOutputTypeDef",
-    "DocumentMetadataConfigurationTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
-    "S3DataSourceConfigurationOutputTypeDef",
+    "DocumentMetadataConfigurationTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
-    "ExperienceConfigurationOutputTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
     "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
+    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
     "UserTokenConfigurationTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     "ListThesauriResponseTypeDef",
-    "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
-    "DatabaseConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
-    "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
-    "ServiceNowConfigurationOutputTypeDef",
     "ServiceNowConfigurationTypeDef",
-    "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
-    "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
-    "ListDataSourceSyncJobsRequestRequestTypeDef",
-    "TimeRangeUnionTypeDef",
-    "ConfluenceConfigurationOutputTypeDef",
+    "DocumentAttributeValueCountPairTypeDef",
     "ConfluenceConfigurationTypeDef",
+    "CreateAccessControlConfigurationRequestRequestTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
-    "HierarchicalPrincipalUnionTypeDef",
+    "UpdateAccessControlConfigurationRequestRequestTypeDef",
     "CreateFeaturedResultsSetResponseTypeDef",
     "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
-    "HookConfigurationOutputTypeDef",
-    "RetrieveResultItemTypeDef",
-    "SourceDocumentTypeDef",
-    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "DocumentMetadataConfigurationUnionTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
-    "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
-    "ExperienceConfigurationUnionTypeDef",
+    "DescribeExperienceResponseTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
-    "WebCrawlerConfigurationOutputTypeDef",
+    "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
-    "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "DocumentInfoTypeDef",
     "DocumentTypeDef",
-    "CreateAccessControlConfigurationRequestRequestTypeDef",
-    "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "RetrieveResultItemTypeDef",
+    "SourceDocumentTypeDef",
     "GetQuerySuggestionsRequestRequestTypeDef",
-    "RetrieveResultTypeDef",
-    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "UpdateIndexRequestRequestTypeDef",
     "AdditionalResultAttributeTypeDef",
-    "SuggestionTypeDef",
-    "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
     "CustomDocumentEnrichmentConfigurationTypeDef",
     "BatchGetDocumentStatusRequestRequestTypeDef",
+    "RetrieveResultTypeDef",
+    "SuggestionTypeDef",
     "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
-    "GetQuerySuggestionsResponseTypeDef",
-    "DescribeDataSourceResponseTypeDef",
-    "DataSourceConfigurationUnionTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
-    "CustomDocumentEnrichmentConfigurationUnionTypeDef",
+    "DescribeDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
+    "GetQuerySuggestionsResponseTypeDef",
     "QueryResultTypeDef",
 )
 
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
         "Id": str,
@@ -448,38 +390,30 @@
 )
 
 class DataSourceToIndexFieldMappingTypeDef(
     _RequiredDataSourceToIndexFieldMappingTypeDef, _OptionalDataSourceToIndexFieldMappingTypeDef
 ):
     pass
 
-DataSourceVpcConfigurationOutputTypeDef = TypedDict(
-    "DataSourceVpcConfigurationOutputTypeDef",
+DataSourceVpcConfigurationTypeDef = TypedDict(
+    "DataSourceVpcConfigurationTypeDef",
     {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
     },
 )
 
 S3PathTypeDef = TypedDict(
     "S3PathTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-DataSourceVpcConfigurationTypeDef = TypedDict(
-    "DataSourceVpcConfigurationTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-)
-
 EntityConfigurationTypeDef = TypedDict(
     "EntityConfigurationTypeDef",
     {
         "EntityId": str,
         "EntityType": EntityTypeType,
     },
 )
@@ -691,24 +625,14 @@
         "DatabasePort": int,
         "DatabaseName": str,
         "TableName": str,
         "SecretArn": str,
     },
 )
 
-ContentSourceConfigurationOutputTypeDef = TypedDict(
-    "ContentSourceConfigurationOutputTypeDef",
-    {
-        "DataSourceIds": List[str],
-        "FaqIds": List[str],
-        "DirectPutContent": bool,
-    },
-    total=False,
-)
-
 ContentSourceConfigurationTypeDef = TypedDict(
     "ContentSourceConfigurationTypeDef",
     {
         "DataSourceIds": Sequence[str],
         "FaqIds": Sequence[str],
         "DirectPutContent": bool,
     },
@@ -772,22 +696,14 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
-TemplateConfigurationOutputTypeDef = TypedDict(
-    "TemplateConfigurationOutputTypeDef",
-    {
-        "Template": Dict[str, Any],
-    },
-    total=False,
-)
-
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "Template": Mapping[str, Any],
     },
     total=False,
 )
@@ -1046,27 +962,16 @@
     {
         "Id": str,
         "IndexId": str,
         "EntityIds": Sequence[str],
     },
 )
 
-DocumentAttributeValueOutputTypeDef = TypedDict(
-    "DocumentAttributeValueOutputTypeDef",
-    {
-        "StringValue": str,
-        "StringListValue": List[str],
-        "LongValue": int,
-        "DateValue": datetime,
-    },
-    total=False,
-)
-
-RelevanceOutputTypeDef = TypedDict(
-    "RelevanceOutputTypeDef",
+RelevanceTypeDef = TypedDict(
+    "RelevanceTypeDef",
     {
         "Freshness": bool,
         "Importance": int,
         "Duration": str,
         "RankOrder": OrderType,
         "ValueImportanceMap": Dict[str, int],
     },
@@ -1080,26 +985,14 @@
         "Searchable": bool,
         "Displayable": bool,
         "Sortable": bool,
     },
     total=False,
 )
 
-RelevanceTypeDef = TypedDict(
-    "RelevanceTypeDef",
-    {
-        "Freshness": bool,
-        "Importance": int,
-        "Duration": str,
-        "RankOrder": OrderType,
-        "ValueImportanceMap": Mapping[str, int],
-    },
-    total=False,
-)
-
 DocumentsMetadataConfigurationTypeDef = TypedDict(
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
     },
     total=False,
 )
@@ -1195,16 +1088,16 @@
 )
 
 class GetSnapshotsRequestRequestTypeDef(
     _RequiredGetSnapshotsRequestRequestTypeDef, _OptionalGetSnapshotsRequestRequestTypeDef
 ):
     pass
 
-TimeRangeOutputTypeDef = TypedDict(
-    "TimeRangeOutputTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
@@ -1642,33 +1535,14 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
     },
 )
 
-_RequiredSeedUrlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSeedUrlConfigurationOutputTypeDef",
-    {
-        "SeedUrls": List[str],
-    },
-)
-_OptionalSeedUrlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSeedUrlConfigurationOutputTypeDef",
-    {
-        "WebCrawlerMode": WebCrawlerModeType,
-    },
-    total=False,
-)
-
-class SeedUrlConfigurationOutputTypeDef(
-    _RequiredSeedUrlConfigurationOutputTypeDef, _OptionalSeedUrlConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
@@ -1680,21 +1554,14 @@
 )
 
 class SeedUrlConfigurationTypeDef(
     _RequiredSeedUrlConfigurationTypeDef, _OptionalSeedUrlConfigurationTypeDef
 ):
     pass
 
-SiteMapsConfigurationOutputTypeDef = TypedDict(
-    "SiteMapsConfigurationOutputTypeDef",
-    {
-        "SiteMaps": List[str],
-    },
-)
-
 SiteMapsConfigurationTypeDef = TypedDict(
     "SiteMapsConfigurationTypeDef",
     {
         "SiteMaps": Sequence[str],
     },
 )
 
@@ -1738,36 +1605,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredColumnConfigurationOutputTypeDef = TypedDict(
-    "_RequiredColumnConfigurationOutputTypeDef",
-    {
-        "DocumentIdColumnName": str,
-        "DocumentDataColumnName": str,
-        "ChangeDetectingColumns": List[str],
-    },
-)
-_OptionalColumnConfigurationOutputTypeDef = TypedDict(
-    "_OptionalColumnConfigurationOutputTypeDef",
-    {
-        "DocumentTitleColumnName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class ColumnConfigurationOutputTypeDef(
-    _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": Sequence[str],
     },
@@ -1782,38 +1627,14 @@
 )
 
 class ColumnConfigurationTypeDef(
     _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
 ):
     pass
 
-_RequiredGoogleDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGoogleDriveConfigurationOutputTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGoogleDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGoogleDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "ExcludeMimeTypes": List[str],
-        "ExcludeUserAccounts": List[str],
-        "ExcludeSharedDrives": List[str],
-    },
-    total=False,
-)
-
-class GoogleDriveConfigurationOutputTypeDef(
-    _RequiredGoogleDriveConfigurationOutputTypeDef, _OptionalGoogleDriveConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredGoogleDriveConfigurationTypeDef = TypedDict(
     "_RequiredGoogleDriveConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGoogleDriveConfigurationTypeDef = TypedDict(
@@ -1830,36 +1651,14 @@
 )
 
 class GoogleDriveConfigurationTypeDef(
     _RequiredGoogleDriveConfigurationTypeDef, _OptionalGoogleDriveConfigurationTypeDef
 ):
     pass
 
-_RequiredSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceChatterFeedConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceChatterFeedConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceChatterFeedConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "IncludeFilterTypes": List[SalesforceChatterFeedIncludeFilterTypeType],
-    },
-    total=False,
-)
-
-class SalesforceChatterFeedConfigurationOutputTypeDef(
-    _RequiredSalesforceChatterFeedConfigurationOutputTypeDef,
-    _OptionalSalesforceChatterFeedConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceChatterFeedConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceChatterFeedConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceChatterFeedConfigurationTypeDef = TypedDict(
@@ -1874,36 +1673,14 @@
 
 class SalesforceChatterFeedConfigurationTypeDef(
     _RequiredSalesforceChatterFeedConfigurationTypeDef,
     _OptionalSalesforceChatterFeedConfigurationTypeDef,
 ):
     pass
 
-_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(
-    _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
-    _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     {
         "Name": str,
         "DocumentDataFieldName": str,
     },
 )
@@ -1918,35 +1695,14 @@
 
 class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
-_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(
-    _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
-    _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef = TypedDict(
@@ -1960,54 +1716,23 @@
 
 class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(
     _RequiredSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     _OptionalSalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
 ):
     pass
 
-SalesforceStandardObjectAttachmentConfigurationOutputTypeDef = TypedDict(
-    "SalesforceStandardObjectAttachmentConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 SalesforceStandardObjectAttachmentConfigurationTypeDef = TypedDict(
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     {
         "DocumentTitleFieldName": str,
         "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-_RequiredSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceStandardObjectConfigurationOutputTypeDef",
-    {
-        "Name": SalesforceStandardObjectNameType,
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalSalesforceStandardObjectConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceStandardObjectConfigurationOutputTypeDef",
-    {
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class SalesforceStandardObjectConfigurationOutputTypeDef(
-    _RequiredSalesforceStandardObjectConfigurationOutputTypeDef,
-    _OptionalSalesforceStandardObjectConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceStandardObjectConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceStandardObjectConfigurationTypeDef",
     {
         "Name": SalesforceStandardObjectNameType,
         "DocumentDataFieldName": str,
     },
 )
@@ -2022,39 +1747,14 @@
 
 class SalesforceStandardObjectConfigurationTypeDef(
     _RequiredSalesforceStandardObjectConfigurationTypeDef,
     _OptionalSalesforceStandardObjectConfigurationTypeDef,
 ):
     pass
 
-_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "FilterQuery": str,
-    },
-    total=False,
-)
-
-class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(
-    _RequiredServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-    _OptionalServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowKnowledgeArticleConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -2072,38 +1772,14 @@
 
 class ServiceNowKnowledgeArticleConfigurationTypeDef(
     _RequiredServiceNowKnowledgeArticleConfigurationTypeDef,
     _OptionalServiceNowKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
-_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowServiceCatalogConfigurationOutputTypeDef",
-    {
-        "DocumentDataFieldName": str,
-    },
-)
-_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowServiceCatalogConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-        "DocumentTitleFieldName": str,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class ServiceNowServiceCatalogConfigurationOutputTypeDef(
-    _RequiredServiceNowServiceCatalogConfigurationOutputTypeDef,
-    _OptionalServiceNowServiceCatalogConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowServiceCatalogConfigurationTypeDef",
     {
         "DocumentDataFieldName": str,
     },
 )
 _OptionalServiceNowServiceCatalogConfigurationTypeDef = TypedDict(
@@ -2120,37 +1796,14 @@
 
 class ServiceNowServiceCatalogConfigurationTypeDef(
     _RequiredServiceNowServiceCatalogConfigurationTypeDef,
     _OptionalServiceNowServiceCatalogConfigurationTypeDef,
 ):
     pass
 
-_RequiredWorkDocsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredWorkDocsConfigurationOutputTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalWorkDocsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalWorkDocsConfigurationOutputTypeDef",
-    {
-        "CrawlComments": bool,
-        "UseChangeLog": bool,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class WorkDocsConfigurationOutputTypeDef(
-    _RequiredWorkDocsConfigurationOutputTypeDef, _OptionalWorkDocsConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredWorkDocsConfigurationTypeDef = TypedDict(
     "_RequiredWorkDocsConfigurationTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalWorkDocsConfigurationTypeDef = TypedDict(
@@ -2166,208 +1819,195 @@
 )
 
 class WorkDocsConfigurationTypeDef(
     _RequiredWorkDocsConfigurationTypeDef, _OptionalWorkDocsConfigurationTypeDef
 ):
     pass
 
-_RequiredBoxConfigurationOutputTypeDef = TypedDict(
-    "_RequiredBoxConfigurationOutputTypeDef",
+_RequiredBoxConfigurationTypeDef = TypedDict(
+    "_RequiredBoxConfigurationTypeDef",
     {
         "EnterpriseId": str,
         "SecretArn": str,
     },
 )
-_OptionalBoxConfigurationOutputTypeDef = TypedDict(
-    "_OptionalBoxConfigurationOutputTypeDef",
+_OptionalBoxConfigurationTypeDef = TypedDict(
+    "_OptionalBoxConfigurationTypeDef",
     {
         "UseChangeLog": bool,
         "CrawlComments": bool,
         "CrawlTasks": bool,
         "CrawlWebLinks": bool,
-        "FileFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "TaskFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WebLinkFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "FileFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "TaskFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WebLinkFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-class BoxConfigurationOutputTypeDef(
-    _RequiredBoxConfigurationOutputTypeDef, _OptionalBoxConfigurationOutputTypeDef
-):
+class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
-_RequiredFsxConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFsxConfigurationOutputTypeDef",
+_RequiredFsxConfigurationTypeDef = TypedDict(
+    "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
 )
-_OptionalFsxConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFsxConfigurationOutputTypeDef",
+_OptionalFsxConfigurationTypeDef = TypedDict(
+    "_OptionalFsxConfigurationTypeDef",
     {
         "SecretArn": str,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-class FsxConfigurationOutputTypeDef(
-    _RequiredFsxConfigurationOutputTypeDef, _OptionalFsxConfigurationOutputTypeDef
-):
+class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
     pass
 
-_RequiredJiraConfigurationOutputTypeDef = TypedDict(
-    "_RequiredJiraConfigurationOutputTypeDef",
+_RequiredJiraConfigurationTypeDef = TypedDict(
+    "_RequiredJiraConfigurationTypeDef",
     {
         "JiraAccountUrl": str,
         "SecretArn": str,
     },
 )
-_OptionalJiraConfigurationOutputTypeDef = TypedDict(
-    "_OptionalJiraConfigurationOutputTypeDef",
+_OptionalJiraConfigurationTypeDef = TypedDict(
+    "_OptionalJiraConfigurationTypeDef",
     {
         "UseChangeLog": bool,
-        "Project": List[str],
-        "IssueType": List[str],
-        "Status": List[str],
-        "IssueSubEntityFilter": List[IssueSubEntityType],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "IssueFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "ProjectFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WorkLogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "Project": Sequence[str],
+        "IssueType": Sequence[str],
+        "Status": Sequence[str],
+        "IssueSubEntityFilter": Sequence[IssueSubEntityType],
+        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "IssueFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "ProjectFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WorkLogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-class JiraConfigurationOutputTypeDef(
-    _RequiredJiraConfigurationOutputTypeDef, _OptionalJiraConfigurationOutputTypeDef
+class JiraConfigurationTypeDef(
+    _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
 ):
     pass
 
-_RequiredQuipConfigurationOutputTypeDef = TypedDict(
-    "_RequiredQuipConfigurationOutputTypeDef",
+_RequiredQuipConfigurationTypeDef = TypedDict(
+    "_RequiredQuipConfigurationTypeDef",
     {
         "Domain": str,
         "SecretArn": str,
     },
 )
-_OptionalQuipConfigurationOutputTypeDef = TypedDict(
-    "_OptionalQuipConfigurationOutputTypeDef",
+_OptionalQuipConfigurationTypeDef = TypedDict(
+    "_OptionalQuipConfigurationTypeDef",
     {
         "CrawlFileComments": bool,
         "CrawlChatRooms": bool,
         "CrawlAttachments": bool,
-        "FolderIds": List[str],
-        "ThreadFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "MessageFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "AttachmentFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "FolderIds": Sequence[str],
+        "ThreadFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "MessageFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-class QuipConfigurationOutputTypeDef(
-    _RequiredQuipConfigurationOutputTypeDef, _OptionalQuipConfigurationOutputTypeDef
+class QuipConfigurationTypeDef(
+    _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
 ):
     pass
 
-_RequiredSlackConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSlackConfigurationOutputTypeDef",
+_RequiredSlackConfigurationTypeDef = TypedDict(
+    "_RequiredSlackConfigurationTypeDef",
     {
         "TeamId": str,
         "SecretArn": str,
-        "SlackEntityList": List[SlackEntityType],
+        "SlackEntityList": Sequence[SlackEntityType],
         "SinceCrawlDate": str,
     },
 )
-_OptionalSlackConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSlackConfigurationOutputTypeDef",
+_OptionalSlackConfigurationTypeDef = TypedDict(
+    "_OptionalSlackConfigurationTypeDef",
     {
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
         "UseChangeLog": bool,
         "CrawlBotMessage": bool,
         "ExcludeArchived": bool,
         "LookBackPeriod": int,
-        "PrivateChannelFilter": List[str],
-        "PublicChannelFilter": List[str],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
+        "PrivateChannelFilter": Sequence[str],
+        "PublicChannelFilter": Sequence[str],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-class SlackConfigurationOutputTypeDef(
-    _RequiredSlackConfigurationOutputTypeDef, _OptionalSlackConfigurationOutputTypeDef
+class SlackConfigurationTypeDef(
+    _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
 ):
     pass
 
-_RequiredAlfrescoConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationOutputTypeDef",
+_RequiredAlfrescoConfigurationTypeDef = TypedDict(
+    "_RequiredAlfrescoConfigurationTypeDef",
     {
         "SiteUrl": str,
         "SiteId": str,
         "SecretArn": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
 )
-_OptionalAlfrescoConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationOutputTypeDef",
+_OptionalAlfrescoConfigurationTypeDef = TypedDict(
+    "_OptionalAlfrescoConfigurationTypeDef",
     {
         "CrawlSystemFolders": bool,
         "CrawlComments": bool,
-        "EntityFilter": List[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
+        "EntityFilter": Sequence[AlfrescoEntityType],
+        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
+        "InclusionPatterns": Sequence[str],
+        "ExclusionPatterns": Sequence[str],
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
     total=False,
 )
 
-class AlfrescoConfigurationOutputTypeDef(
-    _RequiredAlfrescoConfigurationOutputTypeDef, _OptionalAlfrescoConfigurationOutputTypeDef
+class AlfrescoConfigurationTypeDef(
+    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
 OnPremiseConfigurationTypeDef = TypedDict(
     "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
 )
 
-OneDriveUsersOutputTypeDef = TypedDict(
-    "OneDriveUsersOutputTypeDef",
-    {
-        "OneDriveUserList": List[str],
-        "OneDriveUserS3Path": S3PathTypeDef,
-    },
-    total=False,
-)
-
 OneDriveUsersTypeDef = TypedDict(
     "OneDriveUsersTypeDef",
     {
         "OneDriveUserList": Sequence[str],
         "OneDriveUserS3Path": S3PathTypeDef,
     },
     total=False,
@@ -2416,189 +2056,14 @@
 )
 
 class UpdateThesaurusRequestRequestTypeDef(
     _RequiredUpdateThesaurusRequestRequestTypeDef, _OptionalUpdateThesaurusRequestRequestTypeDef
 ):
     pass
 
-_RequiredAlfrescoConfigurationTypeDef = TypedDict(
-    "_RequiredAlfrescoConfigurationTypeDef",
-    {
-        "SiteUrl": str,
-        "SiteId": str,
-        "SecretArn": str,
-        "SslCertificateS3Path": S3PathTypeDef,
-    },
-)
-_OptionalAlfrescoConfigurationTypeDef = TypedDict(
-    "_OptionalAlfrescoConfigurationTypeDef",
-    {
-        "CrawlSystemFolders": bool,
-        "CrawlComments": bool,
-        "EntityFilter": Sequence[AlfrescoEntityType],
-        "DocumentLibraryFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "BlogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WikiFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class AlfrescoConfigurationTypeDef(
-    _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
-):
-    pass
-
-_RequiredBoxConfigurationTypeDef = TypedDict(
-    "_RequiredBoxConfigurationTypeDef",
-    {
-        "EnterpriseId": str,
-        "SecretArn": str,
-    },
-)
-_OptionalBoxConfigurationTypeDef = TypedDict(
-    "_OptionalBoxConfigurationTypeDef",
-    {
-        "UseChangeLog": bool,
-        "CrawlComments": bool,
-        "CrawlTasks": bool,
-        "CrawlWebLinks": bool,
-        "FileFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "TaskFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WebLinkFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
-    pass
-
-DataSourceVpcConfigurationUnionTypeDef = Union[
-    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-]
-_RequiredFsxConfigurationTypeDef = TypedDict(
-    "_RequiredFsxConfigurationTypeDef",
-    {
-        "FileSystemId": str,
-        "FileSystemType": Literal["WINDOWS"],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-)
-_OptionalFsxConfigurationTypeDef = TypedDict(
-    "_OptionalFsxConfigurationTypeDef",
-    {
-        "SecretArn": str,
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class FsxConfigurationTypeDef(_RequiredFsxConfigurationTypeDef, _OptionalFsxConfigurationTypeDef):
-    pass
-
-_RequiredJiraConfigurationTypeDef = TypedDict(
-    "_RequiredJiraConfigurationTypeDef",
-    {
-        "JiraAccountUrl": str,
-        "SecretArn": str,
-    },
-)
-_OptionalJiraConfigurationTypeDef = TypedDict(
-    "_OptionalJiraConfigurationTypeDef",
-    {
-        "UseChangeLog": bool,
-        "Project": Sequence[str],
-        "IssueType": Sequence[str],
-        "Status": Sequence[str],
-        "IssueSubEntityFilter": Sequence[IssueSubEntityType],
-        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "CommentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "IssueFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "ProjectFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "WorkLogFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class JiraConfigurationTypeDef(
-    _RequiredJiraConfigurationTypeDef, _OptionalJiraConfigurationTypeDef
-):
-    pass
-
-_RequiredQuipConfigurationTypeDef = TypedDict(
-    "_RequiredQuipConfigurationTypeDef",
-    {
-        "Domain": str,
-        "SecretArn": str,
-    },
-)
-_OptionalQuipConfigurationTypeDef = TypedDict(
-    "_OptionalQuipConfigurationTypeDef",
-    {
-        "CrawlFileComments": bool,
-        "CrawlChatRooms": bool,
-        "CrawlAttachments": bool,
-        "FolderIds": Sequence[str],
-        "ThreadFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "MessageFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "AttachmentFieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class QuipConfigurationTypeDef(
-    _RequiredQuipConfigurationTypeDef, _OptionalQuipConfigurationTypeDef
-):
-    pass
-
-_RequiredSlackConfigurationTypeDef = TypedDict(
-    "_RequiredSlackConfigurationTypeDef",
-    {
-        "TeamId": str,
-        "SecretArn": str,
-        "SlackEntityList": Sequence[SlackEntityType],
-        "SinceCrawlDate": str,
-    },
-)
-_OptionalSlackConfigurationTypeDef = TypedDict(
-    "_OptionalSlackConfigurationTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
-        "UseChangeLog": bool,
-        "CrawlBotMessage": bool,
-        "ExcludeArchived": bool,
-        "LookBackPeriod": int,
-        "PrivateChannelFilter": Sequence[str],
-        "PublicChannelFilter": Sequence[str],
-        "InclusionPatterns": Sequence[str],
-        "ExclusionPatterns": Sequence[str],
-        "FieldMappings": Sequence[DataSourceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
-class SlackConfigurationTypeDef(
-    _RequiredSlackConfigurationTypeDef, _OptionalSlackConfigurationTypeDef
-):
-    pass
-
 AssociateEntitiesToExperienceRequestRequestTypeDef = TypedDict(
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
         "EntityList": Sequence[EntityConfigurationTypeDef],
     },
@@ -2806,22 +2271,14 @@
     {
         "SuggestableConfigList": Sequence[SuggestableConfigTypeDef],
         "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
     total=False,
 )
 
-AuthenticationConfigurationOutputTypeDef = TypedDict(
-    "AuthenticationConfigurationOutputTypeDef",
-    {
-        "BasicAuthentication": List[BasicAuthenticationConfigurationTypeDef],
-    },
-    total=False,
-)
-
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "BasicAuthentication": Sequence[BasicAuthenticationConfigurationTypeDef],
     },
     total=False,
 )
@@ -2895,88 +2352,31 @@
         "StringListValue": Sequence[str],
         "LongValue": int,
         "DateValue": TimestampTypeDef,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceAttachmentConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
         "CrawlAttachments": bool,
         "AttachmentFieldMappings": Sequence[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-ConfluenceBlogConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceBlogConfigurationOutputTypeDef",
-    {
-        "BlogFieldMappings": List[ConfluenceBlogToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceBlogConfigurationTypeDef = TypedDict(
     "ConfluenceBlogConfigurationTypeDef",
     {
         "BlogFieldMappings": Sequence[ConfluenceBlogToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-_RequiredSharePointConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSharePointConfigurationOutputTypeDef",
-    {
-        "SharePointVersion": SharePointVersionType,
-        "Urls": List[str],
-        "SecretArn": str,
-    },
-)
-_OptionalSharePointConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSharePointConfigurationOutputTypeDef",
-    {
-        "CrawlAttachments": bool,
-        "UseChangeLog": bool,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "DocumentTitleFieldName": str,
-        "DisableLocalGroups": bool,
-        "SslCertificateS3Path": S3PathTypeDef,
-        "AuthenticationType": SharePointOnlineAuthenticationTypeType,
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SharePointConfigurationOutputTypeDef(
-    _RequiredSharePointConfigurationOutputTypeDef, _OptionalSharePointConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredSharePointConfigurationTypeDef = TypedDict(
     "_RequiredSharePointConfigurationTypeDef",
     {
         "SharePointVersion": SharePointVersionType,
         "Urls": Sequence[str],
         "SecretArn": str,
     },
@@ -3000,42 +2400,22 @@
 )
 
 class SharePointConfigurationTypeDef(
     _RequiredSharePointConfigurationTypeDef, _OptionalSharePointConfigurationTypeDef
 ):
     pass
 
-ConfluencePageConfigurationOutputTypeDef = TypedDict(
-    "ConfluencePageConfigurationOutputTypeDef",
-    {
-        "PageFieldMappings": List[ConfluencePageToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluencePageConfigurationTypeDef = TypedDict(
     "ConfluencePageConfigurationTypeDef",
     {
         "PageFieldMappings": Sequence[ConfluencePageToIndexFieldMappingTypeDef],
     },
     total=False,
 )
 
-ConfluenceSpaceConfigurationOutputTypeDef = TypedDict(
-    "ConfluenceSpaceConfigurationOutputTypeDef",
-    {
-        "CrawlPersonalSpaces": bool,
-        "CrawlArchivedSpaces": bool,
-        "IncludeSpaces": List[str],
-        "ExcludeSpaces": List[str],
-        "SpaceFieldMappings": List[ConfluenceSpaceToIndexFieldMappingTypeDef],
-    },
-    total=False,
-)
-
 ConfluenceSpaceConfigurationTypeDef = TypedDict(
     "ConfluenceSpaceConfigurationTypeDef",
     {
         "CrawlPersonalSpaces": bool,
         "CrawlArchivedSpaces": bool,
         "IncludeSpaces": Sequence[str],
         "ExcludeSpaces": Sequence[str],
@@ -3049,21 +2429,14 @@
     {
         "SuggestedQueryText": str,
         "Corrections": List[CorrectionTypeDef],
     },
     total=False,
 )
 
-HierarchicalPrincipalOutputTypeDef = TypedDict(
-    "HierarchicalPrincipalOutputTypeDef",
-    {
-        "PrincipalList": List[PrincipalTypeDef],
-    },
-)
-
 HierarchicalPrincipalTypeDef = TypedDict(
     "HierarchicalPrincipalTypeDef",
     {
         "PrincipalList": Sequence[PrincipalTypeDef],
     },
 )
 
@@ -3294,85 +2667,22 @@
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDocumentAttributeConditionOutputTypeDef = TypedDict(
-    "_RequiredDocumentAttributeConditionOutputTypeDef",
-    {
-        "ConditionDocumentAttributeKey": str,
-        "Operator": ConditionOperatorType,
-    },
-)
-_OptionalDocumentAttributeConditionOutputTypeDef = TypedDict(
-    "_OptionalDocumentAttributeConditionOutputTypeDef",
-    {
-        "ConditionOnValue": DocumentAttributeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-class DocumentAttributeConditionOutputTypeDef(
-    _RequiredDocumentAttributeConditionOutputTypeDef,
-    _OptionalDocumentAttributeConditionOutputTypeDef,
-):
-    pass
-
-DocumentAttributeOutputTypeDef = TypedDict(
-    "DocumentAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": DocumentAttributeValueOutputTypeDef,
-    },
-)
-
-DocumentAttributeTargetOutputTypeDef = TypedDict(
-    "DocumentAttributeTargetOutputTypeDef",
-    {
-        "TargetDocumentAttributeKey": str,
-        "TargetDocumentAttributeValueDeletion": bool,
-        "TargetDocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
-    },
-    total=False,
-)
-
-DocumentAttributeValueCountPairTypeDef = TypedDict(
-    "DocumentAttributeValueCountPairTypeDef",
-    {
-        "DocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
-        "Count": int,
-        "FacetResults": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
-_RequiredDocumentMetadataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDocumentMetadataConfigurationOutputTypeDef",
+DocumentRelevanceConfigurationTypeDef = TypedDict(
+    "DocumentRelevanceConfigurationTypeDef",
     {
         "Name": str,
-        "Type": DocumentAttributeValueTypeType,
-    },
-)
-_OptionalDocumentMetadataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDocumentMetadataConfigurationOutputTypeDef",
-    {
-        "Relevance": RelevanceOutputTypeDef,
-        "Search": SearchTypeDef,
+        "Relevance": RelevanceTypeDef,
     },
-    total=False,
 )
 
-class DocumentMetadataConfigurationOutputTypeDef(
-    _RequiredDocumentMetadataConfigurationOutputTypeDef,
-    _OptionalDocumentMetadataConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredDocumentMetadataConfigurationTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
 )
@@ -3386,45 +2696,14 @@
 )
 
 class DocumentMetadataConfigurationTypeDef(
     _RequiredDocumentMetadataConfigurationTypeDef, _OptionalDocumentMetadataConfigurationTypeDef
 ):
     pass
 
-DocumentRelevanceConfigurationTypeDef = TypedDict(
-    "DocumentRelevanceConfigurationTypeDef",
-    {
-        "Name": str,
-        "Relevance": RelevanceTypeDef,
-    },
-)
-
-_RequiredS3DataSourceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3DataSourceConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3DataSourceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3DataSourceConfigurationOutputTypeDef",
-    {
-        "InclusionPrefixes": List[str],
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "DocumentsMetadataConfiguration": DocumentsMetadataConfigurationTypeDef,
-        "AccessControlListConfiguration": AccessControlListConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class S3DataSourceConfigurationOutputTypeDef(
-    _RequiredS3DataSourceConfigurationOutputTypeDef, _OptionalS3DataSourceConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredS3DataSourceConfigurationTypeDef = TypedDict(
     "_RequiredS3DataSourceConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3DataSourceConfigurationTypeDef = TypedDict(
@@ -3450,23 +2729,14 @@
         "EntityId": str,
         "EntityType": EntityTypeType,
         "DisplayData": EntityDisplayDataTypeDef,
     },
     total=False,
 )
 
-ExperienceConfigurationOutputTypeDef = TypedDict(
-    "ExperienceConfigurationOutputTypeDef",
-    {
-        "ContentSourceConfiguration": ContentSourceConfigurationOutputTypeDef,
-        "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ExperienceConfigurationTypeDef = TypedDict(
     "ExperienceConfigurationTypeDef",
     {
         "ContentSourceConfiguration": ContentSourceConfigurationTypeDef,
         "UserIdentityConfiguration": UserIdentityConfigurationTypeDef,
     },
     total=False,
@@ -3489,22 +2759,46 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
-        "SnapShotTimeFilter": TimeRangeOutputTypeDef,
+        "SnapShotTimeFilter": TimeRangeTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+    },
+)
+_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTimeFilter": TimeRangeTypeDef,
+        "StatusFilter": DataSourceSyncJobStatusType,
+    },
+    total=False,
+)
+
+class ListDataSourceSyncJobsRequestRequestTypeDef(
+    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
+    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
+):
+    pass
+
 GroupMembersTypeDef = TypedDict(
     "GroupMembersTypeDef",
     {
         "MemberGroups": Sequence[MemberGroupTypeDef],
         "MemberUsers": Sequence[MemberUserTypeDef],
         "S3PathforGroupMembers": S3PathTypeDef,
     },
@@ -3578,23 +2872,14 @@
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UrlsOutputTypeDef = TypedDict(
-    "UrlsOutputTypeDef",
-    {
-        "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
-        "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 UrlsTypeDef = TypedDict(
     "UrlsTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationTypeDef,
     },
     total=False,
@@ -3613,37 +2898,14 @@
     "TableRowTypeDef",
     {
         "Cells": List[TableCellTypeDef],
     },
     total=False,
 )
 
-_RequiredDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDatabaseConfigurationOutputTypeDef",
-    {
-        "DatabaseEngineType": DatabaseEngineTypeType,
-        "ConnectionConfiguration": ConnectionConfigurationTypeDef,
-        "ColumnConfiguration": ColumnConfigurationOutputTypeDef,
-    },
-)
-_OptionalDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDatabaseConfigurationOutputTypeDef",
-    {
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "AclConfiguration": AclConfigurationTypeDef,
-        "SqlConfiguration": SqlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class DatabaseConfigurationOutputTypeDef(
-    _RequiredDatabaseConfigurationOutputTypeDef, _OptionalDatabaseConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredDatabaseConfigurationTypeDef",
     {
         "DatabaseEngineType": DatabaseEngineTypeType,
         "ConnectionConfiguration": ConnectionConfigurationTypeDef,
         "ColumnConfiguration": ColumnConfigurationTypeDef,
     },
@@ -3659,39 +2921,14 @@
 )
 
 class DatabaseConfigurationTypeDef(
     _RequiredDatabaseConfigurationTypeDef, _OptionalDatabaseConfigurationTypeDef
 ):
     pass
 
-_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "IncludedStates": List[SalesforceKnowledgeArticleStateType],
-    },
-)
-_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef",
-    {
-        "StandardKnowledgeArticleTypeConfiguration": (
-            SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef
-        ),
-        "CustomKnowledgeArticleTypeConfigurations": List[
-            SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef
-        ],
-    },
-    total=False,
-)
-
-class SalesforceKnowledgeArticleConfigurationOutputTypeDef(
-    _RequiredSalesforceKnowledgeArticleConfigurationOutputTypeDef,
-    _OptionalSalesforceKnowledgeArticleConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceKnowledgeArticleConfigurationTypeDef",
     {
         "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
@@ -3709,37 +2946,14 @@
 
 class SalesforceKnowledgeArticleConfigurationTypeDef(
     _RequiredSalesforceKnowledgeArticleConfigurationTypeDef,
     _OptionalSalesforceKnowledgeArticleConfigurationTypeDef,
 ):
     pass
 
-_RequiredServiceNowConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceNowConfigurationOutputTypeDef",
-    {
-        "HostUrl": str,
-        "SecretArn": str,
-        "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
-    },
-)
-_OptionalServiceNowConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceNowConfigurationOutputTypeDef",
-    {
-        "KnowledgeArticleConfiguration": ServiceNowKnowledgeArticleConfigurationOutputTypeDef,
-        "ServiceCatalogConfiguration": ServiceNowServiceCatalogConfigurationOutputTypeDef,
-        "AuthenticationType": ServiceNowAuthenticationTypeType,
-    },
-    total=False,
-)
-
-class ServiceNowConfigurationOutputTypeDef(
-    _RequiredServiceNowConfigurationOutputTypeDef, _OptionalServiceNowConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredServiceNowConfigurationTypeDef = TypedDict(
     "_RequiredServiceNowConfigurationTypeDef",
     {
         "HostUrl": str,
         "SecretArn": str,
         "ServiceNowBuildVersion": ServiceNowBuildVersionTypeType,
     },
@@ -3755,61 +2969,14 @@
 )
 
 class ServiceNowConfigurationTypeDef(
     _RequiredServiceNowConfigurationTypeDef, _OptionalServiceNowConfigurationTypeDef
 ):
     pass
 
-_RequiredGitHubConfigurationOutputTypeDef = TypedDict(
-    "_RequiredGitHubConfigurationOutputTypeDef",
-    {
-        "SecretArn": str,
-    },
-)
-_OptionalGitHubConfigurationOutputTypeDef = TypedDict(
-    "_OptionalGitHubConfigurationOutputTypeDef",
-    {
-        "SaaSConfiguration": SaaSConfigurationTypeDef,
-        "OnPremiseConfiguration": OnPremiseConfigurationTypeDef,
-        "Type": TypeType,
-        "UseChangeLog": bool,
-        "GitHubDocumentCrawlProperties": GitHubDocumentCrawlPropertiesTypeDef,
-        "RepositoryFilter": List[str],
-        "InclusionFolderNamePatterns": List[str],
-        "InclusionFileTypePatterns": List[str],
-        "InclusionFileNamePatterns": List[str],
-        "ExclusionFolderNamePatterns": List[str],
-        "ExclusionFileTypePatterns": List[str],
-        "ExclusionFileNamePatterns": List[str],
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "GitHubRepositoryConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubCommitConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueDocumentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueCommentConfigurationFieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "GitHubIssueAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestCommentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestDocumentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-        "GitHubPullRequestDocumentAttachmentConfigurationFieldMappings": List[
-            DataSourceToIndexFieldMappingTypeDef
-        ],
-    },
-    total=False,
-)
-
-class GitHubConfigurationOutputTypeDef(
-    _RequiredGitHubConfigurationOutputTypeDef, _OptionalGitHubConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredGitHubConfigurationTypeDef = TypedDict(
     "_RequiredGitHubConfigurationTypeDef",
     {
         "SecretArn": str,
     },
 )
 _OptionalGitHubConfigurationTypeDef = TypedDict(
@@ -3855,38 +3022,14 @@
 )
 
 class GitHubConfigurationTypeDef(
     _RequiredGitHubConfigurationTypeDef, _OptionalGitHubConfigurationTypeDef
 ):
     pass
 
-_RequiredOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOneDriveConfigurationOutputTypeDef",
-    {
-        "TenantDomain": str,
-        "SecretArn": str,
-        "OneDriveUsers": OneDriveUsersOutputTypeDef,
-    },
-)
-_OptionalOneDriveConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOneDriveConfigurationOutputTypeDef",
-    {
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "FieldMappings": List[DataSourceToIndexFieldMappingTypeDef],
-        "DisableLocalGroups": bool,
-    },
-    total=False,
-)
-
-class OneDriveConfigurationOutputTypeDef(
-    _RequiredOneDriveConfigurationOutputTypeDef, _OptionalOneDriveConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredOneDriveConfigurationTypeDef = TypedDict(
     "_RequiredOneDriveConfigurationTypeDef",
     {
         "TenantDomain": str,
         "SecretArn": str,
         "OneDriveUsers": OneDriveUsersTypeDef,
     },
@@ -4004,68 +3147,24 @@
     "DocumentAttributeTypeDef",
     {
         "Key": str,
         "Value": DocumentAttributeValueTypeDef,
     },
 )
 
-_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-    },
-)
-_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTimeFilter": TimeRangeTypeDef,
-        "StatusFilter": DataSourceSyncJobStatusType,
-    },
-    total=False,
-)
-
-class ListDataSourceSyncJobsRequestRequestTypeDef(
-    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
-    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
-):
-    pass
-
-TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
-_RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredConfluenceConfigurationOutputTypeDef",
-    {
-        "ServerUrl": str,
-        "SecretArn": str,
-        "Version": ConfluenceVersionType,
-    },
-)
-_OptionalConfluenceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalConfluenceConfigurationOutputTypeDef",
+DocumentAttributeValueCountPairTypeDef = TypedDict(
+    "DocumentAttributeValueCountPairTypeDef",
     {
-        "SpaceConfiguration": ConfluenceSpaceConfigurationOutputTypeDef,
-        "PageConfiguration": ConfluencePageConfigurationOutputTypeDef,
-        "BlogConfiguration": ConfluenceBlogConfigurationOutputTypeDef,
-        "AttachmentConfiguration": ConfluenceAttachmentConfigurationOutputTypeDef,
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "InclusionPatterns": List[str],
-        "ExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-        "AuthenticationType": ConfluenceAuthenticationTypeType,
+        "DocumentAttributeValue": DocumentAttributeValueTypeDef,
+        "Count": int,
+        "FacetResults": List[Dict[str, Any]],
     },
     total=False,
 )
 
-class ConfluenceConfigurationOutputTypeDef(
-    _RequiredConfluenceConfigurationOutputTypeDef, _OptionalConfluenceConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4087,29 +3186,74 @@
 )
 
 class ConfluenceConfigurationTypeDef(
     _RequiredConfluenceConfigurationTypeDef, _OptionalConfluenceConfigurationTypeDef
 ):
     pass
 
+_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
 DescribeAccessControlConfigurationResponseTypeDef = TypedDict(
     "DescribeAccessControlConfigurationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
-        "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
+        "HierarchicalAccessControlList": List[HierarchicalPrincipalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HierarchicalPrincipalUnionTypeDef = Union[
-    HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef
-]
+_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+    },
+)
+_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
 CreateFeaturedResultsSetResponseTypeDef = TypedDict(
     "CreateFeaturedResultsSetResponseTypeDef",
     {
         "FeaturedResultsSet": FeaturedResultsSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4147,70 +3291,14 @@
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHookConfigurationOutputTypeDef = TypedDict(
-    "_RequiredHookConfigurationOutputTypeDef",
-    {
-        "LambdaArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalHookConfigurationOutputTypeDef = TypedDict(
-    "_OptionalHookConfigurationOutputTypeDef",
-    {
-        "InvocationCondition": DocumentAttributeConditionOutputTypeDef,
-    },
-    total=False,
-)
-
-class HookConfigurationOutputTypeDef(
-    _RequiredHookConfigurationOutputTypeDef, _OptionalHookConfigurationOutputTypeDef
-):
-    pass
-
-RetrieveResultItemTypeDef = TypedDict(
-    "RetrieveResultItemTypeDef",
-    {
-        "Id": str,
-        "DocumentId": str,
-        "DocumentTitle": str,
-        "Content": str,
-        "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
-    },
-    total=False,
-)
-
-SourceDocumentTypeDef = TypedDict(
-    "SourceDocumentTypeDef",
-    {
-        "DocumentId": str,
-        "SuggestionAttributes": List[str],
-        "AdditionalAttributes": List[DocumentAttributeOutputTypeDef],
-    },
-    total=False,
-)
-
-InlineCustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
-    "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    {
-        "Condition": DocumentAttributeConditionOutputTypeDef,
-        "Target": DocumentAttributeTargetOutputTypeDef,
-        "DocumentContentDeletion": bool,
-    },
-    total=False,
-)
-
-DocumentMetadataConfigurationUnionTypeDef = Union[
-    DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef
-]
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4267,32 +3355,14 @@
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeExperienceResponseTypeDef = TypedDict(
-    "DescribeExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Endpoints": List[ExperienceEndpointTypeDef],
-        "Configuration": ExperienceConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": ExperienceStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
     },
 )
@@ -4308,17 +3378,32 @@
 )
 
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
-ExperienceConfigurationUnionTypeDef = Union[
-    ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-]
+DescribeExperienceResponseTypeDef = TypedDict(
+    "DescribeExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Endpoints": List[ExperienceEndpointTypeDef],
+        "Configuration": ExperienceConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": ExperienceStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4405,48 +3490,48 @@
         "Edition": IndexEditionType,
         "RoleArn": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "Status": IndexStatusType,
         "Description": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
-        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationOutputTypeDef],
+        "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationTypeDef],
         "IndexStatistics": IndexStatisticsTypeDef,
         "ErrorMessage": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
-    "_RequiredWebCrawlerConfigurationOutputTypeDef",
+_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIndexRequestRequestTypeDef",
     {
-        "Urls": UrlsOutputTypeDef,
+        "Id": str,
     },
 )
-_OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
-    "_OptionalWebCrawlerConfigurationOutputTypeDef",
+_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIndexRequestRequestTypeDef",
     {
-        "CrawlDepth": int,
-        "MaxLinksPerPage": int,
-        "MaxContentSizePerPageInMegaBytes": float,
-        "MaxUrlsPerMinuteCrawlRate": int,
-        "UrlInclusionPatterns": List[str],
-        "UrlExclusionPatterns": List[str],
-        "ProxyConfiguration": ProxyConfigurationTypeDef,
-        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+        "Name": str,
+        "RoleArn": str,
+        "Description": str,
+        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationTypeDef],
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
     total=False,
 )
 
-class WebCrawlerConfigurationOutputTypeDef(
-    _RequiredWebCrawlerConfigurationOutputTypeDef, _OptionalWebCrawlerConfigurationOutputTypeDef
+class UpdateIndexRequestRequestTypeDef(
+    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
 ):
     pass
 
 _RequiredWebCrawlerConfigurationTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationTypeDef",
     {
         "Urls": UrlsTypeDef,
@@ -4485,42 +3570,14 @@
     {
         "Rows": List[TableRowTypeDef],
         "TotalNumberOfRows": int,
     },
     total=False,
 )
 
-_RequiredSalesforceConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSalesforceConfigurationOutputTypeDef",
-    {
-        "ServerUrl": str,
-        "SecretArn": str,
-    },
-)
-_OptionalSalesforceConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSalesforceConfigurationOutputTypeDef",
-    {
-        "StandardObjectConfigurations": List[SalesforceStandardObjectConfigurationOutputTypeDef],
-        "KnowledgeArticleConfiguration": SalesforceKnowledgeArticleConfigurationOutputTypeDef,
-        "ChatterFeedConfiguration": SalesforceChatterFeedConfigurationOutputTypeDef,
-        "CrawlAttachments": bool,
-        "StandardObjectAttachmentConfiguration": (
-            SalesforceStandardObjectAttachmentConfigurationOutputTypeDef
-        ),
-        "IncludeAttachmentFilePatterns": List[str],
-        "ExcludeAttachmentFilePatterns": List[str],
-    },
-    total=False,
-)
-
-class SalesforceConfigurationOutputTypeDef(
-    _RequiredSalesforceConfigurationOutputTypeDef, _OptionalSalesforceConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredSalesforceConfigurationTypeDef = TypedDict(
     "_RequiredSalesforceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
     },
 )
@@ -4629,62 +3686,37 @@
     },
     total=False,
 )
 
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
-_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+RetrieveResultItemTypeDef = TypedDict(
+    "RetrieveResultItemTypeDef",
     {
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
-        "ClientToken": str,
+        "Id": str,
+        "DocumentId": str,
+        "DocumentTitle": str,
+        "Content": str,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-class CreateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-    },
-)
-_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+SourceDocumentTypeDef = TypedDict(
+    "SourceDocumentTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+        "DocumentId": str,
+        "SuggestionAttributes": List[str],
+        "AdditionalAttributes": List[DocumentAttributeTypeDef],
     },
     total=False,
 )
 
-class UpdateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4700,104 +3732,23 @@
 
 class GetQuerySuggestionsRequestRequestTypeDef(
     _RequiredGetQuerySuggestionsRequestRequestTypeDef,
     _OptionalGetQuerySuggestionsRequestRequestTypeDef,
 ):
     pass
 
-RetrieveResultTypeDef = TypedDict(
-    "RetrieveResultTypeDef",
-    {
-        "QueryId": str,
-        "ResultItems": List[RetrieveResultItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CustomDocumentEnrichmentConfigurationOutputTypeDef = TypedDict(
-    "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    {
-        "InlineConfigurations": List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef],
-        "PreExtractionHookConfiguration": HookConfigurationOutputTypeDef,
-        "PostExtractionHookConfiguration": HookConfigurationOutputTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIndexRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIndexRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-        "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationUnionTypeDef],
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateIndexRequestRequestTypeDef(
-    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
-):
-    pass
-
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
 )
 
-SuggestionTypeDef = TypedDict(
-    "SuggestionTypeDef",
-    {
-        "Id": str,
-        "Value": SuggestionValueTypeDef,
-        "SourceDocuments": List[SourceDocumentTypeDef],
-    },
-    total=False,
-)
-
-DataSourceConfigurationOutputTypeDef = TypedDict(
-    "DataSourceConfigurationOutputTypeDef",
-    {
-        "S3Configuration": S3DataSourceConfigurationOutputTypeDef,
-        "SharePointConfiguration": SharePointConfigurationOutputTypeDef,
-        "DatabaseConfiguration": DatabaseConfigurationOutputTypeDef,
-        "SalesforceConfiguration": SalesforceConfigurationOutputTypeDef,
-        "OneDriveConfiguration": OneDriveConfigurationOutputTypeDef,
-        "ServiceNowConfiguration": ServiceNowConfigurationOutputTypeDef,
-        "ConfluenceConfiguration": ConfluenceConfigurationOutputTypeDef,
-        "GoogleDriveConfiguration": GoogleDriveConfigurationOutputTypeDef,
-        "WebCrawlerConfiguration": WebCrawlerConfigurationOutputTypeDef,
-        "WorkDocsConfiguration": WorkDocsConfigurationOutputTypeDef,
-        "FsxConfiguration": FsxConfigurationOutputTypeDef,
-        "SlackConfiguration": SlackConfigurationOutputTypeDef,
-        "BoxConfiguration": BoxConfigurationOutputTypeDef,
-        "QuipConfiguration": QuipConfigurationOutputTypeDef,
-        "JiraConfiguration": JiraConfigurationOutputTypeDef,
-        "GitHubConfiguration": GitHubConfigurationOutputTypeDef,
-        "AlfrescoConfiguration": AlfrescoConfigurationOutputTypeDef,
-        "TemplateConfiguration": TemplateConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "S3Configuration": S3DataSourceConfigurationTypeDef,
         "SharePointConfiguration": SharePointConfigurationTypeDef,
         "DatabaseConfiguration": DatabaseConfigurationTypeDef,
         "SalesforceConfiguration": SalesforceConfigurationTypeDef,
@@ -4834,25 +3785,44 @@
     "BatchGetDocumentStatusRequestRequestTypeDef",
     {
         "IndexId": str,
         "DocumentInfoList": Sequence[DocumentInfoTypeDef],
     },
 )
 
+RetrieveResultTypeDef = TypedDict(
+    "RetrieveResultTypeDef",
+    {
+        "QueryId": str,
+        "ResultItems": List[RetrieveResultItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SuggestionTypeDef = TypedDict(
+    "SuggestionTypeDef",
+    {
+        "Id": str,
+        "Value": SuggestionValueTypeDef,
+        "SourceDocuments": List[SourceDocumentTypeDef],
+    },
+    total=False,
+)
+
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
         "FeedbackToken": str,
     },
     total=False,
 )
 
 QueryResultItemTypeDef = TypedDict(
     "QueryResultItemTypeDef",
@@ -4861,56 +3831,22 @@
         "Type": QueryResultTypeType,
         "Format": QueryResultFormatType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
         "DocumentId": str,
         "DocumentTitle": TextWithHighlightsTypeDef,
         "DocumentExcerpt": TextWithHighlightsTypeDef,
         "DocumentURI": str,
-        "DocumentAttributes": List[DocumentAttributeOutputTypeDef],
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
         "ScoreAttributes": ScoreAttributesTypeDef,
         "FeedbackToken": str,
         "TableExcerpt": TableExcerptTypeDef,
     },
     total=False,
 )
 
-GetQuerySuggestionsResponseTypeDef = TypedDict(
-    "GetQuerySuggestionsResponseTypeDef",
-    {
-        "QuerySuggestionsId": str,
-        "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourceResponseTypeDef = TypedDict(
-    "DescribeDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Type": DataSourceTypeType,
-        "Configuration": DataSourceConfigurationOutputTypeDef,
-        "VpcConfiguration": DataSourceVpcConfigurationOutputTypeDef,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Description": str,
-        "Status": DataSourceStatusType,
-        "Schedule": str,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "LanguageCode": str,
-        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataSourceConfigurationUnionTypeDef = Union[
-    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-]
 _RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredBatchPutDocumentRequestRequestTypeDef",
     {
         "IndexId": str,
         "Documents": Sequence[DocumentTypeDef],
     },
 )
@@ -4953,17 +3889,36 @@
 )
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
-CustomDocumentEnrichmentConfigurationUnionTypeDef = Union[
-    CustomDocumentEnrichmentConfigurationTypeDef, CustomDocumentEnrichmentConfigurationOutputTypeDef
-]
+DescribeDataSourceResponseTypeDef = TypedDict(
+    "DescribeDataSourceResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Type": DataSourceTypeType,
+        "Configuration": DataSourceConfigurationTypeDef,
+        "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Description": str,
+        "Status": DataSourceStatusType,
+        "Schedule": str,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "LanguageCode": str,
+        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4983,14 +3938,23 @@
 )
 
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
     pass
 
+GetQuerySuggestionsResponseTypeDef = TypedDict(
+    "GetQuerySuggestionsResponseTypeDef",
+    {
+        "QuerySuggestionsId": str,
+        "Suggestions": List[SuggestionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 QueryResultTypeDef = TypedDict(
     "QueryResultTypeDef",
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
```

### Comparing `types-aiobotocore-kendra-2.5.2.post1/types_aiobotocore_kendra.egg-info/SOURCES.txt` & `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

