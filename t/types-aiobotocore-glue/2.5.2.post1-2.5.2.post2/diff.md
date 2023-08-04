# Comparing `tmp/types-aiobotocore-glue-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-glue-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glue-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-glue-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-glue-2.5.2.post1.tar` & `types-aiobotocore-glue-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.381577 types-aiobotocore-glue-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46032 2023-08-02 14:52:21.377577 types-aiobotocore-glue-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44526 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.381577 types-aiobotocore-glue-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.377577 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   143863 2023-08-02 14:39:27.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   143633 2023-08-02 14:39:27.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-08-02 14:39:28.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-02 14:39:28.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-02 14:39:28.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-08-02 14:39:27.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   302998 2023-08-02 14:39:37.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   302531 2023-08-02 14:39:33.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:26.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.377577 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46032 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:21.000000 types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.224356 types-aiobotocore-glue-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-04 12:00:58.224356 types-aiobotocore-glue-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.224356 types-aiobotocore-glue-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.204355 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143723 2023-08-04 11:46:59.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143493 2023-08-04 11:46:59.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-08-04 11:47:00.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-04 11:47:00.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-04 11:47:00.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-08-04 11:47:00.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   253061 2023-08-04 11:47:07.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   252686 2023-08-04 11:47:04.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.224356 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 12:00:58.000000 types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glue-2.5.2.post1/LICENSE` & `types-aiobotocore-glue-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/setup.py` & `types-aiobotocore-glue-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glue",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__init__.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__init__.pyi` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/__main__.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glue 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Glue 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
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

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/client.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     GetTriggersPaginator,
     GetUserDefinedFunctionsPaginator,
     ListRegistriesPaginator,
     ListSchemasPaginator,
     ListSchemaVersionsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
+    ActionTypeDef,
     AuditContextTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
@@ -74,21 +74,21 @@
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CatalogEntryTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
-    CodeGenConfigurationNodeUnionTypeDef,
+    CodeGenConfigurationNodeTypeDef,
     CodeGenEdgeTypeDef,
-    CodeGenNodeUnionTypeDef,
-    ColumnStatisticsUnionTypeDef,
+    CodeGenNodeTypeDef,
+    ColumnStatisticsTypeDef,
     ConnectionInputTypeDef,
-    ConnectionsListUnionTypeDef,
-    CrawlerTargetsUnionTypeDef,
+    ConnectionsListTypeDef,
+    CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
     CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
@@ -107,27 +107,27 @@
     DataCatalogEncryptionSettingsTypeDef,
     DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
     DataQualityResultFilterCriteriaTypeDef,
     DataQualityRuleRecommendationRunFilterTypeDef,
     DataQualityRulesetEvaluationRunFilterTypeDef,
     DataQualityRulesetFilterCriteriaTypeDef,
     DataQualityTargetTableTypeDef,
-    DataSourceUnionTypeDef,
+    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     DeleteSessionResponseTypeDef,
     DeleteTriggerResponseTypeDef,
     DeleteWorkflowResponseTypeDef,
     DevEndpointCustomLibrariesTypeDef,
-    EncryptionConfigurationUnionTypeDef,
+    EncryptionConfigurationTypeDef,
     EventBatchingConditionTypeDef,
     ExecutionPropertyTypeDef,
     GetBlueprintResponseTypeDef,
     GetBlueprintRunResponseTypeDef,
     GetBlueprintRunsResponseTypeDef,
     GetCatalogImportStatusResponseTypeDef,
     GetClassifierResponseTypeDef,
@@ -188,15 +188,15 @@
     GetUnfilteredTableMetadataResponseTypeDef,
     GetUserDefinedFunctionResponseTypeDef,
     GetUserDefinedFunctionsResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowRunPropertiesResponseTypeDef,
     GetWorkflowRunResponseTypeDef,
     GetWorkflowRunsResponseTypeDef,
-    GlueTableUnionTypeDef,
+    GlueTableTypeDef,
     JobCommandTypeDef,
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
@@ -217,16 +217,16 @@
     ListWorkflowsResponseTypeDef,
     LocationTypeDef,
     MappingEntryTypeDef,
     MetadataKeyValuePairTypeDef,
     NotificationPropertyTypeDef,
     PartitionIndexTypeDef,
     PartitionInputTypeDef,
-    PartitionValueListUnionTypeDef,
-    PredicateUnionTypeDef,
+    PartitionValueListTypeDef,
+    PredicateTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
     QuerySchemaVersionMetadataResponseTypeDef,
     RecrawlPolicyTypeDef,
     RegisterSchemaVersionResponseTypeDef,
     RegistryIdTypeDef,
@@ -378,15 +378,15 @@
         """
 
     async def batch_delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        PartitionsToDelete: Sequence[PartitionValueListUnionTypeDef],
+        PartitionsToDelete: Sequence[PartitionValueListTypeDef],
         CatalogId: str = ...
     ) -> BatchDeletePartitionResponseTypeDef:
         """
         Deletes one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_partition)
@@ -481,15 +481,15 @@
         """
 
     async def batch_get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        PartitionsToGet: Sequence[PartitionValueListUnionTypeDef],
+        PartitionsToGet: Sequence[PartitionValueListTypeDef],
         CatalogId: str = ...
     ) -> BatchGetPartitionResponseTypeDef:
         """
         Retrieves partitions in a batch request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_partition)
@@ -647,15 +647,15 @@
         """
 
     async def create_crawler(
         self,
         *,
         Name: str,
         Role: str,
-        Targets: CrawlerTargetsUnionTypeDef,
+        Targets: CrawlerTargetsTypeDef,
         DatabaseName: str = ...,
         Description: str = ...,
         Schedule: str = ...,
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
@@ -754,41 +754,41 @@
         Role: str,
         Command: JobCommandTypeDef,
         Description: str = ...,
         LogUri: str = ...,
         ExecutionProperty: ExecutionPropertyTypeDef = ...,
         DefaultArguments: Mapping[str, str] = ...,
         NonOverridableArguments: Mapping[str, str] = ...,
-        Connections: ConnectionsListUnionTypeDef = ...,
+        Connections: ConnectionsListTypeDef = ...,
         MaxRetries: int = ...,
         AllocatedCapacity: int = ...,
         Timeout: int = ...,
         MaxCapacity: float = ...,
         SecurityConfiguration: str = ...,
         Tags: Mapping[str, str] = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
-        CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeUnionTypeDef] = ...,
+        CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeTypeDef] = ...,
         ExecutionClass: ExecutionClassType = ...,
         SourceControlDetails: SourceControlDetailsTypeDef = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a new job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_job)
         """
 
     async def create_ml_transform(
         self,
         *,
         Name: str,
-        InputRecordTables: Sequence[GlueTableUnionTypeDef],
+        InputRecordTables: Sequence[GlueTableTypeDef],
         Parameters: TransformParametersTypeDef,
         Role: str,
         Description: str = ...,
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
@@ -861,27 +861,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_schema)
         """
 
     async def create_script(
         self,
         *,
-        DagNodes: Sequence[CodeGenNodeUnionTypeDef] = ...,
+        DagNodes: Sequence[CodeGenNodeTypeDef] = ...,
         DagEdges: Sequence[CodeGenEdgeTypeDef] = ...,
         Language: LanguageType = ...
     ) -> CreateScriptResponseTypeDef:
         """
         Transforms a directed acyclic graph (DAG) into code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_script)
         """
 
     async def create_security_configuration(
-        self, *, Name: str, EncryptionConfiguration: EncryptionConfigurationUnionTypeDef
+        self, *, Name: str, EncryptionConfiguration: EncryptionConfigurationTypeDef
     ) -> CreateSecurityConfigurationResponseTypeDef:
         """
         Creates a new security configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_security_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_security_configuration)
         """
@@ -892,15 +892,15 @@
         Id: str,
         Role: str,
         Command: SessionCommandTypeDef,
         Description: str = ...,
         Timeout: int = ...,
         IdleTimeout: int = ...,
         DefaultArguments: Mapping[str, str] = ...,
-        Connections: ConnectionsListUnionTypeDef = ...,
+        Connections: ConnectionsListTypeDef = ...,
         MaxCapacity: float = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         SecurityConfiguration: str = ...,
         GlueVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         RequestOrigin: str = ...
@@ -929,18 +929,18 @@
         """
 
     async def create_trigger(
         self,
         *,
         Name: str,
         Type: TriggerTypeType,
-        Actions: Sequence[ActionUnionTypeDef],
+        Actions: Sequence[ActionTypeDef],
         WorkflowName: str = ...,
         Schedule: str = ...,
-        Predicate: PredicateUnionTypeDef = ...,
+        Predicate: PredicateTypeDef = ...,
         Description: str = ...,
         StartOnCreation: bool = ...,
         Tags: Mapping[str, str] = ...,
         EventBatchingCondition: EventBatchingConditionTypeDef = ...
     ) -> CreateTriggerResponseTypeDef:
         """
         Creates a new trigger.
@@ -2384,15 +2384,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_crawler_schedule)
         """
 
     async def start_data_quality_rule_recommendation_run(
         self,
         *,
-        DataSource: DataSourceUnionTypeDef,
+        DataSource: DataSourceTypeDef,
         Role: str,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         CreatedRulesetName: str = ...,
         ClientToken: str = ...
     ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
         """
@@ -2402,22 +2402,22 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_data_quality_rule_recommendation_run)
         """
 
     async def start_data_quality_ruleset_evaluation_run(
         self,
         *,
-        DataSource: DataSourceUnionTypeDef,
+        DataSource: DataSourceTypeDef,
         Role: str,
         RulesetNames: Sequence[str],
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         ClientToken: str = ...,
         AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
-        AdditionalDataSources: Mapping[str, DataSourceUnionTypeDef] = ...
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
     ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
         """
         Once you have a ruleset definition (either recommended or your own), you call
         this operation to evaluate the ruleset against a data source (Glue table).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_data_quality_ruleset_evaluation_run)
@@ -2597,30 +2597,30 @@
 
     async def update_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],
+        ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
         CatalogId: str = ...
     ) -> UpdateColumnStatisticsForPartitionResponseTypeDef:
         """
         Creates or updates partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_partition)
         """
 
     async def update_column_statistics_for_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],
+        ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
         CatalogId: str = ...
     ) -> UpdateColumnStatisticsForTableResponseTypeDef:
         """
         Creates or updates table statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_table)
@@ -2639,15 +2639,15 @@
     async def update_crawler(
         self,
         *,
         Name: str,
         Role: str = ...,
         DatabaseName: str = ...,
         Description: str = ...,
-        Targets: CrawlerTargetsUnionTypeDef = ...,
+        Targets: CrawlerTargetsTypeDef = ...,
         Schedule: str = ...,
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
```

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/client.pyi` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     GetTriggersPaginator,
     GetUserDefinedFunctionsPaginator,
     ListRegistriesPaginator,
     ListSchemasPaginator,
     ListSchemaVersionsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
+    ActionTypeDef,
     AuditContextTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
@@ -74,21 +74,21 @@
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CatalogEntryTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
-    CodeGenConfigurationNodeUnionTypeDef,
+    CodeGenConfigurationNodeTypeDef,
     CodeGenEdgeTypeDef,
-    CodeGenNodeUnionTypeDef,
-    ColumnStatisticsUnionTypeDef,
+    CodeGenNodeTypeDef,
+    ColumnStatisticsTypeDef,
     ConnectionInputTypeDef,
-    ConnectionsListUnionTypeDef,
-    CrawlerTargetsUnionTypeDef,
+    ConnectionsListTypeDef,
+    CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
     CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
@@ -107,27 +107,27 @@
     DataCatalogEncryptionSettingsTypeDef,
     DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
     DataQualityResultFilterCriteriaTypeDef,
     DataQualityRuleRecommendationRunFilterTypeDef,
     DataQualityRulesetEvaluationRunFilterTypeDef,
     DataQualityRulesetFilterCriteriaTypeDef,
     DataQualityTargetTableTypeDef,
-    DataSourceUnionTypeDef,
+    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     DeleteSessionResponseTypeDef,
     DeleteTriggerResponseTypeDef,
     DeleteWorkflowResponseTypeDef,
     DevEndpointCustomLibrariesTypeDef,
-    EncryptionConfigurationUnionTypeDef,
+    EncryptionConfigurationTypeDef,
     EventBatchingConditionTypeDef,
     ExecutionPropertyTypeDef,
     GetBlueprintResponseTypeDef,
     GetBlueprintRunResponseTypeDef,
     GetBlueprintRunsResponseTypeDef,
     GetCatalogImportStatusResponseTypeDef,
     GetClassifierResponseTypeDef,
@@ -188,15 +188,15 @@
     GetUnfilteredTableMetadataResponseTypeDef,
     GetUserDefinedFunctionResponseTypeDef,
     GetUserDefinedFunctionsResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowRunPropertiesResponseTypeDef,
     GetWorkflowRunResponseTypeDef,
     GetWorkflowRunsResponseTypeDef,
-    GlueTableUnionTypeDef,
+    GlueTableTypeDef,
     JobCommandTypeDef,
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
@@ -217,16 +217,16 @@
     ListWorkflowsResponseTypeDef,
     LocationTypeDef,
     MappingEntryTypeDef,
     MetadataKeyValuePairTypeDef,
     NotificationPropertyTypeDef,
     PartitionIndexTypeDef,
     PartitionInputTypeDef,
-    PartitionValueListUnionTypeDef,
-    PredicateUnionTypeDef,
+    PartitionValueListTypeDef,
+    PredicateTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
     QuerySchemaVersionMetadataResponseTypeDef,
     RecrawlPolicyTypeDef,
     RegisterSchemaVersionResponseTypeDef,
     RegistryIdTypeDef,
@@ -371,15 +371,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_connection)
         """
     async def batch_delete_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        PartitionsToDelete: Sequence[PartitionValueListUnionTypeDef],
+        PartitionsToDelete: Sequence[PartitionValueListTypeDef],
         CatalogId: str = ...
     ) -> BatchDeletePartitionResponseTypeDef:
         """
         Deletes one or more partitions in a batch operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_delete_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_delete_partition)
@@ -465,15 +465,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_jobs)
         """
     async def batch_get_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        PartitionsToGet: Sequence[PartitionValueListUnionTypeDef],
+        PartitionsToGet: Sequence[PartitionValueListTypeDef],
         CatalogId: str = ...
     ) -> BatchGetPartitionResponseTypeDef:
         """
         Retrieves partitions in a batch request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#batch_get_partition)
@@ -616,15 +616,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_connection)
         """
     async def create_crawler(
         self,
         *,
         Name: str,
         Role: str,
-        Targets: CrawlerTargetsUnionTypeDef,
+        Targets: CrawlerTargetsTypeDef,
         DatabaseName: str = ...,
         Description: str = ...,
         Schedule: str = ...,
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
@@ -718,40 +718,40 @@
         Role: str,
         Command: JobCommandTypeDef,
         Description: str = ...,
         LogUri: str = ...,
         ExecutionProperty: ExecutionPropertyTypeDef = ...,
         DefaultArguments: Mapping[str, str] = ...,
         NonOverridableArguments: Mapping[str, str] = ...,
-        Connections: ConnectionsListUnionTypeDef = ...,
+        Connections: ConnectionsListTypeDef = ...,
         MaxRetries: int = ...,
         AllocatedCapacity: int = ...,
         Timeout: int = ...,
         MaxCapacity: float = ...,
         SecurityConfiguration: str = ...,
         Tags: Mapping[str, str] = ...,
         NotificationProperty: NotificationPropertyTypeDef = ...,
         GlueVersion: str = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
-        CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeUnionTypeDef] = ...,
+        CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeTypeDef] = ...,
         ExecutionClass: ExecutionClassType = ...,
         SourceControlDetails: SourceControlDetailsTypeDef = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a new job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_job)
         """
     async def create_ml_transform(
         self,
         *,
         Name: str,
-        InputRecordTables: Sequence[GlueTableUnionTypeDef],
+        InputRecordTables: Sequence[GlueTableTypeDef],
         Parameters: TransformParametersTypeDef,
         Role: str,
         Description: str = ...,
         GlueVersion: str = ...,
         MaxCapacity: float = ...,
         WorkerType: WorkerTypeType = ...,
         NumberOfWorkers: int = ...,
@@ -819,26 +819,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_schema)
         """
     async def create_script(
         self,
         *,
-        DagNodes: Sequence[CodeGenNodeUnionTypeDef] = ...,
+        DagNodes: Sequence[CodeGenNodeTypeDef] = ...,
         DagEdges: Sequence[CodeGenEdgeTypeDef] = ...,
         Language: LanguageType = ...
     ) -> CreateScriptResponseTypeDef:
         """
         Transforms a directed acyclic graph (DAG) into code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_script)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_script)
         """
     async def create_security_configuration(
-        self, *, Name: str, EncryptionConfiguration: EncryptionConfigurationUnionTypeDef
+        self, *, Name: str, EncryptionConfiguration: EncryptionConfigurationTypeDef
     ) -> CreateSecurityConfigurationResponseTypeDef:
         """
         Creates a new security configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_security_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_security_configuration)
         """
@@ -848,15 +848,15 @@
         Id: str,
         Role: str,
         Command: SessionCommandTypeDef,
         Description: str = ...,
         Timeout: int = ...,
         IdleTimeout: int = ...,
         DefaultArguments: Mapping[str, str] = ...,
-        Connections: ConnectionsListUnionTypeDef = ...,
+        Connections: ConnectionsListTypeDef = ...,
         MaxCapacity: float = ...,
         NumberOfWorkers: int = ...,
         WorkerType: WorkerTypeType = ...,
         SecurityConfiguration: str = ...,
         GlueVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         RequestOrigin: str = ...
@@ -883,18 +883,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table)
         """
     async def create_trigger(
         self,
         *,
         Name: str,
         Type: TriggerTypeType,
-        Actions: Sequence[ActionUnionTypeDef],
+        Actions: Sequence[ActionTypeDef],
         WorkflowName: str = ...,
         Schedule: str = ...,
-        Predicate: PredicateUnionTypeDef = ...,
+        Predicate: PredicateTypeDef = ...,
         Description: str = ...,
         StartOnCreation: bool = ...,
         Tags: Mapping[str, str] = ...,
         EventBatchingCondition: EventBatchingConditionTypeDef = ...
     ) -> CreateTriggerResponseTypeDef:
         """
         Creates a new trigger.
@@ -2211,15 +2211,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_crawler_schedule)
         """
     async def start_data_quality_rule_recommendation_run(
         self,
         *,
-        DataSource: DataSourceUnionTypeDef,
+        DataSource: DataSourceTypeDef,
         Role: str,
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         CreatedRulesetName: str = ...,
         ClientToken: str = ...
     ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
         """
@@ -2228,22 +2228,22 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_data_quality_rule_recommendation_run)
         """
     async def start_data_quality_ruleset_evaluation_run(
         self,
         *,
-        DataSource: DataSourceUnionTypeDef,
+        DataSource: DataSourceTypeDef,
         Role: str,
         RulesetNames: Sequence[str],
         NumberOfWorkers: int = ...,
         Timeout: int = ...,
         ClientToken: str = ...,
         AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
-        AdditionalDataSources: Mapping[str, DataSourceUnionTypeDef] = ...
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
     ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
         """
         Once you have a ruleset definition (either recommended or your own), you call
         this operation to evaluate the ruleset against a data source (Glue table).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#start_data_quality_ruleset_evaluation_run)
@@ -2406,29 +2406,29 @@
         """
     async def update_column_statistics_for_partition(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
-        ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],
+        ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
         CatalogId: str = ...
     ) -> UpdateColumnStatisticsForPartitionResponseTypeDef:
         """
         Creates or updates partition statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_partition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_partition)
         """
     async def update_column_statistics_for_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
-        ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],
+        ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],
         CatalogId: str = ...
     ) -> UpdateColumnStatisticsForTableResponseTypeDef:
         """
         Creates or updates table statistics of columns.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_column_statistics_for_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#update_column_statistics_for_table)
@@ -2445,15 +2445,15 @@
     async def update_crawler(
         self,
         *,
         Name: str,
         Role: str = ...,
         DatabaseName: str = ...,
         Description: str = ...,
-        Targets: CrawlerTargetsUnionTypeDef = ...,
+        Targets: CrawlerTargetsTypeDef = ...,
         Schedule: str = ...,
         Classifiers: Sequence[str] = ...,
         TablePrefix: str = ...,
         SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,
         RecrawlPolicy: RecrawlPolicyTypeDef = ...,
         LineageConfiguration: LineageConfigurationTypeDef = ...,
         LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,
```

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/literals.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/literals.pyi` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/paginator.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/paginator.pyi` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/type_defs.py` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_glue.type_defs import NotificationPropertyTypeDef
 
     data: NotificationPropertyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Mapping, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
@@ -109,23 +107,20 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "NotificationPropertyTypeDef",
-    "AggregateOperationOutputTypeDef",
     "AggregateOperationTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
     "OptionTypeDef",
-    "ApplyMappingOutputTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
-    "PartitionValueListOutputTypeDef",
-    "BasicCatalogTargetOutputTypeDef",
+    "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
@@ -137,104 +132,80 @@
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
-    "BlobTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
     "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
-    "KafkaStreamingSourceOptionsOutputTypeDef",
+    "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
-    "KinesisStreamingSourceOptionsOutputTypeDef",
+    "KinesisStreamingSourceOptionsTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
     "CatalogSourceTypeDef",
-    "CatalogTargetOutputTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
     "DirectJDBCSourceTypeDef",
-    "DropDuplicatesOutputTypeDef",
-    "DropFieldsOutputTypeDef",
-    "DynamoDBCatalogSourceTypeDef",
-    "FillMissingValuesOutputTypeDef",
-    "MergeOutputTypeDef",
-    "MicrosoftSQLServerCatalogSourceTypeDef",
-    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
-    "MySQLCatalogSourceTypeDef",
-    "MySQLCatalogTargetOutputTypeDef",
-    "OracleSQLCatalogSourceTypeDef",
-    "OracleSQLCatalogTargetOutputTypeDef",
-    "PIIDetectionOutputTypeDef",
-    "PostgreSQLCatalogSourceTypeDef",
-    "PostgreSQLCatalogTargetOutputTypeDef",
-    "RedshiftSourceTypeDef",
-    "RelationalCatalogSourceTypeDef",
-    "RenameFieldOutputTypeDef",
-    "SelectFieldsOutputTypeDef",
-    "SelectFromCollectionOutputTypeDef",
-    "SpigotOutputTypeDef",
-    "SplitFieldsOutputTypeDef",
-    "UnionOutputTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
+    "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
+    "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
+    "MySQLCatalogSourceTypeDef",
     "MySQLCatalogTargetTypeDef",
+    "OracleSQLCatalogSourceTypeDef",
     "OracleSQLCatalogTargetTypeDef",
     "PIIDetectionTypeDef",
+    "PostgreSQLCatalogSourceTypeDef",
     "PostgreSQLCatalogTargetTypeDef",
+    "RedshiftSourceTypeDef",
+    "RelationalCatalogSourceTypeDef",
     "RenameFieldTypeDef",
     "SelectFieldsTypeDef",
     "SelectFromCollectionTypeDef",
     "SpigotTypeDef",
     "SplitFieldsTypeDef",
     "UnionTypeDef",
     "CodeGenEdgeTypeDef",
     "CodeGenNodeArgTypeDef",
     "ColumnImportanceTypeDef",
-    "ColumnOutputTypeDef",
     "ColumnRowFilterTypeDef",
-    "DateColumnStatisticsDataOutputTypeDef",
+    "DateColumnStatisticsDataTypeDef",
     "DoubleColumnStatisticsDataTypeDef",
     "LongColumnStatisticsDataTypeDef",
     "StringColumnStatisticsDataTypeDef",
-    "TimestampTypeDef",
     "ColumnTypeDef",
     "ConditionTypeDef",
     "ConfusionMatrixTypeDef",
     "PhysicalConnectionRequirementsTypeDef",
     "ConnectionPasswordEncryptionTypeDef",
-    "PhysicalConnectionRequirementsOutputTypeDef",
-    "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
-    "DeltaTargetOutputTypeDef",
-    "DynamoDBTargetTypeDef",
-    "JdbcTargetOutputTypeDef",
-    "MongoDBTargetTypeDef",
-    "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
+    "DynamoDBTargetTypeDef",
     "JdbcTargetTypeDef",
+    "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
     "ScheduleTypeDef",
     "SchemaChangePolicyTypeDef",
@@ -246,32 +217,32 @@
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
     "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
+    "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "DQResultsPublishingOptionsTypeDef",
     "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    "TimestampTypeDef",
     "DataQualityRuleResultTypeDef",
-    "GlueTableOutputTypeDef",
-    "GlueTableTypeDef",
     "DatabaseIdentifierTypeDef",
     "FederatedDatabaseTypeDef",
     "DatatypeTypeDef",
-    "DecimalNumberOutputTypeDef",
+    "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
@@ -290,23 +261,21 @@
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
-    "TransformConfigParameterOutputTypeDef",
     "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FederatedTableTypeDef",
-    "FilterValueOutputTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
@@ -365,18 +334,16 @@
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
-    "JDBCConnectorOptionsOutputTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
-    "JoinColumnOutputTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
     "ListCrawlersRequestRequestTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
@@ -386,34 +353,29 @@
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MLUserDataEncryptionTypeDef",
-    "MappingOutputTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
-    "PartitionValueListTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
-    "UpsertRedshiftTargetOptionsOutputTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
-    "SerDeInfoOutputTypeDef",
     "SerDeInfoTypeDef",
-    "SkewedInfoOutputTypeDef",
     "SkewedInfoTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
@@ -438,24 +400,23 @@
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "AggregateOutputTypeDef",
     "AggregateTypeDef",
-    "AmazonRedshiftNodeDataOutputTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
+    "BatchDeletePartitionRequestRequestTypeDef",
+    "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
     "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
@@ -527,98 +488,75 @@
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
     "BatchGetCustomEntityTypesResponseTypeDef",
     "ListCustomEntityTypesResponseTypeDef",
     "BatchGetDevEndpointsResponseTypeDef",
     "GetDevEndpointResponseTypeDef",
     "GetDevEndpointsResponseTypeDef",
-    "DecimalNumberTypeDef",
     "GetBlueprintRunResponseTypeDef",
     "GetBlueprintRunsResponseTypeDef",
     "BlueprintTypeDef",
     "GetCatalogImportStatusResponseTypeDef",
-    "CatalogKafkaSourceOutputTypeDef",
-    "DirectKafkaSourceOutputTypeDef",
-    "CatalogKinesisSourceOutputTypeDef",
-    "DirectKinesisSourceOutputTypeDef",
-    "GovernedCatalogTargetOutputTypeDef",
+    "CatalogKafkaSourceTypeDef",
+    "DirectKafkaSourceTypeDef",
+    "CatalogKinesisSourceTypeDef",
+    "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
-    "S3CatalogTargetOutputTypeDef",
     "S3CatalogTargetTypeDef",
-    "S3DeltaCatalogTargetOutputTypeDef",
     "S3DeltaCatalogTargetTypeDef",
-    "S3HudiCatalogTargetOutputTypeDef",
     "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
-    "CodeGenNodeOutputTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
-    "DateColumnStatisticsDataTypeDef",
-    "GetTableRequestRequestTypeDef",
-    "GetTablesRequestRequestTypeDef",
-    "KafkaStreamingSourceOptionsTypeDef",
-    "KinesisStreamingSourceOptionsTypeDef",
-    "TaskRunFilterCriteriaTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
-    "ConnectionsListUnionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
-    "CrawlerTargetsOutputTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
     "CreateDataQualityRulesetRequestRequestTypeDef",
-    "DataQualityRulesetFilterCriteriaTypeDef",
     "DataQualityRulesetListDetailsTypeDef",
     "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
-    "EvaluateDataQualityMultiFrameOutputTypeDef",
     "EvaluateDataQualityMultiFrameTypeDef",
-    "EvaluateDataQualityOutputTypeDef",
     "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
-    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
-    "DataSourceOutputTypeDef",
-    "DataSourceTypeDef",
-    "GlueTableUnionTypeDef",
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    "GetTableRequestRequestTypeDef",
+    "GetTablesRequestRequestTypeDef",
+    "TaskRunFilterCriteriaTypeDef",
     "NullValueFieldTypeDef",
-    "DecimalColumnStatisticsDataOutputTypeDef",
+    "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
-    "S3DeltaDirectTargetOutputTypeDef",
     "S3DeltaDirectTargetTypeDef",
-    "S3DirectTargetOutputTypeDef",
     "S3DirectTargetTypeDef",
-    "S3GlueParquetTargetOutputTypeDef",
     "S3GlueParquetTargetTypeDef",
-    "S3HudiDirectTargetOutputTypeDef",
     "S3HudiDirectTargetTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
-    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
@@ -643,128 +581,94 @@
     "GetPartitionsRequestGetPartitionsPaginateTypeDef",
     "GetPartitionsRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
-    "GlueSchemaOutputTypeDef",
     "GlueSchemaTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
     "JobRunTypeDef",
-    "JoinOutputTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
-    "PartitionValueListUnionTypeDef",
-    "RedshiftTargetOutputTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
-    "ActionUnionTypeDef",
-    "AmazonRedshiftSourceOutputTypeDef",
-    "AmazonRedshiftTargetOutputTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
-    "DecimalColumnStatisticsDataTypeDef",
     "BatchGetBlueprintsResponseTypeDef",
     "GetBlueprintResponseTypeDef",
     "GetClassifierResponseTypeDef",
     "GetClassifiersResponseTypeDef",
+    "CreateScriptRequestRequestTypeDef",
     "GetDataflowGraphResponseTypeDef",
-    "CodeGenNodeUnionTypeDef",
     "GetMappingRequestRequestTypeDef",
     "GetPlanRequestRequestTypeDef",
-    "CatalogKafkaSourceTypeDef",
-    "DirectKafkaSourceTypeDef",
-    "CatalogKinesisSourceTypeDef",
-    "DirectKinesisSourceTypeDef",
-    "GetMLTaskRunsRequestRequestTypeDef",
+    "CreateTriggerRequestRequestTypeDef",
     "TriggerTypeDef",
-    "PredicateUnionTypeDef",
     "TriggerUpdateTypeDef",
     "EvaluationMetricsTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
-    "CrawlerTargetsUnionTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
-    "ListDataQualityRulesetsRequestRequestTypeDef",
     "ListDataQualityRulesetsResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
-    "ListSessionsResponseTypeDef",
-    "GetDataCatalogEncryptionSettingsResponseTypeDef",
-    "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "DatabaseTypeDef",
-    "DatabaseInputTypeDef",
     "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultFilterCriteriaTypeDef",
     "DataQualityResultTypeDef",
     "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRuleRecommendationRunFilterTypeDef",
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunFilterTypeDef",
     "GetDataQualityResultResponseTypeDef",
     "GetDataQualityRuleRecommendationRunResponseTypeDef",
     "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "DataSourceUnionTypeDef",
     "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "DropNullFieldsOutputTypeDef",
+    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "ListSessionsResponseTypeDef",
+    "GetDataCatalogEncryptionSettingsResponseTypeDef",
+    "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    "DatabaseInputTypeDef",
+    "DatabaseTypeDef",
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    "GetMLTaskRunsRequestRequestTypeDef",
     "DropNullFieldsTypeDef",
-    "ColumnStatisticsDataOutputTypeDef",
-    "StorageDescriptorOutputTypeDef",
+    "ColumnStatisticsDataTypeDef",
     "StorageDescriptorTypeDef",
-    "SecurityConfigurationTypeDef",
     "CreateSecurityConfigurationRequestRequestTypeDef",
-    "EncryptionConfigurationUnionTypeDef",
+    "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
-    "AthenaConnectorSourceOutputTypeDef",
-    "CatalogDeltaSourceOutputTypeDef",
-    "CatalogHudiSourceOutputTypeDef",
-    "CustomCodeOutputTypeDef",
-    "DynamicTransformOutputTypeDef",
-    "JDBCConnectorSourceOutputTypeDef",
-    "JDBCConnectorTargetOutputTypeDef",
-    "S3CatalogDeltaSourceOutputTypeDef",
-    "S3CatalogHudiSourceOutputTypeDef",
-    "S3CsvSourceOutputTypeDef",
-    "S3DeltaSourceOutputTypeDef",
-    "S3HudiSourceOutputTypeDef",
-    "S3JsonSourceOutputTypeDef",
-    "S3ParquetSourceOutputTypeDef",
-    "SparkConnectorSourceOutputTypeDef",
-    "SparkConnectorTargetOutputTypeDef",
-    "SparkSQLOutputTypeDef",
     "AthenaConnectorSourceTypeDef",
     "CatalogDeltaSourceTypeDef",
     "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
@@ -781,100 +685,90 @@
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
     "TaskRunTypeDef",
     "CreateMLTransformRequestRequestTypeDef",
     "QuerySchemaVersionMetadataResponseTypeDef",
-    "BatchDeletePartitionRequestRequestTypeDef",
-    "BatchGetPartitionRequestRequestTypeDef",
     "CreateUserDefinedFunctionRequestRequestTypeDef",
     "UpdateUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionResponseTypeDef",
     "GetUserDefinedFunctionsResponseTypeDef",
     "StatementTypeDef",
-    "CreateTriggerRequestRequestTypeDef",
     "GetPartitionIndexesResponseTypeDef",
-    "ColumnStatisticsDataTypeDef",
-    "CreateScriptRequestRequestTypeDef",
     "BatchGetTriggersResponseTypeDef",
     "GetTriggerResponseTypeDef",
     "GetTriggersResponseTypeDef",
     "TriggerNodeDetailsTypeDef",
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "GetDatabaseResponseTypeDef",
-    "GetDatabasesResponseTypeDef",
-    "CreateDatabaseRequestRequestTypeDef",
-    "UpdateDatabaseRequestRequestTypeDef",
     "ListDataQualityResultsResponseTypeDef",
+    "ListDataQualityResultsRequestRequestTypeDef",
     "BatchGetDataQualityResultResponseTypeDef",
     "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    "ListDataQualityResultsRequestRequestTypeDef",
     "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
     "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "ColumnStatisticsOutputTypeDef",
-    "PartitionTypeDef",
-    "TableTypeDef",
+    "CreateDatabaseRequestRequestTypeDef",
+    "UpdateDatabaseRequestRequestTypeDef",
+    "GetDatabaseResponseTypeDef",
+    "GetDatabasesResponseTypeDef",
+    "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
+    "PartitionTypeDef",
     "TableInputTypeDef",
+    "TableTypeDef",
     "GetSecurityConfigurationResponseTypeDef",
     "GetSecurityConfigurationsResponseTypeDef",
-    "CodeGenConfigurationNodeOutputTypeDef",
     "CodeGenConfigurationNodeTypeDef",
     "GetMLTaskRunsResponseTypeDef",
     "GetStatementResponseTypeDef",
     "ListStatementsResponseTypeDef",
-    "ColumnStatisticsTypeDef",
     "NodeTypeDef",
     "GetMLTransformsResponseTypeDef",
     "ColumnStatisticsErrorTypeDef",
     "GetColumnStatisticsForPartitionResponseTypeDef",
     "GetColumnStatisticsForTableResponseTypeDef",
+    "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
+    "UpdateColumnStatisticsForTableRequestRequestTypeDef",
+    "BatchCreatePartitionRequestRequestTypeDef",
+    "BatchUpdatePartitionRequestEntryTypeDef",
+    "CreatePartitionRequestRequestTypeDef",
+    "UpdatePartitionRequestRequestTypeDef",
     "BatchGetPartitionResponseTypeDef",
     "GetPartitionResponseTypeDef",
     "GetPartitionsResponseTypeDef",
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     "UnfilteredPartitionTypeDef",
+    "CreateTableRequestRequestTypeDef",
+    "UpdateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
     "GetTablesResponseTypeDef",
     "GetUnfilteredTableMetadataResponseTypeDef",
     "SearchTablesResponseTypeDef",
     "TableVersionTypeDef",
-    "BatchCreatePartitionRequestRequestTypeDef",
-    "BatchUpdatePartitionRequestEntryTypeDef",
-    "CreatePartitionRequestRequestTypeDef",
-    "UpdatePartitionRequestRequestTypeDef",
-    "CreateTableRequestRequestTypeDef",
-    "UpdateTableRequestRequestTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "CodeGenConfigurationNodeUnionTypeDef",
     "JobUpdateTypeDef",
-    "ColumnStatisticsUnionTypeDef",
     "WorkflowGraphTypeDef",
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     "UpdateColumnStatisticsForTableResponseTypeDef",
+    "BatchUpdatePartitionRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     "GetTableVersionResponseTypeDef",
     "GetTableVersionsResponseTypeDef",
-    "BatchUpdatePartitionRequestRequestTypeDef",
     "BatchGetJobsResponseTypeDef",
     "GetJobResponseTypeDef",
     "GetJobsResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    "UpdateColumnStatisticsForTableRequestRequestTypeDef",
     "WorkflowRunTypeDef",
     "GetWorkflowRunResponseTypeDef",
     "GetWorkflowRunsResponseTypeDef",
     "WorkflowTypeDef",
     "BatchGetWorkflowsResponseTypeDef",
     "GetWorkflowResponseTypeDef",
 )
@@ -883,26 +777,18 @@
     "NotificationPropertyTypeDef",
     {
         "NotifyDelayAfter": int,
     },
     total=False,
 )
 
-AggregateOperationOutputTypeDef = TypedDict(
-    "AggregateOperationOutputTypeDef",
-    {
-        "Column": List[str],
-        "AggFunc": AggFunctionType,
-    },
-)
-
 AggregateOperationTypeDef = TypedDict(
     "AggregateOperationTypeDef",
     {
-        "Column": Sequence[str],
+        "Column": List[str],
         "AggFunc": AggFunctionType,
     },
 )
 
 AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
     "AmazonRedshiftAdvancedOptionTypeDef",
     {
@@ -918,64 +804,45 @@
         "Value": str,
         "Label": str,
         "Description": str,
     },
     total=False,
 )
 
-ApplyMappingOutputTypeDef = TypedDict(
-    "ApplyMappingOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Mapping": List["MappingOutputTypeDef"],
-    },
-)
-
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Mapping": Sequence["MappingTypeDef"],
+        "Inputs": List[str],
+        "Mapping": List["MappingTypeDef"],
     },
 )
 
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
         "RequestedColumns": Sequence[str],
         "AllColumnsRequested": bool,
     },
     total=False,
 )
 
-PartitionValueListOutputTypeDef = TypedDict(
-    "PartitionValueListOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
-BasicCatalogTargetOutputTypeDef = TypedDict(
-    "BasicCatalogTargetOutputTypeDef",
+PartitionValueListTypeDef = TypedDict(
+    "PartitionValueListTypeDef",
     {
-        "Name": str,
-        "Inputs": List[str],
-        "Database": str,
-        "Table": str,
+        "Values": Sequence[str],
     },
 )
 
 BasicCatalogTargetTypeDef = TypedDict(
     "BasicCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -1226,15 +1093,14 @@
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlueprintDetailsTypeDef = TypedDict(
     "BlueprintDetailsTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
     total=False,
@@ -1336,16 +1202,16 @@
         "ImportCompleted": bool,
         "ImportTime": datetime,
         "ImportedBy": str,
     },
     total=False,
 )
 
-KafkaStreamingSourceOptionsOutputTypeDef = TypedDict(
-    "KafkaStreamingSourceOptionsOutputTypeDef",
+KafkaStreamingSourceOptionsTypeDef = TypedDict(
+    "KafkaStreamingSourceOptionsTypeDef",
     {
         "BootstrapServers": str,
         "SecurityProtocol": str,
         "ConnectionName": str,
         "TopicName": str,
         "Assign": str,
         "SubscribePattern": str,
@@ -1371,16 +1237,16 @@
     {
         "PollingTime": int,
         "RecordPollingLimit": int,
     },
     total=False,
 )
 
-KinesisStreamingSourceOptionsOutputTypeDef = TypedDict(
-    "KinesisStreamingSourceOptionsOutputTypeDef",
+KinesisStreamingSourceOptionsTypeDef = TypedDict(
+    "KinesisStreamingSourceOptionsTypeDef",
     {
         "EndpointUrl": str,
         "StreamName": str,
         "Classification": str,
         "Delimiter": str,
         "StartingPosition": StartingPositionType,
         "MaxFetchTimeInMs": int,
@@ -1417,43 +1283,19 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredCatalogTargetOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "Tables": List[str],
-    },
-)
-_OptionalCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalCatalogTargetOutputTypeDef",
-    {
-        "ConnectionName": str,
-        "EventQueueArn": str,
-        "DlqEventQueueArn": str,
-    },
-    total=False,
-)
-
-
-class CatalogTargetOutputTypeDef(
-    _RequiredCatalogTargetOutputTypeDef, _OptionalCatalogTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredCatalogTargetTypeDef = TypedDict(
     "_RequiredCatalogTargetTypeDef",
     {
         "DatabaseName": str,
-        "Tables": Sequence[str],
+        "Tables": List[str],
     },
 )
 _OptionalCatalogTargetTypeDef = TypedDict(
     "_OptionalCatalogTargetTypeDef",
     {
         "ConnectionName": str,
         "EventQueueArn": str,
@@ -1601,38 +1443,36 @@
 )
 
 
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
 
-_RequiredDropDuplicatesOutputTypeDef = TypedDict(
-    "_RequiredDropDuplicatesOutputTypeDef",
+_RequiredDropDuplicatesTypeDef = TypedDict(
+    "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
-_OptionalDropDuplicatesOutputTypeDef = TypedDict(
-    "_OptionalDropDuplicatesOutputTypeDef",
+_OptionalDropDuplicatesTypeDef = TypedDict(
+    "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
 
-class DropDuplicatesOutputTypeDef(
-    _RequiredDropDuplicatesOutputTypeDef, _OptionalDropDuplicatesOutputTypeDef
-):
+class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
 
-DropFieldsOutputTypeDef = TypedDict(
-    "DropFieldsOutputTypeDef",
+DropFieldsTypeDef = TypedDict(
+    "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
 )
 
@@ -1641,39 +1481,39 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredFillMissingValuesOutputTypeDef = TypedDict(
-    "_RequiredFillMissingValuesOutputTypeDef",
+_RequiredFillMissingValuesTypeDef = TypedDict(
+    "_RequiredFillMissingValuesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ImputedPath": str,
     },
 )
-_OptionalFillMissingValuesOutputTypeDef = TypedDict(
-    "_OptionalFillMissingValuesOutputTypeDef",
+_OptionalFillMissingValuesTypeDef = TypedDict(
+    "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
 
-class FillMissingValuesOutputTypeDef(
-    _RequiredFillMissingValuesOutputTypeDef, _OptionalFillMissingValuesOutputTypeDef
+class FillMissingValuesTypeDef(
+    _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
 
-MergeOutputTypeDef = TypedDict(
-    "MergeOutputTypeDef",
+MergeTypeDef = TypedDict(
+    "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
     },
 )
@@ -1683,16 +1523,16 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-MicrosoftSQLServerCatalogTargetOutputTypeDef = TypedDict(
-    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1702,16 +1542,16 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-MySQLCatalogTargetOutputTypeDef = TypedDict(
-    "MySQLCatalogTargetOutputTypeDef",
+MySQLCatalogTargetTypeDef = TypedDict(
+    "MySQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1721,62 +1561,60 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-OracleSQLCatalogTargetOutputTypeDef = TypedDict(
-    "OracleSQLCatalogTargetOutputTypeDef",
+OracleSQLCatalogTargetTypeDef = TypedDict(
+    "OracleSQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredPIIDetectionOutputTypeDef = TypedDict(
-    "_RequiredPIIDetectionOutputTypeDef",
+_RequiredPIIDetectionTypeDef = TypedDict(
+    "_RequiredPIIDetectionTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "PiiType": PiiTypeType,
         "EntityTypesToDetect": List[str],
     },
 )
-_OptionalPIIDetectionOutputTypeDef = TypedDict(
-    "_OptionalPIIDetectionOutputTypeDef",
+_OptionalPIIDetectionTypeDef = TypedDict(
+    "_OptionalPIIDetectionTypeDef",
     {
         "OutputColumnName": str,
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
 
-class PIIDetectionOutputTypeDef(
-    _RequiredPIIDetectionOutputTypeDef, _OptionalPIIDetectionOutputTypeDef
-):
+class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
 
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-PostgreSQLCatalogTargetOutputTypeDef = TypedDict(
-    "PostgreSQLCatalogTargetOutputTypeDef",
+PostgreSQLCatalogTargetTypeDef = TypedDict(
+    "PostgreSQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1808,242 +1646,47 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-RenameFieldOutputTypeDef = TypedDict(
-    "RenameFieldOutputTypeDef",
+RenameFieldTypeDef = TypedDict(
+    "RenameFieldTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SourcePath": List[str],
         "TargetPath": List[str],
     },
 )
 
-SelectFieldsOutputTypeDef = TypedDict(
-    "SelectFieldsOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
-    },
-)
-
-SelectFromCollectionOutputTypeDef = TypedDict(
-    "SelectFromCollectionOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Index": int,
-    },
-)
-
-_RequiredSpigotOutputTypeDef = TypedDict(
-    "_RequiredSpigotOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-    },
-)
-_OptionalSpigotOutputTypeDef = TypedDict(
-    "_OptionalSpigotOutputTypeDef",
-    {
-        "Topk": int,
-        "Prob": float,
-    },
-    total=False,
-)
-
-
-class SpigotOutputTypeDef(_RequiredSpigotOutputTypeDef, _OptionalSpigotOutputTypeDef):
-    pass
-
-
-SplitFieldsOutputTypeDef = TypedDict(
-    "SplitFieldsOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
-    },
-)
-
-UnionOutputTypeDef = TypedDict(
-    "UnionOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "UnionType": UnionTypeType,
-    },
-)
-
-_RequiredDropDuplicatesTypeDef = TypedDict(
-    "_RequiredDropDuplicatesTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-    },
-)
-_OptionalDropDuplicatesTypeDef = TypedDict(
-    "_OptionalDropDuplicatesTypeDef",
-    {
-        "Columns": Sequence[Sequence[str]],
-    },
-    total=False,
-)
-
-
-class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
-    pass
-
-
-DropFieldsTypeDef = TypedDict(
-    "DropFieldsTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
-    },
-)
-
-_RequiredFillMissingValuesTypeDef = TypedDict(
-    "_RequiredFillMissingValuesTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "ImputedPath": str,
-    },
-)
-_OptionalFillMissingValuesTypeDef = TypedDict(
-    "_OptionalFillMissingValuesTypeDef",
-    {
-        "FilledPath": str,
-    },
-    total=False,
-)
-
-
-class FillMissingValuesTypeDef(
-    _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
-):
-    pass
-
-
-MergeTypeDef = TypedDict(
-    "MergeTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Source": str,
-        "PrimaryKeys": Sequence[Sequence[str]],
-    },
-)
-
-MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
-    "MicrosoftSQLServerCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-MySQLCatalogTargetTypeDef = TypedDict(
-    "MySQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-OracleSQLCatalogTargetTypeDef = TypedDict(
-    "OracleSQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-_RequiredPIIDetectionTypeDef = TypedDict(
-    "_RequiredPIIDetectionTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "PiiType": PiiTypeType,
-        "EntityTypesToDetect": Sequence[str],
-    },
-)
-_OptionalPIIDetectionTypeDef = TypedDict(
-    "_OptionalPIIDetectionTypeDef",
-    {
-        "OutputColumnName": str,
-        "SampleFraction": float,
-        "ThresholdFraction": float,
-        "MaskValue": str,
-    },
-    total=False,
-)
-
-
-class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
-    pass
-
-
-PostgreSQLCatalogTargetTypeDef = TypedDict(
-    "PostgreSQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-RenameFieldTypeDef = TypedDict(
-    "RenameFieldTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "SourcePath": Sequence[str],
-        "TargetPath": Sequence[str],
-    },
-)
-
 SelectFieldsTypeDef = TypedDict(
     "SelectFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
+        "Inputs": List[str],
+        "Paths": List[List[str]],
     },
 )
 
 SelectFromCollectionTypeDef = TypedDict(
     "SelectFromCollectionTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Index": int,
     },
 )
 
 _RequiredSpigotTypeDef = TypedDict(
     "_RequiredSpigotTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
     },
 )
 _OptionalSpigotTypeDef = TypedDict(
     "_OptionalSpigotTypeDef",
     {
         "Topk": int,
@@ -2057,24 +1700,24 @@
     pass
 
 
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
+        "Inputs": List[str],
+        "Paths": List[List[str]],
     },
 )
 
 UnionTypeDef = TypedDict(
     "UnionTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "UnionType": UnionTypeType,
     },
 )
 
 _RequiredCodeGenEdgeTypeDef = TypedDict(
     "_RequiredCodeGenEdgeTypeDef",
     {
@@ -2120,63 +1763,42 @@
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
 )
 
-_RequiredColumnOutputTypeDef = TypedDict(
-    "_RequiredColumnOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalColumnOutputTypeDef = TypedDict(
-    "_OptionalColumnOutputTypeDef",
-    {
-        "Type": str,
-        "Comment": str,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ColumnOutputTypeDef(_RequiredColumnOutputTypeDef, _OptionalColumnOutputTypeDef):
-    pass
-
-
 ColumnRowFilterTypeDef = TypedDict(
     "ColumnRowFilterTypeDef",
     {
         "ColumnName": str,
         "RowFilterExpression": str,
     },
     total=False,
 )
 
-_RequiredDateColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredDateColumnStatisticsDataOutputTypeDef",
+_RequiredDateColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredDateColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
-_OptionalDateColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalDateColumnStatisticsDataOutputTypeDef",
+_OptionalDateColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalDateColumnStatisticsDataTypeDef",
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
 
-class DateColumnStatisticsDataOutputTypeDef(
-    _RequiredDateColumnStatisticsDataOutputTypeDef, _OptionalDateColumnStatisticsDataOutputTypeDef
+class DateColumnStatisticsDataTypeDef(
+    _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
 
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
@@ -2229,15 +1851,14 @@
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 _RequiredColumnTypeDef = TypedDict(
     "_RequiredColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalColumnTypeDef = TypedDict(
@@ -2305,36 +1926,18 @@
 
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
 
-PhysicalConnectionRequirementsOutputTypeDef = TypedDict(
-    "PhysicalConnectionRequirementsOutputTypeDef",
-    {
-        "SubnetId": str,
-        "SecurityGroupIdList": List[str],
-        "AvailabilityZone": str,
-    },
-    total=False,
-)
-
-ConnectionsListOutputTypeDef = TypedDict(
-    "ConnectionsListOutputTypeDef",
-    {
-        "Connections": List[str],
-    },
-    total=False,
-)
-
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
-        "Connections": Sequence[str],
+        "Connections": List[str],
     },
     total=False,
 )
 
 CrawlTypeDef = TypedDict(
     "CrawlTypeDef",
     {
@@ -2376,16 +1979,16 @@
         "TablesCreated": int,
         "TablesUpdated": int,
         "TablesDeleted": int,
     },
     total=False,
 )
 
-DeltaTargetOutputTypeDef = TypedDict(
-    "DeltaTargetOutputTypeDef",
+DeltaTargetTypeDef = TypedDict(
+    "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
         "CreateNativeDeltaTable": bool,
     },
     total=False,
@@ -2397,16 +2000,16 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
-JdbcTargetOutputTypeDef = TypedDict(
-    "JdbcTargetOutputTypeDef",
+JdbcTargetTypeDef = TypedDict(
+    "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
         "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
@@ -2418,54 +2021,19 @@
         "ConnectionName": str,
         "Path": str,
         "ScanAll": bool,
     },
     total=False,
 )
 
-S3TargetOutputTypeDef = TypedDict(
-    "S3TargetOutputTypeDef",
-    {
-        "Path": str,
-        "Exclusions": List[str],
-        "ConnectionName": str,
-        "SampleSize": int,
-        "EventQueueArn": str,
-        "DlqEventQueueArn": str,
-    },
-    total=False,
-)
-
-DeltaTargetTypeDef = TypedDict(
-    "DeltaTargetTypeDef",
-    {
-        "DeltaTables": Sequence[str],
-        "ConnectionName": str,
-        "WriteManifest": bool,
-        "CreateNativeDeltaTable": bool,
-    },
-    total=False,
-)
-
-JdbcTargetTypeDef = TypedDict(
-    "JdbcTargetTypeDef",
-    {
-        "ConnectionName": str,
-        "Path": str,
-        "Exclusions": Sequence[str],
-        "EnableAdditionalMetadata": Sequence[JdbcMetadataEntryType],
-    },
-    total=False,
-)
-
 S3TargetTypeDef = TypedDict(
     "S3TargetTypeDef",
     {
         "Path": str,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "ConnectionName": str,
         "SampleSize": int,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
@@ -2750,14 +2318,36 @@
         "LastCommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+_RequiredGlueTableTypeDef = TypedDict(
+    "_RequiredGlueTableTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGlueTableTypeDef = TypedDict(
+    "_OptionalGlueTableTypeDef",
+    {
+        "CatalogId": str,
+        "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
+    pass
+
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2898,70 +2488,27 @@
     {
         "CloudWatchMetricsEnabled": bool,
         "ResultsS3Prefix": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DataQualityRuleResultTypeDef = TypedDict(
     "DataQualityRuleResultTypeDef",
     {
         "Name": str,
         "Description": str,
         "EvaluationMessage": str,
         "Result": DataQualityRuleResultStatusType,
         "EvaluatedMetrics": Dict[str, float],
     },
     total=False,
 )
 
-_RequiredGlueTableOutputTypeDef = TypedDict(
-    "_RequiredGlueTableOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGlueTableOutputTypeDef = TypedDict(
-    "_OptionalGlueTableOutputTypeDef",
-    {
-        "CatalogId": str,
-        "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class GlueTableOutputTypeDef(_RequiredGlueTableOutputTypeDef, _OptionalGlueTableOutputTypeDef):
-    pass
-
-
-_RequiredGlueTableTypeDef = TypedDict(
-    "_RequiredGlueTableTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGlueTableTypeDef = TypedDict(
-    "_OptionalGlueTableTypeDef",
-    {
-        "CatalogId": str,
-        "ConnectionName": str,
-        "AdditionalOptions": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
-    pass
-
-
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Region": str,
     },
@@ -2981,16 +2528,16 @@
     "DatatypeTypeDef",
     {
         "Id": str,
         "Label": str,
     },
 )
 
-DecimalNumberOutputTypeDef = TypedDict(
-    "DecimalNumberOutputTypeDef",
+DecimalNumberTypeDef = TypedDict(
+    "DecimalNumberTypeDef",
     {
         "UnscaledValue": bytes,
         "Scale": int,
     },
 )
 
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
@@ -3344,53 +2891,27 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
-_RequiredTransformConfigParameterOutputTypeDef = TypedDict(
-    "_RequiredTransformConfigParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParamTypeType,
-    },
-)
-_OptionalTransformConfigParameterOutputTypeDef = TypedDict(
-    "_OptionalTransformConfigParameterOutputTypeDef",
-    {
-        "ValidationRule": str,
-        "ValidationMessage": str,
-        "Value": List[str],
-        "ListType": ParamTypeType,
-        "IsOptional": bool,
-    },
-    total=False,
-)
-
-
-class TransformConfigParameterOutputTypeDef(
-    _RequiredTransformConfigParameterOutputTypeDef, _OptionalTransformConfigParameterOutputTypeDef
-):
-    pass
-
-
 _RequiredTransformConfigParameterTypeDef = TypedDict(
     "_RequiredTransformConfigParameterTypeDef",
     {
         "Name": str,
         "Type": ParamTypeType,
     },
 )
 _OptionalTransformConfigParameterTypeDef = TypedDict(
     "_OptionalTransformConfigParameterTypeDef",
     {
         "ValidationRule": str,
         "ValidationMessage": str,
-        "Value": Sequence[str],
+        "Value": List[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
 
@@ -3450,27 +2971,19 @@
         "Identifier": str,
         "DatabaseIdentifier": str,
         "ConnectionName": str,
     },
     total=False,
 )
 
-FilterValueOutputTypeDef = TypedDict(
-    "FilterValueOutputTypeDef",
-    {
-        "Type": FilterValueTypeType,
-        "Value": List[str],
-    },
-)
-
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
-        "Value": Sequence[str],
+        "Value": List[str],
     },
 )
 
 FindMatchesParametersTypeDef = TypedDict(
     "FindMatchesParametersTypeDef",
     {
         "PrimaryKeyColumnName": str,
@@ -4317,66 +3830,43 @@
     {
         "InputS3Path": str,
         "Replace": bool,
     },
     total=False,
 )
 
-JDBCConnectorOptionsOutputTypeDef = TypedDict(
-    "JDBCConnectorOptionsOutputTypeDef",
-    {
-        "FilterPredicate": str,
-        "PartitionColumn": str,
-        "LowerBound": int,
-        "UpperBound": int,
-        "NumPartitions": int,
-        "JobBookmarkKeys": List[str],
-        "JobBookmarkKeysSortOrder": str,
-        "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
-    },
-    total=False,
-)
-
 JDBCConnectorOptionsTypeDef = TypedDict(
     "JDBCConnectorOptionsTypeDef",
     {
         "FilterPredicate": str,
         "PartitionColumn": str,
         "LowerBound": int,
         "UpperBound": int,
         "NumPartitions": int,
-        "JobBookmarkKeys": Sequence[str],
+        "JobBookmarkKeys": List[str],
         "JobBookmarkKeysSortOrder": str,
-        "DataTypeMapping": Mapping[JDBCDataTypeType, GlueRecordTypeType],
+        "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
     },
     total=False,
 )
 
 PredecessorTypeDef = TypedDict(
     "PredecessorTypeDef",
     {
         "JobName": str,
         "RunId": str,
     },
     total=False,
 )
 
-JoinColumnOutputTypeDef = TypedDict(
-    "JoinColumnOutputTypeDef",
-    {
-        "From": str,
-        "Keys": List[List[str]],
-    },
-)
-
 JoinColumnTypeDef = TypedDict(
     "JoinColumnTypeDef",
     {
         "From": str,
-        "Keys": Sequence[Sequence[str]],
+        "Keys": List[List[str]],
     },
 )
 
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "Name": str,
@@ -4560,36 +4050,23 @@
 
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
 
-MappingOutputTypeDef = TypedDict(
-    "MappingOutputTypeDef",
-    {
-        "ToKey": str,
-        "FromPath": List[str],
-        "FromType": str,
-        "ToType": str,
-        "Dropped": bool,
-        "Children": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
-        "FromPath": Sequence[str],
+        "FromPath": List[str],
         "FromType": str,
         "ToType": str,
         "Dropped": bool,
-        "Children": Sequence[Dict[str, Any]],
+        "Children": List[Dict[str, Any]],
     },
     total=False,
 )
 
 OtherMetadataValueListItemTypeDef = TypedDict(
     "OtherMetadataValueListItemTypeDef",
     {
@@ -4612,21 +4089,14 @@
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
     },
 )
 
-PartitionValueListTypeDef = TypedDict(
-    "PartitionValueListTypeDef",
-    {
-        "Values": Sequence[str],
-    },
-)
-
 PropertyPredicateTypeDef = TypedDict(
     "PropertyPredicateTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparator": ComparatorType,
     },
@@ -4662,30 +4132,20 @@
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
-UpsertRedshiftTargetOptionsOutputTypeDef = TypedDict(
-    "UpsertRedshiftTargetOptionsOutputTypeDef",
-    {
-        "TableLocation": str,
-        "ConnectionName": str,
-        "UpsertKeys": List[str],
-    },
-    total=False,
-)
-
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
-        "UpsertKeys": Sequence[str],
+        "UpsertKeys": List[str],
     },
     total=False,
 )
 
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
@@ -4763,44 +4223,24 @@
     {
         "FieldName": str,
         "Sort": SortType,
     },
     total=False,
 )
 
-SerDeInfoOutputTypeDef = TypedDict(
-    "SerDeInfoOutputTypeDef",
-    {
-        "Name": str,
-        "SerializationLibrary": str,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
 SerDeInfoTypeDef = TypedDict(
     "SerDeInfoTypeDef",
     {
         "Name": str,
         "SerializationLibrary": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-SkewedInfoOutputTypeDef = TypedDict(
-    "SkewedInfoOutputTypeDef",
-    {
-        "SkewedColumnNames": List[str],
-        "SkewedColumnValues": List[str],
-        "SkewedColumnValueLocationMaps": Dict[str, str],
-    },
-    total=False,
-)
-
 SkewedInfoTypeDef = TypedDict(
     "SkewedInfoTypeDef",
     {
         "SkewedColumnNames": Sequence[str],
         "SkewedColumnValues": Sequence[str],
         "SkewedColumnValueLocationMaps": Mapping[str, str],
     },
@@ -5246,32 +4686,19 @@
         "RunningActions": int,
         "ErroredActions": int,
         "WaitingActions": int,
     },
     total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "JobName": str,
-        "Arguments": Dict[str, str],
-        "Timeout": int,
-        "SecurityConfiguration": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "CrawlerName": str,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "JobName": str,
-        "Arguments": Mapping[str, str],
+        "Arguments": Dict[str, str],
         "Timeout": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "CrawlerName": str,
     },
     total=False,
 )
@@ -5302,36 +4729,26 @@
 
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
 
-AggregateOutputTypeDef = TypedDict(
-    "AggregateOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Groups": List[List[str]],
-        "Aggs": List[AggregateOperationOutputTypeDef],
-    },
-)
-
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Groups": Sequence[Sequence[str]],
-        "Aggs": Sequence[AggregateOperationTypeDef],
+        "Inputs": List[str],
+        "Groups": List[List[str]],
+        "Aggs": List[AggregateOperationTypeDef],
     },
 )
 
-AmazonRedshiftNodeDataOutputTypeDef = TypedDict(
-    "AmazonRedshiftNodeDataOutputTypeDef",
+AmazonRedshiftNodeDataTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataTypeDef",
     {
         "AccessType": str,
         "SourceType": str,
         "Connection": OptionTypeDef,
         "Schema": OptionTypeDef,
         "Table": OptionTypeDef,
         "CatalogDatabase": OptionTypeDef,
@@ -5355,47 +4772,14 @@
         "TableSchema": List[OptionTypeDef],
         "StagingTable": str,
         "SelectedColumns": List[OptionTypeDef],
     },
     total=False,
 )
 
-AmazonRedshiftNodeDataTypeDef = TypedDict(
-    "AmazonRedshiftNodeDataTypeDef",
-    {
-        "AccessType": str,
-        "SourceType": str,
-        "Connection": OptionTypeDef,
-        "Schema": OptionTypeDef,
-        "Table": OptionTypeDef,
-        "CatalogDatabase": OptionTypeDef,
-        "CatalogTable": OptionTypeDef,
-        "CatalogRedshiftSchema": str,
-        "CatalogRedshiftTable": str,
-        "TempDir": str,
-        "IamRole": OptionTypeDef,
-        "AdvancedOptions": Sequence[AmazonRedshiftAdvancedOptionTypeDef],
-        "SampleQuery": str,
-        "PreAction": str,
-        "PostAction": str,
-        "Action": str,
-        "TablePrefix": str,
-        "Upsert": bool,
-        "MergeAction": str,
-        "MergeWhenMatched": str,
-        "MergeWhenNotMatched": str,
-        "MergeClause": str,
-        "CrawlerConnection": str,
-        "TableSchema": Sequence[OptionTypeDef],
-        "StagingTable": str,
-        "SelectedColumns": Sequence[OptionTypeDef],
-    },
-    total=False,
-)
-
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -5443,19 +4827,66 @@
     pass
 
 
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
-        "Partitions": List[PartitionValueListOutputTypeDef],
+        "Partitions": List[PartitionValueListTypeDef],
+    },
+    total=False,
+)
+
+_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
     },
     total=False,
 )
 
+
+class BatchDeletePartitionRequestRequestTypeDef(
+    _RequiredBatchDeletePartitionRequestRequestTypeDef,
+    _OptionalBatchDeletePartitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetPartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetPartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class BatchGetPartitionRequestRequestTypeDef(
+    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
+):
+    pass
+
+
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6198,22 +5629,14 @@
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DecimalNumberTypeDef = TypedDict(
-    "DecimalNumberTypeDef",
-    {
-        "UnscaledValue": BlobTypeDef,
-        "Scale": int,
-    },
-)
-
 GetBlueprintRunResponseTypeDef = TypedDict(
     "GetBlueprintRunResponseTypeDef",
     {
         "BlueprintRun": BlueprintRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6248,304 +5671,202 @@
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCatalogKafkaSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogKafkaSourceOutputTypeDef",
+_RequiredCatalogKafkaSourceTypeDef = TypedDict(
+    "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
 )
-_OptionalCatalogKafkaSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogKafkaSourceOutputTypeDef",
+_OptionalCatalogKafkaSourceTypeDef = TypedDict(
+    "_OptionalCatalogKafkaSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
 
-class CatalogKafkaSourceOutputTypeDef(
-    _RequiredCatalogKafkaSourceOutputTypeDef, _OptionalCatalogKafkaSourceOutputTypeDef
+class CatalogKafkaSourceTypeDef(
+    _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
 
-_RequiredDirectKafkaSourceOutputTypeDef = TypedDict(
-    "_RequiredDirectKafkaSourceOutputTypeDef",
+_RequiredDirectKafkaSourceTypeDef = TypedDict(
+    "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalDirectKafkaSourceOutputTypeDef = TypedDict(
-    "_OptionalDirectKafkaSourceOutputTypeDef",
+_OptionalDirectKafkaSourceTypeDef = TypedDict(
+    "_OptionalDirectKafkaSourceTypeDef",
     {
-        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
 
-class DirectKafkaSourceOutputTypeDef(
-    _RequiredDirectKafkaSourceOutputTypeDef, _OptionalDirectKafkaSourceOutputTypeDef
+class DirectKafkaSourceTypeDef(
+    _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
 
-_RequiredCatalogKinesisSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogKinesisSourceOutputTypeDef",
+_RequiredCatalogKinesisSourceTypeDef = TypedDict(
+    "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
 )
-_OptionalCatalogKinesisSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogKinesisSourceOutputTypeDef",
+_OptionalCatalogKinesisSourceTypeDef = TypedDict(
+    "_OptionalCatalogKinesisSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
 
-class CatalogKinesisSourceOutputTypeDef(
-    _RequiredCatalogKinesisSourceOutputTypeDef, _OptionalCatalogKinesisSourceOutputTypeDef
+class CatalogKinesisSourceTypeDef(
+    _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
 
-_RequiredDirectKinesisSourceOutputTypeDef = TypedDict(
-    "_RequiredDirectKinesisSourceOutputTypeDef",
+_RequiredDirectKinesisSourceTypeDef = TypedDict(
+    "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalDirectKinesisSourceOutputTypeDef = TypedDict(
-    "_OptionalDirectKinesisSourceOutputTypeDef",
+_OptionalDirectKinesisSourceTypeDef = TypedDict(
+    "_OptionalDirectKinesisSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
 
-class DirectKinesisSourceOutputTypeDef(
-    _RequiredDirectKinesisSourceOutputTypeDef, _OptionalDirectKinesisSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredGovernedCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredGovernedCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalGovernedCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalGovernedCatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class GovernedCatalogTargetOutputTypeDef(
-    _RequiredGovernedCatalogTargetOutputTypeDef, _OptionalGovernedCatalogTargetOutputTypeDef
+class DirectKinesisSourceTypeDef(
+    _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
 
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalGovernedCatalogTargetTypeDef = TypedDict(
     "_OptionalGovernedCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
 
-_RequiredS3CatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3CatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3CatalogTargetOutputTypeDef(
-    _RequiredS3CatalogTargetOutputTypeDef, _OptionalS3CatalogTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3CatalogTargetTypeDef = TypedDict(
     "_OptionalS3CatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
-    pass
-
-
-_RequiredS3DeltaCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3DeltaCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaCatalogTargetOutputTypeDef",
-    {
         "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
-class S3DeltaCatalogTargetOutputTypeDef(
-    _RequiredS3DeltaCatalogTargetOutputTypeDef, _OptionalS3DeltaCatalogTargetOutputTypeDef
-):
+class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
 
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
     "_OptionalS3DeltaCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "AdditionalOptions": Mapping[str, str],
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
 
-_RequiredS3HudiCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3HudiCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3HudiCatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3HudiCatalogTargetOutputTypeDef(
-    _RequiredS3HudiCatalogTargetOutputTypeDef, _OptionalS3HudiCatalogTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
-        "AdditionalOptions": Mapping[str, str],
+        "AdditionalOptions": Dict[str, str],
     },
 )
 _OptionalS3HudiCatalogTargetTypeDef = TypedDict(
     "_OptionalS3HudiCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3HudiCatalogTargetTypeDef(
@@ -6561,37 +5882,14 @@
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
     },
     total=False,
 )
 
-_RequiredCodeGenNodeOutputTypeDef = TypedDict(
-    "_RequiredCodeGenNodeOutputTypeDef",
-    {
-        "Id": str,
-        "NodeType": str,
-        "Args": List[CodeGenNodeArgTypeDef],
-    },
-)
-_OptionalCodeGenNodeOutputTypeDef = TypedDict(
-    "_OptionalCodeGenNodeOutputTypeDef",
-    {
-        "LineNumber": int,
-    },
-    total=False,
-)
-
-
-class CodeGenNodeOutputTypeDef(
-    _RequiredCodeGenNodeOutputTypeDef, _OptionalCodeGenNodeOutputTypeDef
-):
-    pass
-
-
 _RequiredCodeGenNodeTypeDef = TypedDict(
     "_RequiredCodeGenNodeTypeDef",
     {
         "Id": str,
         "NodeType": str,
         "Args": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -6615,166 +5913,19 @@
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
     total=False,
 )
 
-_RequiredDateColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredDateColumnStatisticsDataTypeDef",
-    {
-        "NumberOfNulls": int,
-        "NumberOfDistinctValues": int,
-    },
-)
-_OptionalDateColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalDateColumnStatisticsDataTypeDef",
-    {
-        "MinimumValue": TimestampTypeDef,
-        "MaximumValue": TimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class DateColumnStatisticsDataTypeDef(
-    _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
-):
-    pass
-
-
-_RequiredGetTableRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "Name": str,
-    },
-)
-_OptionalGetTableRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTableRequestRequestTypeDef(
-    _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredGetTablesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTablesRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalGetTablesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTablesRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "Expression": str,
-        "NextToken": str,
-        "MaxResults": int,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTablesRequestRequestTypeDef(
-    _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
-):
-    pass
-
-
-KafkaStreamingSourceOptionsTypeDef = TypedDict(
-    "KafkaStreamingSourceOptionsTypeDef",
-    {
-        "BootstrapServers": str,
-        "SecurityProtocol": str,
-        "ConnectionName": str,
-        "TopicName": str,
-        "Assign": str,
-        "SubscribePattern": str,
-        "Classification": str,
-        "Delimiter": str,
-        "StartingOffsets": str,
-        "EndingOffsets": str,
-        "PollTimeoutMs": int,
-        "NumRetries": int,
-        "RetryIntervalMs": int,
-        "MaxOffsetsPerTrigger": int,
-        "MinPartitions": int,
-        "IncludeHeaders": bool,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": TimestampTypeDef,
-    },
-    total=False,
-)
-
-KinesisStreamingSourceOptionsTypeDef = TypedDict(
-    "KinesisStreamingSourceOptionsTypeDef",
-    {
-        "EndpointUrl": str,
-        "StreamName": str,
-        "Classification": str,
-        "Delimiter": str,
-        "StartingPosition": StartingPositionType,
-        "MaxFetchTimeInMs": int,
-        "MaxFetchRecordsPerShard": int,
-        "MaxRecordPerRead": int,
-        "AddIdleTimeBetweenReads": bool,
-        "IdleTimeBetweenReadsInMs": int,
-        "DescribeShardInterval": int,
-        "NumRetries": int,
-        "RetryIntervalMs": int,
-        "MaxRetryIntervalMs": int,
-        "AvoidEmptyBatches": bool,
-        "StreamArn": str,
-        "RoleArn": str,
-        "RoleSessionName": str,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": TimestampTypeDef,
-    },
-    total=False,
-)
-
-TaskRunFilterCriteriaTypeDef = TypedDict(
-    "TaskRunFilterCriteriaTypeDef",
-    {
-        "TaskRunType": TaskTypeType,
-        "Status": TaskStatusTypeType,
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
-    },
-    total=False,
-)
-
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "Logical": LogicalType,
-        "Conditions": List[ConditionTypeDef],
-    },
-    total=False,
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Logical": LogicalType,
-        "Conditions": Sequence[ConditionTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
     total=False,
 )
 
 FindMatchesMetricsTypeDef = TypedDict(
     "FindMatchesMetricsTypeDef",
     {
@@ -6815,23 +5966,22 @@
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
         "ConnectionProperties": Dict[ConnectionPropertyKeyType, str],
-        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsOutputTypeDef,
+        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
-ConnectionsListUnionTypeDef = Union[ConnectionsListTypeDef, ConnectionsListOutputTypeDef]
 CrawlerNodeDetailsTypeDef = TypedDict(
     "CrawlerNodeDetailsTypeDef",
     {
         "Crawls": List[CrawlTypeDef],
     },
     total=False,
 )
@@ -6850,36 +6000,23 @@
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CrawlerTargetsOutputTypeDef = TypedDict(
-    "CrawlerTargetsOutputTypeDef",
-    {
-        "S3Targets": List[S3TargetOutputTypeDef],
-        "JdbcTargets": List[JdbcTargetOutputTypeDef],
-        "MongoDBTargets": List[MongoDBTargetTypeDef],
-        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
-        "CatalogTargets": List[CatalogTargetOutputTypeDef],
-        "DeltaTargets": List[DeltaTargetOutputTypeDef],
-    },
-    total=False,
-)
-
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
-        "S3Targets": Sequence[S3TargetTypeDef],
-        "JdbcTargets": Sequence[JdbcTargetTypeDef],
-        "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
-        "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
-        "CatalogTargets": Sequence[CatalogTargetTypeDef],
-        "DeltaTargets": Sequence[DeltaTargetTypeDef],
+        "S3Targets": List[S3TargetTypeDef],
+        "JdbcTargets": List[JdbcTargetTypeDef],
+        "MongoDBTargets": List[MongoDBTargetTypeDef],
+        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
+        "CatalogTargets": List[CatalogTargetTypeDef],
+        "DeltaTargets": List[DeltaTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -6936,28 +6073,14 @@
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
 
-DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedBefore": TimestampTypeDef,
-        "CreatedAfter": TimestampTypeDef,
-        "LastModifiedBefore": TimestampTypeDef,
-        "LastModifiedAfter": TimestampTypeDef,
-        "TargetTable": DataQualityTargetTableTypeDef,
-    },
-    total=False,
-)
-
 DataQualityRulesetListDetailsTypeDef = TypedDict(
     "DataQualityRulesetListDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
@@ -6978,14 +6101,21 @@
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "RecommendationRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "GlueTable": GlueTableTypeDef,
+    },
+)
+
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -7105,106 +6235,54 @@
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
         "Description": str,
         "Role": str,
         "Command": SessionCommandTypeDef,
         "DefaultArguments": Dict[str, str],
-        "Connections": ConnectionsListOutputTypeDef,
+        "Connections": ConnectionsListTypeDef,
         "Progress": float,
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
-_RequiredEvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityMultiFrameOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityMultiFrameOutputTypeDef",
-    {
-        "AdditionalDataSources": Dict[str, str],
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class EvaluateDataQualityMultiFrameOutputTypeDef(
-    _RequiredEvaluateDataQualityMultiFrameOutputTypeDef,
-    _OptionalEvaluateDataQualityMultiFrameOutputTypeDef,
-):
-    pass
-
-
 _RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityMultiFrameTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityMultiFrameTypeDef",
     {
-        "AdditionalDataSources": Mapping[str, str],
+        "AdditionalDataSources": Dict[str, str],
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Mapping[Literal["performanceTuning.caching"], str],
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
 
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
 
-_RequiredEvaluateDataQualityOutputTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityOutputTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityOutputTypeDef",
-    {
-        "Output": DQTransformOutputType,
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class EvaluateDataQualityOutputTypeDef(
-    _RequiredEvaluateDataQualityOutputTypeDef, _OptionalEvaluateDataQualityOutputTypeDef
-):
-    pass
-
-
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityTypeDef",
     {
         "Output": DQTransformOutputType,
@@ -7226,75 +6304,125 @@
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
 )
 
-PrincipalPermissionsOutputTypeDef = TypedDict(
-    "PrincipalPermissionsOutputTypeDef",
+PrincipalPermissionsTypeDef = TypedDict(
+    "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
-PrincipalPermissionsTypeDef = TypedDict(
-    "PrincipalPermissionsTypeDef",
+DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
+    "DataQualityRulesetFilterCriteriaTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": Sequence[PermissionType],
+        "Name": str,
+        "Description": str,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+        "LastModifiedBefore": TimestampTypeDef,
+        "LastModifiedAfter": TimestampTypeDef,
+        "TargetTable": DataQualityTargetTableTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+_RequiredGetTableRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableRequestRequestTypeDef",
     {
-        "GlueTable": GlueTableOutputTypeDef,
+        "DatabaseName": str,
+        "Name": str,
     },
 )
+_OptionalGetTableRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+    },
+    total=False,
+)
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
+
+class GetTableRequestRequestTypeDef(
+    _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetTablesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTablesRequestRequestTypeDef",
     {
-        "GlueTable": GlueTableTypeDef,
+        "DatabaseName": str,
+    },
+)
+_OptionalGetTablesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTablesRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "Expression": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTablesRequestRequestTypeDef(
+    _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
+):
+    pass
+
+
+TaskRunFilterCriteriaTypeDef = TypedDict(
+    "TaskRunFilterCriteriaTypeDef",
+    {
+        "TaskRunType": TaskTypeType,
+        "Status": TaskStatusTypeType,
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-GlueTableUnionTypeDef = Union[GlueTableTypeDef, GlueTableOutputTypeDef]
 NullValueFieldTypeDef = TypedDict(
     "NullValueFieldTypeDef",
     {
         "Value": str,
         "Datatype": DatatypeTypeDef,
     },
 )
 
-_RequiredDecimalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredDecimalColumnStatisticsDataOutputTypeDef",
+_RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredDecimalColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
-_OptionalDecimalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalDecimalColumnStatisticsDataOutputTypeDef",
+_OptionalDecimalColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalDecimalColumnStatisticsDataTypeDef",
     {
-        "MinimumValue": DecimalNumberOutputTypeDef,
-        "MaximumValue": DecimalNumberOutputTypeDef,
+        "MinimumValue": DecimalNumberTypeDef,
+        "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
 
-class DecimalColumnStatisticsDataOutputTypeDef(
-    _RequiredDecimalColumnStatisticsDataOutputTypeDef,
-    _OptionalDecimalColumnStatisticsDataOutputTypeDef,
+class DecimalColumnStatisticsDataTypeDef(
+    _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
 
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
@@ -7388,232 +6516,117 @@
 
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredS3DeltaDirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaDirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": DeltaTargetCompressionTypeType,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DeltaDirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaDirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DeltaDirectTargetOutputTypeDef(
-    _RequiredS3DeltaDirectTargetOutputTypeDef, _OptionalS3DeltaDirectTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DeltaDirectTargetTypeDef = TypedDict(
     "_OptionalS3DeltaDirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "AdditionalOptions": Mapping[str, str],
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
 
-_RequiredS3DirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "Compression": str,
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DirectTargetOutputTypeDef(
-    _RequiredS3DirectTargetOutputTypeDef, _OptionalS3DirectTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DirectTargetTypeDef = TypedDict(
     "_OptionalS3DirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
 
-_RequiredS3GlueParquetTargetOutputTypeDef = TypedDict(
-    "_RequiredS3GlueParquetTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-    },
-)
-_OptionalS3GlueParquetTargetOutputTypeDef = TypedDict(
-    "_OptionalS3GlueParquetTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "Compression": ParquetCompressionTypeType,
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3GlueParquetTargetOutputTypeDef(
-    _RequiredS3GlueParquetTargetOutputTypeDef, _OptionalS3GlueParquetTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
     },
 )
 _OptionalS3GlueParquetTargetTypeDef = TypedDict(
     "_OptionalS3GlueParquetTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
 
-_RequiredS3HudiDirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3HudiDirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": HudiTargetCompressionTypeType,
-        "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiDirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3HudiDirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3HudiDirectTargetOutputTypeDef(
-    _RequiredS3HudiDirectTargetOutputTypeDef, _OptionalS3HudiDirectTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
         "Format": TargetFormatType,
-        "AdditionalOptions": Mapping[str, str],
+        "AdditionalOptions": Dict[str, str],
     },
 )
 _OptionalS3HudiDirectTargetTypeDef = TypedDict(
     "_OptionalS3HudiDirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "S3Encryption": List[S3EncryptionTypeDef],
-        "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
-        "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -7625,41 +6638,19 @@
     {
         "VersionNumber": int,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredFilterExpressionOutputTypeDef = TypedDict(
-    "_RequiredFilterExpressionOutputTypeDef",
-    {
-        "Operation": FilterOperationType,
-        "Values": List[FilterValueOutputTypeDef],
-    },
-)
-_OptionalFilterExpressionOutputTypeDef = TypedDict(
-    "_OptionalFilterExpressionOutputTypeDef",
-    {
-        "Negated": bool,
-    },
-    total=False,
-)
-
-
-class FilterExpressionOutputTypeDef(
-    _RequiredFilterExpressionOutputTypeDef, _OptionalFilterExpressionOutputTypeDef
-):
-    pass
-
-
 _RequiredFilterExpressionTypeDef = TypedDict(
     "_RequiredFilterExpressionTypeDef",
     {
         "Operation": FilterOperationType,
-        "Values": Sequence[FilterValueTypeDef],
+        "Values": List[FilterValueTypeDef],
     },
 )
 _OptionalFilterExpressionTypeDef = TypedDict(
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
@@ -8125,26 +7116,18 @@
 
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
 
-GlueSchemaOutputTypeDef = TypedDict(
-    "GlueSchemaOutputTypeDef",
-    {
-        "Columns": List[GlueStudioSchemaColumnTypeDef],
-    },
-    total=False,
-)
-
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
-        "Columns": Sequence[GlueStudioSchemaColumnTypeDef],
+        "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
 
 _RequiredGovernedCatalogSourceTypeDef = TypedDict(
     "_RequiredGovernedCatalogSourceTypeDef",
     {
@@ -8218,31 +7201,21 @@
         "GlueVersion": str,
         "DPUSeconds": float,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
-JoinOutputTypeDef = TypedDict(
-    "JoinOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "JoinType": JoinTypeType,
-        "Columns": List[JoinColumnOutputTypeDef],
-    },
-)
-
 JoinTypeDef = TypedDict(
     "JoinTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "JoinType": JoinTypeType,
-        "Columns": Sequence[JoinColumnTypeDef],
+        "Columns": List[JoinColumnTypeDef],
     },
 )
 
 TaskRunPropertiesTypeDef = TypedDict(
     "TaskRunPropertiesTypeDef",
     {
         "TaskType": TaskTypeType,
@@ -8357,46 +7330,19 @@
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
 
-PartitionValueListUnionTypeDef = Union[PartitionValueListTypeDef, PartitionValueListOutputTypeDef]
-_RequiredRedshiftTargetOutputTypeDef = TypedDict(
-    "_RequiredRedshiftTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalRedshiftTargetOutputTypeDef = TypedDict(
-    "_OptionalRedshiftTargetOutputTypeDef",
-    {
-        "RedshiftTmpDir": str,
-        "TmpDirIAMRole": str,
-        "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RedshiftTargetOutputTypeDef(
-    _RequiredRedshiftTargetOutputTypeDef, _OptionalRedshiftTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 _OptionalRedshiftTargetTypeDef = TypedDict(
     "_OptionalRedshiftTargetTypeDef",
     {
@@ -8473,49 +7419,29 @@
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
-AmazonRedshiftSourceOutputTypeDef = TypedDict(
-    "AmazonRedshiftSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Data": AmazonRedshiftNodeDataOutputTypeDef,
-    },
-    total=False,
-)
-
-AmazonRedshiftTargetOutputTypeDef = TypedDict(
-    "AmazonRedshiftTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Data": AmazonRedshiftNodeDataOutputTypeDef,
-        "Inputs": List[str],
-    },
-    total=False,
-)
-
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
     },
     total=False,
 )
 
 AmazonRedshiftTargetTypeDef = TypedDict(
     "AmazonRedshiftTargetTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
     },
     total=False,
 )
 
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
@@ -8584,37 +7510,14 @@
     "BatchDeleteTableVersionResponseTypeDef",
     {
         "Errors": List[TableVersionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredDecimalColumnStatisticsDataTypeDef",
-    {
-        "NumberOfNulls": int,
-        "NumberOfDistinctValues": int,
-    },
-)
-_OptionalDecimalColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalDecimalColumnStatisticsDataTypeDef",
-    {
-        "MinimumValue": DecimalNumberTypeDef,
-        "MaximumValue": DecimalNumberTypeDef,
-    },
-    total=False,
-)
-
-
-class DecimalColumnStatisticsDataTypeDef(
-    _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
-):
-    pass
-
-
 BatchGetBlueprintsResponseTypeDef = TypedDict(
     "BatchGetBlueprintsResponseTypeDef",
     {
         "Blueprints": List[BlueprintTypeDef],
         "MissingBlueprints": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8641,24 +7544,33 @@
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateScriptRequestRequestTypeDef = TypedDict(
+    "CreateScriptRequestRequestTypeDef",
+    {
+        "DagNodes": Sequence[CodeGenNodeTypeDef],
+        "DagEdges": Sequence[CodeGenEdgeTypeDef],
+        "Language": LanguageType,
+    },
+    total=False,
+)
+
 GetDataflowGraphResponseTypeDef = TypedDict(
     "GetDataflowGraphResponseTypeDef",
     {
-        "DagNodes": List[CodeGenNodeOutputTypeDef],
+        "DagNodes": List[CodeGenNodeTypeDef],
         "DagEdges": List[CodeGenEdgeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CodeGenNodeUnionTypeDef = Union[CodeGenNodeTypeDef, CodeGenNodeOutputTypeDef]
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
     },
 )
 _OptionalGetMappingRequestRequestTypeDef = TypedDict(
@@ -8698,156 +7610,60 @@
 
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCatalogKafkaSourceTypeDef = TypedDict(
-    "_RequiredCatalogKafkaSourceTypeDef",
-    {
-        "Name": str,
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalCatalogKafkaSourceTypeDef = TypedDict(
-    "_OptionalCatalogKafkaSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class CatalogKafkaSourceTypeDef(
-    _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
-):
-    pass
-
-
-_RequiredDirectKafkaSourceTypeDef = TypedDict(
-    "_RequiredDirectKafkaSourceTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDirectKafkaSourceTypeDef = TypedDict(
-    "_OptionalDirectKafkaSourceTypeDef",
-    {
-        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class DirectKafkaSourceTypeDef(
-    _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
-):
-    pass
-
-
-_RequiredCatalogKinesisSourceTypeDef = TypedDict(
-    "_RequiredCatalogKinesisSourceTypeDef",
-    {
-        "Name": str,
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalCatalogKinesisSourceTypeDef = TypedDict(
-    "_OptionalCatalogKinesisSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class CatalogKinesisSourceTypeDef(
-    _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
-):
-    pass
-
-
-_RequiredDirectKinesisSourceTypeDef = TypedDict(
-    "_RequiredDirectKinesisSourceTypeDef",
+_RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
+        "Type": TriggerTypeType,
+        "Actions": Sequence[ActionTypeDef],
     },
 )
-_OptionalDirectKinesisSourceTypeDef = TypedDict(
-    "_OptionalDirectKinesisSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class DirectKinesisSourceTypeDef(
-    _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
-):
-    pass
-
-
-_RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetMLTaskRunsRequestRequestTypeDef",
-    {
-        "TransformId": str,
-    },
-)
-_OptionalGetMLTaskRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetMLTaskRunsRequestRequestTypeDef",
+_OptionalCreateTriggerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTriggerRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TaskRunFilterCriteriaTypeDef,
-        "Sort": TaskRunSortCriteriaTypeDef,
+        "WorkflowName": str,
+        "Schedule": str,
+        "Predicate": PredicateTypeDef,
+        "Description": str,
+        "StartOnCreation": bool,
+        "Tags": Mapping[str, str],
+        "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
 
-class GetMLTaskRunsRequestRequestTypeDef(
-    _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
+class CreateTriggerRequestRequestTypeDef(
+    _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
 
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
         "State": TriggerStateType,
         "Description": str,
         "Schedule": str,
-        "Actions": List[ActionOutputTypeDef],
-        "Predicate": PredicateOutputTypeDef,
+        "Actions": List[ActionTypeDef],
+        "Predicate": PredicateTypeDef,
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-PredicateUnionTypeDef = Union[PredicateTypeDef, PredicateOutputTypeDef]
 TriggerUpdateTypeDef = TypedDict(
     "TriggerUpdateTypeDef",
     {
         "Name": str,
         "Description": str,
         "Schedule": str,
         "Actions": Sequence[ActionTypeDef],
@@ -8940,15 +7756,15 @@
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
         "Role": str,
-        "Targets": CrawlerTargetsOutputTypeDef,
+        "Targets": CrawlerTargetsTypeDef,
         "DatabaseName": str,
         "Description": str,
         "Classifiers": List[str],
         "RecrawlPolicy": RecrawlPolicyTypeDef,
         "SchemaChangePolicy": SchemaChangePolicyTypeDef,
         "LineageConfiguration": LineageConfigurationTypeDef,
         "State": CrawlerStateType,
@@ -8962,15 +7778,14 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
     },
     total=False,
 )
 
-CrawlerTargetsUnionTypeDef = Union[CrawlerTargetsTypeDef, CrawlerTargetsOutputTypeDef]
 _RequiredCreateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
         "Targets": CrawlerTargetsTypeDef,
     },
@@ -9030,158 +7845,53 @@
 
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
 
-ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 ListDataQualityRulesetsResponseTypeDef = TypedDict(
     "ListDataQualityRulesetsResponseTypeDef",
     {
         "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSessionsResponseTypeDef = TypedDict(
-    "ListSessionsResponseTypeDef",
-    {
-        "Ids": List[str],
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
-    "GetDataCatalogEncryptionSettingsResponseTypeDef",
-    {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-    },
-)
-_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
-    _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredDatabaseTypeDef = TypedDict(
-    "_RequiredDatabaseTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseTypeDef = TypedDict(
-    "_OptionalDatabaseTypeDef",
-    {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Dict[str, str],
-        "CreateTime": datetime,
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "CatalogId": str,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
-    },
-    total=False,
-)
-
-
-class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
-    pass
-
-
-_RequiredDatabaseInputTypeDef = TypedDict(
-    "_RequiredDatabaseInputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseInputTypeDef = TypedDict(
-    "_OptionalDatabaseInputTypeDef",
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
     {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Mapping[str, str],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
+        "ResultId": str,
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
     },
     total=False,
 )
 
-
-class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
-    pass
-
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
+DataQualityResultFilterCriteriaTypeDef = TypedDict(
+    "DataQualityResultFilterCriteriaTypeDef",
     {
-        "ResultId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "JobName": str,
         "JobRunId": str,
-        "StartedOn": datetime,
+        "StartedAfter": TimestampTypeDef,
+        "StartedBefore": TimestampTypeDef,
     },
     total=False,
 )
 
 DataQualityResultTypeDef = TypedDict(
     "DataQualityResultTypeDef",
     {
         "ResultId": str,
         "Score": float,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "RulesetName": str,
         "EvaluationContext": str,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "JobName": str,
         "JobRunId": str,
         "RulesetEvaluationRunId": str,
@@ -9192,36 +7902,82 @@
 
 DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
     "DataQualityRuleRecommendationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
+class DataQualityRuleRecommendationRunFilterTypeDef(
+    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
+    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+):
+    pass
+
+
 DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
+class DataQualityRulesetEvaluationRunFilterTypeDef(
+    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
+    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+):
+    pass
+
+
 GetDataQualityResultResponseTypeDef = TypedDict(
     "GetDataQualityResultResponseTypeDef",
     {
         "ResultId": str,
         "Score": float,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "RulesetName": str,
         "EvaluationContext": str,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "JobName": str,
         "JobRunId": str,
         "RulesetEvaluationRunId": str,
@@ -9230,15 +7986,15 @@
     },
 )
 
 GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
     "GetDataQualityRuleRecommendationRunResponseTypeDef",
     {
         "RunId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Role": str,
         "NumberOfWorkers": int,
         "Timeout": int,
         "Status": TaskStatusTypeType,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
@@ -9250,209 +8006,275 @@
     },
 )
 
 GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
     "GetDataQualityRulesetEvaluationRunResponseTypeDef",
     {
         "RunId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Role": str,
         "NumberOfWorkers": int,
         "Timeout": int,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "Status": TaskStatusTypeType,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
         "RulesetNames": List[str],
         "ResultIds": List[str],
-        "AdditionalDataSources": Dict[str, DataSourceOutputTypeDef],
+        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataQualityResultFilterCriteriaTypeDef = TypedDict(
-    "DataQualityResultFilterCriteriaTypeDef",
+_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedAfter": TimestampTypeDef,
-        "StartedBefore": TimestampTypeDef,
+        "Role": str,
+    },
+)
+_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "CreatedRulesetName": str,
+        "ClientToken": str,
     },
     total=False,
 )
 
-_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+
+class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "RulesetNames": Sequence[str],
     },
 )
-_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "ClientToken": str,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
 
-class DataQualityRuleRecommendationRunFilterTypeDef(
-    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
-    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
     {
-        "DataSource": DataSourceTypeDef,
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
     {
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "Ids": List[str],
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
+    "GetDataCatalogEncryptionSettingsResponseTypeDef",
+    {
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    {
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+    },
+)
+_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
     },
     total=False,
 )
 
 
-class DataQualityRulesetEvaluationRunFilterTypeDef(
-    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
-    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
+    _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
+    _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
 
-DataSourceUnionTypeDef = Union[DataSourceTypeDef, DataSourceOutputTypeDef]
-_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+_RequiredDatabaseInputTypeDef = TypedDict(
+    "_RequiredDatabaseInputTypeDef",
     {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
+        "Name": str,
     },
 )
-_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+_OptionalDatabaseInputTypeDef = TypedDict(
+    "_OptionalDatabaseInputTypeDef",
     {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "CreatedRulesetName": str,
-        "ClientToken": str,
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Mapping[str, str],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "TargetDatabase": DatabaseIdentifierTypeDef,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
 
-class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-):
+class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
 
-_RequiredDropNullFieldsOutputTypeDef = TypedDict(
-    "_RequiredDropNullFieldsOutputTypeDef",
+_RequiredDatabaseTypeDef = TypedDict(
+    "_RequiredDatabaseTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
     },
 )
-_OptionalDropNullFieldsOutputTypeDef = TypedDict(
-    "_OptionalDropNullFieldsOutputTypeDef",
+_OptionalDatabaseTypeDef = TypedDict(
+    "_OptionalDatabaseTypeDef",
     {
-        "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": List[NullValueFieldTypeDef],
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Dict[str, str],
+        "CreateTime": datetime,
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "TargetDatabase": DatabaseIdentifierTypeDef,
+        "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
+    },
+    total=False,
+)
+
+
+class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
+    pass
+
+
+ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+_RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetMLTaskRunsRequestRequestTypeDef",
+    {
+        "TransformId": str,
+    },
+)
+_OptionalGetMLTaskRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetMLTaskRunsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TaskRunFilterCriteriaTypeDef,
+        "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
 
-class DropNullFieldsOutputTypeDef(
-    _RequiredDropNullFieldsOutputTypeDef, _OptionalDropNullFieldsOutputTypeDef
+class GetMLTaskRunsRequestRequestTypeDef(
+    _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
     },
 )
 _OptionalDropNullFieldsTypeDef = TypedDict(
     "_OptionalDropNullFieldsTypeDef",
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": Sequence[NullValueFieldTypeDef],
+        "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
 
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
 
-_RequiredColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredColumnStatisticsDataOutputTypeDef",
+_RequiredColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
-_OptionalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalColumnStatisticsDataOutputTypeDef",
+_OptionalColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalColumnStatisticsDataTypeDef",
     {
         "BooleanColumnStatisticsData": BooleanColumnStatisticsDataTypeDef,
-        "DateColumnStatisticsData": DateColumnStatisticsDataOutputTypeDef,
-        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataOutputTypeDef,
+        "DateColumnStatisticsData": DateColumnStatisticsDataTypeDef,
+        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataTypeDef,
         "DoubleColumnStatisticsData": DoubleColumnStatisticsDataTypeDef,
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
 
-class ColumnStatisticsDataOutputTypeDef(
-    _RequiredColumnStatisticsDataOutputTypeDef, _OptionalColumnStatisticsDataOutputTypeDef
+class ColumnStatisticsDataTypeDef(
+    _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
 
-StorageDescriptorOutputTypeDef = TypedDict(
-    "StorageDescriptorOutputTypeDef",
-    {
-        "Columns": List[ColumnOutputTypeDef],
-        "Location": str,
-        "AdditionalLocations": List[str],
-        "InputFormat": str,
-        "OutputFormat": str,
-        "Compressed": bool,
-        "NumberOfBuckets": int,
-        "SerdeInfo": SerDeInfoOutputTypeDef,
-        "BucketColumns": List[str],
-        "SortColumns": List[OrderTypeDef],
-        "Parameters": Dict[str, str],
-        "SkewedInfo": SkewedInfoOutputTypeDef,
-        "StoredAsSubDirectories": bool,
-        "SchemaReference": SchemaReferenceTypeDef,
-    },
-    total=False,
-)
-
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -9466,60 +8288,47 @@
         "SkewedInfo": SkewedInfoTypeDef,
         "StoredAsSubDirectories": bool,
         "SchemaReference": SchemaReferenceTypeDef,
     },
     total=False,
 )
 
-SecurityConfigurationTypeDef = TypedDict(
-    "SecurityConfigurationTypeDef",
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
-        "CreatedTimeStamp": datetime,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
-    total=False,
 )
 
-CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateSecurityConfigurationRequestRequestTypeDef",
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
     {
         "Name": str,
+        "CreatedTimeStamp": datetime,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
+    total=False,
 )
 
-EncryptionConfigurationUnionTypeDef = Union[
-    EncryptionConfigurationTypeDef, EncryptionConfigurationOutputTypeDef
-]
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": List[FilterExpressionOutputTypeDef],
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": Sequence[FilterExpressionTypeDef],
+        "Filters": List[FilterExpressionTypeDef],
     },
 )
 
 _RequiredUpdateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -9568,475 +8377,29 @@
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredAthenaConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredAthenaConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-        "SchemaName": str,
-    },
-)
-_OptionalAthenaConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalAthenaConnectorSourceOutputTypeDef",
-    {
-        "ConnectionTable": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class AthenaConnectorSourceOutputTypeDef(
-    _RequiredAthenaConnectorSourceOutputTypeDef, _OptionalAthenaConnectorSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredCatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogDeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogDeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class CatalogDeltaSourceOutputTypeDef(
-    _RequiredCatalogDeltaSourceOutputTypeDef, _OptionalCatalogDeltaSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredCatalogHudiSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogHudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogHudiSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogHudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class CatalogHudiSourceOutputTypeDef(
-    _RequiredCatalogHudiSourceOutputTypeDef, _OptionalCatalogHudiSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredCustomCodeOutputTypeDef = TypedDict(
-    "_RequiredCustomCodeOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Code": str,
-        "ClassName": str,
-    },
-)
-_OptionalCustomCodeOutputTypeDef = TypedDict(
-    "_OptionalCustomCodeOutputTypeDef",
-    {
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class CustomCodeOutputTypeDef(_RequiredCustomCodeOutputTypeDef, _OptionalCustomCodeOutputTypeDef):
-    pass
-
-
-_RequiredDynamicTransformOutputTypeDef = TypedDict(
-    "_RequiredDynamicTransformOutputTypeDef",
-    {
-        "Name": str,
-        "TransformName": str,
-        "Inputs": List[str],
-        "FunctionName": str,
-        "Path": str,
-    },
-)
-_OptionalDynamicTransformOutputTypeDef = TypedDict(
-    "_OptionalDynamicTransformOutputTypeDef",
-    {
-        "Parameters": List[TransformConfigParameterOutputTypeDef],
-        "Version": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DynamicTransformOutputTypeDef(
-    _RequiredDynamicTransformOutputTypeDef, _OptionalDynamicTransformOutputTypeDef
-):
-    pass
-
-
-_RequiredJDBCConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredJDBCConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalJDBCConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalJDBCConnectorSourceOutputTypeDef",
-    {
-        "AdditionalOptions": JDBCConnectorOptionsOutputTypeDef,
-        "ConnectionTable": str,
-        "Query": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class JDBCConnectorSourceOutputTypeDef(
-    _RequiredJDBCConnectorSourceOutputTypeDef, _OptionalJDBCConnectorSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredJDBCConnectorTargetOutputTypeDef = TypedDict(
-    "_RequiredJDBCConnectorTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "ConnectionName": str,
-        "ConnectionTable": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalJDBCConnectorTargetOutputTypeDef = TypedDict(
-    "_OptionalJDBCConnectorTargetOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class JDBCConnectorTargetOutputTypeDef(
-    _RequiredJDBCConnectorTargetOutputTypeDef, _OptionalJDBCConnectorTargetOutputTypeDef
-):
-    pass
-
-
-_RequiredS3CatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogDeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogDeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3CatalogDeltaSourceOutputTypeDef(
-    _RequiredS3CatalogDeltaSourceOutputTypeDef, _OptionalS3CatalogDeltaSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3CatalogHudiSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogHudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogHudiSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogHudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3CatalogHudiSourceOutputTypeDef(
-    _RequiredS3CatalogHudiSourceOutputTypeDef, _OptionalS3CatalogHudiSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3CsvSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CsvSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-        "Separator": SeparatorType,
-        "QuoteChar": QuoteCharType,
-    },
-)
-_OptionalS3CsvSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CsvSourceOutputTypeDef",
-    {
-        "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "Escaper": str,
-        "Multiline": bool,
-        "WithHeader": bool,
-        "WriteHeader": bool,
-        "SkipFirst": bool,
-        "OptimizePerformance": bool,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3CsvSourceOutputTypeDef(
-    _RequiredS3CsvSourceOutputTypeDef, _OptionalS3CsvSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3DeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3DeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3DeltaSourceOutputTypeDef(
-    _RequiredS3DeltaSourceOutputTypeDef, _OptionalS3DeltaSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3HudiSourceOutputTypeDef = TypedDict(
-    "_RequiredS3HudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3HudiSourceOutputTypeDef = TypedDict(
-    "_OptionalS3HudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3HudiSourceOutputTypeDef(
-    _RequiredS3HudiSourceOutputTypeDef, _OptionalS3HudiSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3JsonSourceOutputTypeDef = TypedDict(
-    "_RequiredS3JsonSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3JsonSourceOutputTypeDef = TypedDict(
-    "_OptionalS3JsonSourceOutputTypeDef",
-    {
-        "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "JsonPath": str,
-        "Multiline": bool,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3JsonSourceOutputTypeDef(
-    _RequiredS3JsonSourceOutputTypeDef, _OptionalS3JsonSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredS3ParquetSourceOutputTypeDef = TypedDict(
-    "_RequiredS3ParquetSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3ParquetSourceOutputTypeDef = TypedDict(
-    "_OptionalS3ParquetSourceOutputTypeDef",
-    {
-        "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class S3ParquetSourceOutputTypeDef(
-    _RequiredS3ParquetSourceOutputTypeDef, _OptionalS3ParquetSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredSparkConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredSparkConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalSparkConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalSparkConnectorSourceOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class SparkConnectorSourceOutputTypeDef(
-    _RequiredSparkConnectorSourceOutputTypeDef, _OptionalSparkConnectorSourceOutputTypeDef
-):
-    pass
-
-
-_RequiredSparkConnectorTargetOutputTypeDef = TypedDict(
-    "_RequiredSparkConnectorTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalSparkConnectorTargetOutputTypeDef = TypedDict(
-    "_OptionalSparkConnectorTargetOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class SparkConnectorTargetOutputTypeDef(
-    _RequiredSparkConnectorTargetOutputTypeDef, _OptionalSparkConnectorTargetOutputTypeDef
-):
-    pass
-
-
-_RequiredSparkSQLOutputTypeDef = TypedDict(
-    "_RequiredSparkSQLOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "SqlQuery": str,
-        "SqlAliases": List[SqlAliasTypeDef],
-    },
-)
-_OptionalSparkSQLOutputTypeDef = TypedDict(
-    "_OptionalSparkSQLOutputTypeDef",
-    {
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class SparkSQLOutputTypeDef(_RequiredSparkSQLOutputTypeDef, _OptionalSparkSQLOutputTypeDef):
-    pass
-
-
 _RequiredAthenaConnectorSourceTypeDef = TypedDict(
     "_RequiredAthenaConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
         "SchemaName": str,
     },
 )
 _OptionalAthenaConnectorSourceTypeDef = TypedDict(
     "_OptionalAthenaConnectorSourceTypeDef",
     {
         "ConnectionTable": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
@@ -10051,16 +8414,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalCatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
@@ -10075,16 +8438,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogHudiSourceTypeDef = TypedDict(
     "_OptionalCatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
@@ -10092,48 +8455,48 @@
     pass
 
 
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Code": str,
         "ClassName": str,
     },
 )
 _OptionalCustomCodeTypeDef = TypedDict(
     "_OptionalCustomCodeTypeDef",
     {
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
 
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "FunctionName": str,
         "Path": str,
     },
 )
 _OptionalDynamicTransformTypeDef = TypedDict(
     "_OptionalDynamicTransformTypeDef",
     {
-        "Parameters": Sequence[TransformConfigParameterTypeDef],
+        "Parameters": List[TransformConfigParameterTypeDef],
         "Version": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
@@ -10150,15 +8513,15 @@
 )
 _OptionalJDBCConnectorSourceTypeDef = TypedDict(
     "_OptionalJDBCConnectorSourceTypeDef",
     {
         "AdditionalOptions": JDBCConnectorOptionsTypeDef,
         "ConnectionTable": str,
         "Query": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
@@ -10166,26 +8529,26 @@
     pass
 
 
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalJDBCConnectorTargetTypeDef = TypedDict(
     "_OptionalJDBCConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
@@ -10200,16 +8563,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalS3CatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
@@ -10224,16 +8587,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogHudiSourceTypeDef = TypedDict(
     "_OptionalS3CatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
@@ -10241,139 +8604,139 @@
     pass
 
 
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
     },
 )
 _OptionalS3CsvSourceTypeDef = TypedDict(
     "_OptionalS3CsvSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "Escaper": str,
         "Multiline": bool,
         "WithHeader": bool,
         "WriteHeader": bool,
         "SkipFirst": bool,
         "OptimizePerformance": bool,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
 
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3DeltaSourceTypeDef = TypedDict(
     "_OptionalS3DeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
+        "AdditionalDeltaOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
 
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3HudiSourceTypeDef = TypedDict(
     "_OptionalS3HudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
+        "AdditionalHudiOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
 
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3JsonSourceTypeDef = TypedDict(
     "_OptionalS3JsonSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "JsonPath": str,
         "Multiline": bool,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
 
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3ParquetSourceTypeDef = TypedDict(
     "_OptionalS3ParquetSourceTypeDef",
     {
         "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
@@ -10387,16 +8750,16 @@
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorSourceTypeDef = TypedDict(
     "_OptionalSparkConnectorSourceTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
@@ -10404,25 +8767,25 @@
     pass
 
 
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorTargetTypeDef = TypedDict(
     "_OptionalSparkConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
@@ -10430,23 +8793,23 @@
     pass
 
 
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "SqlQuery": str,
-        "SqlAliases": Sequence[SqlAliasTypeDef],
+        "SqlAliases": List[SqlAliasTypeDef],
     },
 )
 _OptionalSparkSQLTypeDef = TypedDict(
     "_OptionalSparkSQLTypeDef",
     {
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
@@ -10511,15 +8874,15 @@
     total=False,
 )
 
 _RequiredCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMLTransformRequestRequestTypeDef",
     {
         "Name": str,
-        "InputRecordTables": Sequence[GlueTableUnionTypeDef],
+        "InputRecordTables": Sequence[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "Role": str,
     },
 )
 _OptionalCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMLTransformRequestRequestTypeDef",
     {
@@ -10549,61 +8912,14 @@
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToDelete": Sequence[PartitionValueListUnionTypeDef],
-    },
-)
-_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchDeletePartitionRequestRequestTypeDef(
-    _RequiredBatchDeletePartitionRequestRequestTypeDef,
-    _OptionalBatchDeletePartitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToGet": Sequence[PartitionValueListUnionTypeDef],
-    },
-)
-_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchGetPartitionRequestRequestTypeDef(
-    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
 )
@@ -10674,89 +8990,23 @@
         "Progress": float,
         "StartedOn": int,
         "CompletedOn": int,
     },
     total=False,
 )
 
-_RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTriggerRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Type": TriggerTypeType,
-        "Actions": Sequence[ActionUnionTypeDef],
-    },
-)
-_OptionalCreateTriggerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTriggerRequestRequestTypeDef",
-    {
-        "WorkflowName": str,
-        "Schedule": str,
-        "Predicate": PredicateTypeDef,
-        "Description": str,
-        "StartOnCreation": bool,
-        "Tags": Mapping[str, str],
-        "EventBatchingCondition": EventBatchingConditionTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateTriggerRequestRequestTypeDef(
-    _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
-):
-    pass
-
-
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredColumnStatisticsDataTypeDef",
-    {
-        "Type": ColumnStatisticsTypeType,
-    },
-)
-_OptionalColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalColumnStatisticsDataTypeDef",
-    {
-        "BooleanColumnStatisticsData": BooleanColumnStatisticsDataTypeDef,
-        "DateColumnStatisticsData": DateColumnStatisticsDataTypeDef,
-        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataTypeDef,
-        "DoubleColumnStatisticsData": DoubleColumnStatisticsDataTypeDef,
-        "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
-        "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
-        "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
-    },
-    total=False,
-)
-
-
-class ColumnStatisticsDataTypeDef(
-    _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
-):
-    pass
-
-
-CreateScriptRequestRequestTypeDef = TypedDict(
-    "CreateScriptRequestRequestTypeDef",
-    {
-        "DagNodes": Sequence[CodeGenNodeUnionTypeDef],
-        "DagEdges": Sequence[CodeGenEdgeTypeDef],
-        "Language": LanguageType,
-    },
-    total=False,
-)
-
 BatchGetTriggersResponseTypeDef = TypedDict(
     "BatchGetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "TriggersNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -10808,15 +9058,15 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "InputRecordTables": List[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
         "Schema": List[SchemaColumnTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
@@ -10834,15 +9084,15 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "InputRecordTables": List[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
         "Schema": List[SchemaColumnTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
@@ -10877,31 +9127,80 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDatabaseResponseTypeDef = TypedDict(
-    "GetDatabaseResponseTypeDef",
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
     {
-        "Database": DatabaseTypeDef,
+        "Results": List[DataQualityResultDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDatabasesResponseTypeDef = TypedDict(
-    "GetDatabasesResponseTypeDef",
+ListDataQualityResultsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityResultsRequestRequestTypeDef",
     {
-        "DatabaseList": List[DatabaseTypeDef],
+        "Filter": DataQualityResultFilterCriteriaTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+BatchGetDataQualityResultResponseTypeDef = TypedDict(
+    "BatchGetDataQualityResultResponseTypeDef",
+    {
+        "Results": List[DataQualityResultTypeDef],
+        "ResultsNotFound": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
 _OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
@@ -10938,211 +9237,134 @@
 
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
 
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
-    {
-        "Results": List[DataQualityResultDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchGetDataQualityResultResponseTypeDef = TypedDict(
-    "BatchGetDataQualityResultResponseTypeDef",
-    {
-        "Results": List[DataQualityResultTypeDef],
-        "ResultsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+GetDatabaseResponseTypeDef = TypedDict(
+    "GetDatabaseResponseTypeDef",
     {
-        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
-        "NextToken": str,
+        "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+GetDatabasesResponseTypeDef = TypedDict(
+    "GetDatabasesResponseTypeDef",
     {
-        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
+        "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityResultsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityResultFilterCriteriaTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+ColumnStatisticsTypeDef = TypedDict(
+    "ColumnStatisticsTypeDef",
     {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "ColumnName": str,
+        "ColumnType": str,
+        "AnalyzedTime": datetime,
+        "StatisticsData": ColumnStatisticsDataTypeDef,
     },
-    total=False,
 )
 
-_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "RulesetNames": Sequence[str],
-    },
-)
-_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+PartitionInputTypeDef = TypedDict(
+    "PartitionInputTypeDef",
     {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "ClientToken": str,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "AdditionalDataSources": Mapping[str, DataSourceUnionTypeDef],
+        "Values": Sequence[str],
+        "LastAccessTime": TimestampTypeDef,
+        "StorageDescriptor": StorageDescriptorTypeDef,
+        "Parameters": Mapping[str, str],
+        "LastAnalyzedTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
-class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-):
-    pass
-
-
-ColumnStatisticsOutputTypeDef = TypedDict(
-    "ColumnStatisticsOutputTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnType": str,
-        "AnalyzedTime": datetime,
-        "StatisticsData": ColumnStatisticsDataOutputTypeDef,
-    },
-)
-
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "Values": List[str],
         "DatabaseName": str,
         "TableName": str,
         "CreationTime": datetime,
         "LastAccessTime": datetime,
-        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "StorageDescriptor": StorageDescriptorTypeDef,
         "Parameters": Dict[str, str],
         "LastAnalyzedTime": datetime,
         "CatalogId": str,
     },
     total=False,
 )
 
-_RequiredTableTypeDef = TypedDict(
-    "_RequiredTableTypeDef",
+_RequiredTableInputTypeDef = TypedDict(
+    "_RequiredTableInputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalTableTypeDef = TypedDict(
-    "_OptionalTableTypeDef",
+_OptionalTableInputTypeDef = TypedDict(
+    "_OptionalTableInputTypeDef",
     {
-        "DatabaseName": str,
         "Description": str,
         "Owner": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "LastAccessTime": datetime,
-        "LastAnalyzedTime": datetime,
+        "LastAccessTime": TimestampTypeDef,
+        "LastAnalyzedTime": TimestampTypeDef,
         "Retention": int,
-        "StorageDescriptor": StorageDescriptorOutputTypeDef,
-        "PartitionKeys": List[ColumnOutputTypeDef],
+        "StorageDescriptor": StorageDescriptorTypeDef,
+        "PartitionKeys": Sequence[ColumnTypeDef],
         "ViewOriginalText": str,
         "ViewExpandedText": str,
         "TableType": str,
-        "Parameters": Dict[str, str],
-        "CreatedBy": str,
-        "IsRegisteredWithLakeFormation": bool,
+        "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
-        "CatalogId": str,
-        "VersionId": str,
-        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
 
-class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
+class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
 
-PartitionInputTypeDef = TypedDict(
-    "PartitionInputTypeDef",
-    {
-        "Values": Sequence[str],
-        "LastAccessTime": TimestampTypeDef,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "Parameters": Mapping[str, str],
-        "LastAnalyzedTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTableInputTypeDef = TypedDict(
-    "_RequiredTableInputTypeDef",
+_RequiredTableTypeDef = TypedDict(
+    "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalTableInputTypeDef = TypedDict(
-    "_OptionalTableInputTypeDef",
+_OptionalTableTypeDef = TypedDict(
+    "_OptionalTableTypeDef",
     {
+        "DatabaseName": str,
         "Description": str,
         "Owner": str,
-        "LastAccessTime": TimestampTypeDef,
-        "LastAnalyzedTime": TimestampTypeDef,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "LastAccessTime": datetime,
+        "LastAnalyzedTime": datetime,
         "Retention": int,
         "StorageDescriptor": StorageDescriptorTypeDef,
-        "PartitionKeys": Sequence[ColumnTypeDef],
+        "PartitionKeys": List[ColumnTypeDef],
         "ViewOriginalText": str,
         "ViewExpandedText": str,
         "TableType": str,
-        "Parameters": Mapping[str, str],
+        "Parameters": Dict[str, str],
+        "CreatedBy": str,
+        "IsRegisteredWithLakeFormation": bool,
         "TargetTable": TableIdentifierTypeDef,
+        "CatalogId": str,
+        "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
 
-class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
+class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
 
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
@@ -11155,87 +9377,14 @@
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CodeGenConfigurationNodeOutputTypeDef = TypedDict(
-    "CodeGenConfigurationNodeOutputTypeDef",
-    {
-        "AthenaConnectorSource": AthenaConnectorSourceOutputTypeDef,
-        "JDBCConnectorSource": JDBCConnectorSourceOutputTypeDef,
-        "SparkConnectorSource": SparkConnectorSourceOutputTypeDef,
-        "CatalogSource": CatalogSourceTypeDef,
-        "RedshiftSource": RedshiftSourceTypeDef,
-        "S3CatalogSource": S3CatalogSourceTypeDef,
-        "S3CsvSource": S3CsvSourceOutputTypeDef,
-        "S3JsonSource": S3JsonSourceOutputTypeDef,
-        "S3ParquetSource": S3ParquetSourceOutputTypeDef,
-        "RelationalCatalogSource": RelationalCatalogSourceTypeDef,
-        "DynamoDBCatalogSource": DynamoDBCatalogSourceTypeDef,
-        "JDBCConnectorTarget": JDBCConnectorTargetOutputTypeDef,
-        "SparkConnectorTarget": SparkConnectorTargetOutputTypeDef,
-        "CatalogTarget": BasicCatalogTargetOutputTypeDef,
-        "RedshiftTarget": RedshiftTargetOutputTypeDef,
-        "S3CatalogTarget": S3CatalogTargetOutputTypeDef,
-        "S3GlueParquetTarget": S3GlueParquetTargetOutputTypeDef,
-        "S3DirectTarget": S3DirectTargetOutputTypeDef,
-        "ApplyMapping": ApplyMappingOutputTypeDef,
-        "SelectFields": SelectFieldsOutputTypeDef,
-        "DropFields": DropFieldsOutputTypeDef,
-        "RenameField": RenameFieldOutputTypeDef,
-        "Spigot": SpigotOutputTypeDef,
-        "Join": JoinOutputTypeDef,
-        "SplitFields": SplitFieldsOutputTypeDef,
-        "SelectFromCollection": SelectFromCollectionOutputTypeDef,
-        "FillMissingValues": FillMissingValuesOutputTypeDef,
-        "Filter": FilterOutputTypeDef,
-        "CustomCode": CustomCodeOutputTypeDef,
-        "SparkSQL": SparkSQLOutputTypeDef,
-        "DirectKinesisSource": DirectKinesisSourceOutputTypeDef,
-        "DirectKafkaSource": DirectKafkaSourceOutputTypeDef,
-        "CatalogKinesisSource": CatalogKinesisSourceOutputTypeDef,
-        "CatalogKafkaSource": CatalogKafkaSourceOutputTypeDef,
-        "DropNullFields": DropNullFieldsOutputTypeDef,
-        "Merge": MergeOutputTypeDef,
-        "Union": UnionOutputTypeDef,
-        "PIIDetection": PIIDetectionOutputTypeDef,
-        "Aggregate": AggregateOutputTypeDef,
-        "DropDuplicates": DropDuplicatesOutputTypeDef,
-        "GovernedCatalogTarget": GovernedCatalogTargetOutputTypeDef,
-        "GovernedCatalogSource": GovernedCatalogSourceTypeDef,
-        "MicrosoftSQLServerCatalogSource": MicrosoftSQLServerCatalogSourceTypeDef,
-        "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
-        "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
-        "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
-        "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetOutputTypeDef,
-        "MySQLCatalogTarget": MySQLCatalogTargetOutputTypeDef,
-        "OracleSQLCatalogTarget": OracleSQLCatalogTargetOutputTypeDef,
-        "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetOutputTypeDef,
-        "DynamicTransform": DynamicTransformOutputTypeDef,
-        "EvaluateDataQuality": EvaluateDataQualityOutputTypeDef,
-        "S3CatalogHudiSource": S3CatalogHudiSourceOutputTypeDef,
-        "CatalogHudiSource": CatalogHudiSourceOutputTypeDef,
-        "S3HudiSource": S3HudiSourceOutputTypeDef,
-        "S3HudiCatalogTarget": S3HudiCatalogTargetOutputTypeDef,
-        "S3HudiDirectTarget": S3HudiDirectTargetOutputTypeDef,
-        "DirectJDBCSource": DirectJDBCSourceTypeDef,
-        "S3CatalogDeltaSource": S3CatalogDeltaSourceOutputTypeDef,
-        "CatalogDeltaSource": CatalogDeltaSourceOutputTypeDef,
-        "S3DeltaSource": S3DeltaSourceOutputTypeDef,
-        "S3DeltaCatalogTarget": S3DeltaCatalogTargetOutputTypeDef,
-        "S3DeltaDirectTarget": S3DeltaDirectTargetOutputTypeDef,
-        "AmazonRedshiftSource": AmazonRedshiftSourceOutputTypeDef,
-        "AmazonRedshiftTarget": AmazonRedshiftTargetOutputTypeDef,
-        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameOutputTypeDef,
-    },
-    total=False,
-)
-
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
         "JDBCConnectorSource": JDBCConnectorSourceTypeDef,
         "SparkConnectorSource": SparkConnectorSourceTypeDef,
         "CatalogSource": CatalogSourceTypeDef,
@@ -11327,24 +9476,14 @@
     {
         "Statements": List[StatementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnStatisticsTypeDef = TypedDict(
-    "ColumnStatisticsTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnType": str,
-        "AnalyzedTime": TimestampTypeDef,
-        "StatisticsData": ColumnStatisticsDataTypeDef,
-    },
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Type": NodeTypeType,
         "Name": str,
         "UniqueId": str,
         "TriggerDetails": TriggerNodeDetailsTypeDef,
@@ -11362,129 +9501,86 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
-        "ColumnStatistics": ColumnStatisticsOutputTypeDef,
+        "ColumnStatistics": ColumnStatisticsTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetPartitionResponseTypeDef = TypedDict(
-    "BatchGetPartitionResponseTypeDef",
+_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
-        "Partitions": List[PartitionTypeDef],
-        "UnprocessedKeys": List[PartitionValueListOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionValues": Sequence[str],
+        "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
 )
-
-GetPartitionResponseTypeDef = TypedDict(
-    "GetPartitionResponseTypeDef",
+_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
-        "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CatalogId": str,
     },
+    total=False,
 )
 
-GetPartitionsResponseTypeDef = TypedDict(
-    "GetPartitionsResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionMetadataResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
+    _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
+    _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
+):
+    pass
 
-UnfilteredPartitionTypeDef = TypedDict(
-    "UnfilteredPartitionTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-    },
-    total=False,
-)
 
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
+_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
-        "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DatabaseName": str,
+        "TableName": str,
+        "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
 )
-
-GetTablesResponseTypeDef = TypedDict(
-    "GetTablesResponseTypeDef",
+_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
-        "TableList": List[TableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CatalogId": str,
     },
+    total=False,
 )
 
-GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredTableMetadataResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-SearchTablesResponseTypeDef = TypedDict(
-    "SearchTablesResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateColumnStatisticsForTableRequestRequestTypeDef(
+    _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
+    _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
+):
+    pass
 
-TableVersionTypeDef = TypedDict(
-    "TableVersionTypeDef",
-    {
-        "Table": TableTypeDef,
-        "VersionId": str,
-    },
-    total=False,
-)
 
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
@@ -11557,14 +9653,60 @@
 
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
 
+BatchGetPartitionResponseTypeDef = TypedDict(
+    "BatchGetPartitionResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "UnprocessedKeys": List[PartitionValueListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionResponseTypeDef = TypedDict(
+    "GetPartitionResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionsResponseTypeDef = TypedDict(
+    "GetPartitionsResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionMetadataResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnfilteredPartitionTypeDef = TypedDict(
+    "UnfilteredPartitionTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+    },
+    total=False,
+)
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -11606,47 +9748,131 @@
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
 
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTablesResponseTypeDef = TypedDict(
+    "GetTablesResponseTypeDef",
+    {
+        "TableList": List[TableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredTableMetadataResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "CellFilters": List[ColumnRowFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchTablesResponseTypeDef = TypedDict(
+    "SearchTablesResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableVersionTypeDef = TypedDict(
+    "TableVersionTypeDef",
+    {
+        "Table": TableTypeDef,
+        "VersionId": str,
+    },
+    total=False,
+)
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Role": str,
+        "Command": JobCommandTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LogUri": str,
+        "ExecutionProperty": ExecutionPropertyTypeDef,
+        "DefaultArguments": Mapping[str, str],
+        "NonOverridableArguments": Mapping[str, str],
+        "Connections": ConnectionsListTypeDef,
+        "MaxRetries": int,
+        "AllocatedCapacity": int,
+        "Timeout": int,
+        "MaxCapacity": float,
+        "SecurityConfiguration": str,
+        "Tags": Mapping[str, str],
+        "NotificationProperty": NotificationPropertyTypeDef,
+        "GlueVersion": str,
+        "NumberOfWorkers": int,
+        "WorkerType": WorkerTypeType,
+        "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
+        "ExecutionClass": ExecutionClassType,
+        "SourceControlDetails": SourceControlDetailsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
+
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "ExecutionProperty": ExecutionPropertyTypeDef,
         "Command": JobCommandTypeDef,
         "DefaultArguments": Dict[str, str],
         "NonOverridableArguments": Dict[str, str],
-        "Connections": ConnectionsListOutputTypeDef,
+        "Connections": ConnectionsListTypeDef,
         "MaxRetries": int,
         "AllocatedCapacity": int,
         "Timeout": int,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "GlueVersion": str,
-        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeOutputTypeDef],
+        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-CodeGenConfigurationNodeUnionTypeDef = Union[
-    CodeGenConfigurationNodeTypeDef, CodeGenConfigurationNodeOutputTypeDef
-]
 JobUpdateTypeDef = TypedDict(
     "JobUpdateTypeDef",
     {
         "Description": str,
         "LogUri": str,
         "Role": str,
         "ExecutionProperty": ExecutionPropertyTypeDef,
@@ -11666,15 +9892,14 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-ColumnStatisticsUnionTypeDef = Union[ColumnStatisticsTypeDef, ColumnStatisticsOutputTypeDef]
 WorkflowGraphTypeDef = TypedDict(
     "WorkflowGraphTypeDef",
     {
         "Nodes": List[NodeTypeDef],
         "Edges": List[EdgeTypeDef],
     },
     total=False,
@@ -11692,14 +9917,38 @@
     "UpdateColumnStatisticsForTableResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "Entries": Sequence[BatchUpdatePartitionRequestEntryTypeDef],
+    },
+)
+_OptionalBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class BatchUpdatePartitionRequestRequestTypeDef(
+    _RequiredBatchUpdatePartitionRequestRequestTypeDef,
+    _OptionalBatchUpdatePartitionRequestRequestTypeDef,
+):
+    pass
+
+
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11718,38 +9967,14 @@
     {
         "TableVersions": List[TableVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "Entries": Sequence[BatchUpdatePartitionRequestEntryTypeDef],
-    },
-)
-_OptionalBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchUpdatePartitionRequestRequestTypeDef(
-    _RequiredBatchUpdatePartitionRequestRequestTypeDef,
-    _OptionalBatchUpdatePartitionRequestRequestTypeDef,
-):
-    pass
-
-
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11768,112 +9993,22 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Role": str,
-        "Command": JobCommandTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LogUri": str,
-        "ExecutionProperty": ExecutionPropertyTypeDef,
-        "DefaultArguments": Mapping[str, str],
-        "NonOverridableArguments": Mapping[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "MaxRetries": int,
-        "AllocatedCapacity": int,
-        "Timeout": int,
-        "MaxCapacity": float,
-        "SecurityConfiguration": str,
-        "Tags": Mapping[str, str],
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "GlueVersion": str,
-        "NumberOfWorkers": int,
-        "WorkerType": WorkerTypeType,
-        "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeUnionTypeDef],
-        "ExecutionClass": ExecutionClassType,
-        "SourceControlDetails": SourceControlDetailsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-
 UpdateJobRequestRequestTypeDef = TypedDict(
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
         "JobUpdate": JobUpdateTypeDef,
     },
 )
 
-_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionValues": Sequence[str],
-        "ColumnStatisticsList": Sequence[ColumnStatisticsUnionTypeDef],
-    },
-)
-_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
-    _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
-    _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "ColumnStatisticsList": Sequence[ColumnStatisticsUnionTypeDef],
-    },
-)
-_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class UpdateColumnStatisticsForTableRequestRequestTypeDef(
-    _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
-    _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
-):
-    pass
-
-
 WorkflowRunTypeDef = TypedDict(
     "WorkflowRunTypeDef",
     {
         "Name": str,
         "WorkflowRunId": str,
         "PreviousRunId": str,
         "WorkflowRunProperties": Dict[str, str],
```

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue/type_defs.pyi` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_glue.type_defs import NotificationPropertyTypeDef
 
     data: NotificationPropertyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Mapping, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
@@ -108,23 +106,20 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "NotificationPropertyTypeDef",
-    "AggregateOperationOutputTypeDef",
     "AggregateOperationTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
     "OptionTypeDef",
-    "ApplyMappingOutputTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
-    "PartitionValueListOutputTypeDef",
-    "BasicCatalogTargetOutputTypeDef",
+    "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
@@ -136,104 +131,80 @@
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
-    "BlobTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
     "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
-    "KafkaStreamingSourceOptionsOutputTypeDef",
+    "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
-    "KinesisStreamingSourceOptionsOutputTypeDef",
+    "KinesisStreamingSourceOptionsTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
     "CatalogSourceTypeDef",
-    "CatalogTargetOutputTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
     "DirectJDBCSourceTypeDef",
-    "DropDuplicatesOutputTypeDef",
-    "DropFieldsOutputTypeDef",
-    "DynamoDBCatalogSourceTypeDef",
-    "FillMissingValuesOutputTypeDef",
-    "MergeOutputTypeDef",
-    "MicrosoftSQLServerCatalogSourceTypeDef",
-    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
-    "MySQLCatalogSourceTypeDef",
-    "MySQLCatalogTargetOutputTypeDef",
-    "OracleSQLCatalogSourceTypeDef",
-    "OracleSQLCatalogTargetOutputTypeDef",
-    "PIIDetectionOutputTypeDef",
-    "PostgreSQLCatalogSourceTypeDef",
-    "PostgreSQLCatalogTargetOutputTypeDef",
-    "RedshiftSourceTypeDef",
-    "RelationalCatalogSourceTypeDef",
-    "RenameFieldOutputTypeDef",
-    "SelectFieldsOutputTypeDef",
-    "SelectFromCollectionOutputTypeDef",
-    "SpigotOutputTypeDef",
-    "SplitFieldsOutputTypeDef",
-    "UnionOutputTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
+    "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
+    "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
+    "MySQLCatalogSourceTypeDef",
     "MySQLCatalogTargetTypeDef",
+    "OracleSQLCatalogSourceTypeDef",
     "OracleSQLCatalogTargetTypeDef",
     "PIIDetectionTypeDef",
+    "PostgreSQLCatalogSourceTypeDef",
     "PostgreSQLCatalogTargetTypeDef",
+    "RedshiftSourceTypeDef",
+    "RelationalCatalogSourceTypeDef",
     "RenameFieldTypeDef",
     "SelectFieldsTypeDef",
     "SelectFromCollectionTypeDef",
     "SpigotTypeDef",
     "SplitFieldsTypeDef",
     "UnionTypeDef",
     "CodeGenEdgeTypeDef",
     "CodeGenNodeArgTypeDef",
     "ColumnImportanceTypeDef",
-    "ColumnOutputTypeDef",
     "ColumnRowFilterTypeDef",
-    "DateColumnStatisticsDataOutputTypeDef",
+    "DateColumnStatisticsDataTypeDef",
     "DoubleColumnStatisticsDataTypeDef",
     "LongColumnStatisticsDataTypeDef",
     "StringColumnStatisticsDataTypeDef",
-    "TimestampTypeDef",
     "ColumnTypeDef",
     "ConditionTypeDef",
     "ConfusionMatrixTypeDef",
     "PhysicalConnectionRequirementsTypeDef",
     "ConnectionPasswordEncryptionTypeDef",
-    "PhysicalConnectionRequirementsOutputTypeDef",
-    "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
-    "DeltaTargetOutputTypeDef",
-    "DynamoDBTargetTypeDef",
-    "JdbcTargetOutputTypeDef",
-    "MongoDBTargetTypeDef",
-    "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
+    "DynamoDBTargetTypeDef",
     "JdbcTargetTypeDef",
+    "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
     "ScheduleTypeDef",
     "SchemaChangePolicyTypeDef",
@@ -245,32 +216,32 @@
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
     "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
+    "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "DQResultsPublishingOptionsTypeDef",
     "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    "TimestampTypeDef",
     "DataQualityRuleResultTypeDef",
-    "GlueTableOutputTypeDef",
-    "GlueTableTypeDef",
     "DatabaseIdentifierTypeDef",
     "FederatedDatabaseTypeDef",
     "DatatypeTypeDef",
-    "DecimalNumberOutputTypeDef",
+    "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
@@ -289,23 +260,21 @@
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
-    "TransformConfigParameterOutputTypeDef",
     "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FederatedTableTypeDef",
-    "FilterValueOutputTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
@@ -364,18 +333,16 @@
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
-    "JDBCConnectorOptionsOutputTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
-    "JoinColumnOutputTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
     "ListCrawlersRequestRequestTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
@@ -385,34 +352,29 @@
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MLUserDataEncryptionTypeDef",
-    "MappingOutputTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
-    "PartitionValueListTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
-    "UpsertRedshiftTargetOptionsOutputTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
-    "SerDeInfoOutputTypeDef",
     "SerDeInfoTypeDef",
-    "SkewedInfoOutputTypeDef",
     "SkewedInfoTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
@@ -437,24 +399,23 @@
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "AggregateOutputTypeDef",
     "AggregateTypeDef",
-    "AmazonRedshiftNodeDataOutputTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
+    "BatchDeletePartitionRequestRequestTypeDef",
+    "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
     "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
@@ -526,98 +487,75 @@
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
     "BatchGetCustomEntityTypesResponseTypeDef",
     "ListCustomEntityTypesResponseTypeDef",
     "BatchGetDevEndpointsResponseTypeDef",
     "GetDevEndpointResponseTypeDef",
     "GetDevEndpointsResponseTypeDef",
-    "DecimalNumberTypeDef",
     "GetBlueprintRunResponseTypeDef",
     "GetBlueprintRunsResponseTypeDef",
     "BlueprintTypeDef",
     "GetCatalogImportStatusResponseTypeDef",
-    "CatalogKafkaSourceOutputTypeDef",
-    "DirectKafkaSourceOutputTypeDef",
-    "CatalogKinesisSourceOutputTypeDef",
-    "DirectKinesisSourceOutputTypeDef",
-    "GovernedCatalogTargetOutputTypeDef",
+    "CatalogKafkaSourceTypeDef",
+    "DirectKafkaSourceTypeDef",
+    "CatalogKinesisSourceTypeDef",
+    "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
-    "S3CatalogTargetOutputTypeDef",
     "S3CatalogTargetTypeDef",
-    "S3DeltaCatalogTargetOutputTypeDef",
     "S3DeltaCatalogTargetTypeDef",
-    "S3HudiCatalogTargetOutputTypeDef",
     "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
-    "CodeGenNodeOutputTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
-    "DateColumnStatisticsDataTypeDef",
-    "GetTableRequestRequestTypeDef",
-    "GetTablesRequestRequestTypeDef",
-    "KafkaStreamingSourceOptionsTypeDef",
-    "KinesisStreamingSourceOptionsTypeDef",
-    "TaskRunFilterCriteriaTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
-    "ConnectionsListUnionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
-    "CrawlerTargetsOutputTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
     "CreateDataQualityRulesetRequestRequestTypeDef",
-    "DataQualityRulesetFilterCriteriaTypeDef",
     "DataQualityRulesetListDetailsTypeDef",
     "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
-    "EvaluateDataQualityMultiFrameOutputTypeDef",
     "EvaluateDataQualityMultiFrameTypeDef",
-    "EvaluateDataQualityOutputTypeDef",
     "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
-    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
-    "DataSourceOutputTypeDef",
-    "DataSourceTypeDef",
-    "GlueTableUnionTypeDef",
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    "GetTableRequestRequestTypeDef",
+    "GetTablesRequestRequestTypeDef",
+    "TaskRunFilterCriteriaTypeDef",
     "NullValueFieldTypeDef",
-    "DecimalColumnStatisticsDataOutputTypeDef",
+    "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
-    "S3DeltaDirectTargetOutputTypeDef",
     "S3DeltaDirectTargetTypeDef",
-    "S3DirectTargetOutputTypeDef",
     "S3DirectTargetTypeDef",
-    "S3GlueParquetTargetOutputTypeDef",
     "S3GlueParquetTargetTypeDef",
-    "S3HudiDirectTargetOutputTypeDef",
     "S3HudiDirectTargetTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
-    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
@@ -642,128 +580,94 @@
     "GetPartitionsRequestGetPartitionsPaginateTypeDef",
     "GetPartitionsRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
-    "GlueSchemaOutputTypeDef",
     "GlueSchemaTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
     "JobRunTypeDef",
-    "JoinOutputTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
-    "PartitionValueListUnionTypeDef",
-    "RedshiftTargetOutputTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
-    "ActionUnionTypeDef",
-    "AmazonRedshiftSourceOutputTypeDef",
-    "AmazonRedshiftTargetOutputTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
-    "DecimalColumnStatisticsDataTypeDef",
     "BatchGetBlueprintsResponseTypeDef",
     "GetBlueprintResponseTypeDef",
     "GetClassifierResponseTypeDef",
     "GetClassifiersResponseTypeDef",
+    "CreateScriptRequestRequestTypeDef",
     "GetDataflowGraphResponseTypeDef",
-    "CodeGenNodeUnionTypeDef",
     "GetMappingRequestRequestTypeDef",
     "GetPlanRequestRequestTypeDef",
-    "CatalogKafkaSourceTypeDef",
-    "DirectKafkaSourceTypeDef",
-    "CatalogKinesisSourceTypeDef",
-    "DirectKinesisSourceTypeDef",
-    "GetMLTaskRunsRequestRequestTypeDef",
+    "CreateTriggerRequestRequestTypeDef",
     "TriggerTypeDef",
-    "PredicateUnionTypeDef",
     "TriggerUpdateTypeDef",
     "EvaluationMetricsTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
-    "CrawlerTargetsUnionTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
-    "ListDataQualityRulesetsRequestRequestTypeDef",
     "ListDataQualityRulesetsResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
-    "ListSessionsResponseTypeDef",
-    "GetDataCatalogEncryptionSettingsResponseTypeDef",
-    "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "DatabaseTypeDef",
-    "DatabaseInputTypeDef",
     "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultFilterCriteriaTypeDef",
     "DataQualityResultTypeDef",
     "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRuleRecommendationRunFilterTypeDef",
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunFilterTypeDef",
     "GetDataQualityResultResponseTypeDef",
     "GetDataQualityRuleRecommendationRunResponseTypeDef",
     "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "DataSourceUnionTypeDef",
     "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "DropNullFieldsOutputTypeDef",
+    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "ListSessionsResponseTypeDef",
+    "GetDataCatalogEncryptionSettingsResponseTypeDef",
+    "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    "DatabaseInputTypeDef",
+    "DatabaseTypeDef",
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    "GetMLTaskRunsRequestRequestTypeDef",
     "DropNullFieldsTypeDef",
-    "ColumnStatisticsDataOutputTypeDef",
-    "StorageDescriptorOutputTypeDef",
+    "ColumnStatisticsDataTypeDef",
     "StorageDescriptorTypeDef",
-    "SecurityConfigurationTypeDef",
     "CreateSecurityConfigurationRequestRequestTypeDef",
-    "EncryptionConfigurationUnionTypeDef",
+    "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
-    "AthenaConnectorSourceOutputTypeDef",
-    "CatalogDeltaSourceOutputTypeDef",
-    "CatalogHudiSourceOutputTypeDef",
-    "CustomCodeOutputTypeDef",
-    "DynamicTransformOutputTypeDef",
-    "JDBCConnectorSourceOutputTypeDef",
-    "JDBCConnectorTargetOutputTypeDef",
-    "S3CatalogDeltaSourceOutputTypeDef",
-    "S3CatalogHudiSourceOutputTypeDef",
-    "S3CsvSourceOutputTypeDef",
-    "S3DeltaSourceOutputTypeDef",
-    "S3HudiSourceOutputTypeDef",
-    "S3JsonSourceOutputTypeDef",
-    "S3ParquetSourceOutputTypeDef",
-    "SparkConnectorSourceOutputTypeDef",
-    "SparkConnectorTargetOutputTypeDef",
-    "SparkSQLOutputTypeDef",
     "AthenaConnectorSourceTypeDef",
     "CatalogDeltaSourceTypeDef",
     "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
@@ -780,100 +684,90 @@
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
     "TaskRunTypeDef",
     "CreateMLTransformRequestRequestTypeDef",
     "QuerySchemaVersionMetadataResponseTypeDef",
-    "BatchDeletePartitionRequestRequestTypeDef",
-    "BatchGetPartitionRequestRequestTypeDef",
     "CreateUserDefinedFunctionRequestRequestTypeDef",
     "UpdateUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionResponseTypeDef",
     "GetUserDefinedFunctionsResponseTypeDef",
     "StatementTypeDef",
-    "CreateTriggerRequestRequestTypeDef",
     "GetPartitionIndexesResponseTypeDef",
-    "ColumnStatisticsDataTypeDef",
-    "CreateScriptRequestRequestTypeDef",
     "BatchGetTriggersResponseTypeDef",
     "GetTriggerResponseTypeDef",
     "GetTriggersResponseTypeDef",
     "TriggerNodeDetailsTypeDef",
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "GetDatabaseResponseTypeDef",
-    "GetDatabasesResponseTypeDef",
-    "CreateDatabaseRequestRequestTypeDef",
-    "UpdateDatabaseRequestRequestTypeDef",
     "ListDataQualityResultsResponseTypeDef",
+    "ListDataQualityResultsRequestRequestTypeDef",
     "BatchGetDataQualityResultResponseTypeDef",
     "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    "ListDataQualityResultsRequestRequestTypeDef",
     "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
     "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "ColumnStatisticsOutputTypeDef",
-    "PartitionTypeDef",
-    "TableTypeDef",
+    "CreateDatabaseRequestRequestTypeDef",
+    "UpdateDatabaseRequestRequestTypeDef",
+    "GetDatabaseResponseTypeDef",
+    "GetDatabasesResponseTypeDef",
+    "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
+    "PartitionTypeDef",
     "TableInputTypeDef",
+    "TableTypeDef",
     "GetSecurityConfigurationResponseTypeDef",
     "GetSecurityConfigurationsResponseTypeDef",
-    "CodeGenConfigurationNodeOutputTypeDef",
     "CodeGenConfigurationNodeTypeDef",
     "GetMLTaskRunsResponseTypeDef",
     "GetStatementResponseTypeDef",
     "ListStatementsResponseTypeDef",
-    "ColumnStatisticsTypeDef",
     "NodeTypeDef",
     "GetMLTransformsResponseTypeDef",
     "ColumnStatisticsErrorTypeDef",
     "GetColumnStatisticsForPartitionResponseTypeDef",
     "GetColumnStatisticsForTableResponseTypeDef",
+    "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
+    "UpdateColumnStatisticsForTableRequestRequestTypeDef",
+    "BatchCreatePartitionRequestRequestTypeDef",
+    "BatchUpdatePartitionRequestEntryTypeDef",
+    "CreatePartitionRequestRequestTypeDef",
+    "UpdatePartitionRequestRequestTypeDef",
     "BatchGetPartitionResponseTypeDef",
     "GetPartitionResponseTypeDef",
     "GetPartitionsResponseTypeDef",
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     "UnfilteredPartitionTypeDef",
+    "CreateTableRequestRequestTypeDef",
+    "UpdateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
     "GetTablesResponseTypeDef",
     "GetUnfilteredTableMetadataResponseTypeDef",
     "SearchTablesResponseTypeDef",
     "TableVersionTypeDef",
-    "BatchCreatePartitionRequestRequestTypeDef",
-    "BatchUpdatePartitionRequestEntryTypeDef",
-    "CreatePartitionRequestRequestTypeDef",
-    "UpdatePartitionRequestRequestTypeDef",
-    "CreateTableRequestRequestTypeDef",
-    "UpdateTableRequestRequestTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "CodeGenConfigurationNodeUnionTypeDef",
     "JobUpdateTypeDef",
-    "ColumnStatisticsUnionTypeDef",
     "WorkflowGraphTypeDef",
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     "UpdateColumnStatisticsForTableResponseTypeDef",
+    "BatchUpdatePartitionRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     "GetTableVersionResponseTypeDef",
     "GetTableVersionsResponseTypeDef",
-    "BatchUpdatePartitionRequestRequestTypeDef",
     "BatchGetJobsResponseTypeDef",
     "GetJobResponseTypeDef",
     "GetJobsResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    "UpdateColumnStatisticsForTableRequestRequestTypeDef",
     "WorkflowRunTypeDef",
     "GetWorkflowRunResponseTypeDef",
     "GetWorkflowRunsResponseTypeDef",
     "WorkflowTypeDef",
     "BatchGetWorkflowsResponseTypeDef",
     "GetWorkflowResponseTypeDef",
 )
@@ -882,26 +776,18 @@
     "NotificationPropertyTypeDef",
     {
         "NotifyDelayAfter": int,
     },
     total=False,
 )
 
-AggregateOperationOutputTypeDef = TypedDict(
-    "AggregateOperationOutputTypeDef",
-    {
-        "Column": List[str],
-        "AggFunc": AggFunctionType,
-    },
-)
-
 AggregateOperationTypeDef = TypedDict(
     "AggregateOperationTypeDef",
     {
-        "Column": Sequence[str],
+        "Column": List[str],
         "AggFunc": AggFunctionType,
     },
 )
 
 AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
     "AmazonRedshiftAdvancedOptionTypeDef",
     {
@@ -917,64 +803,45 @@
         "Value": str,
         "Label": str,
         "Description": str,
     },
     total=False,
 )
 
-ApplyMappingOutputTypeDef = TypedDict(
-    "ApplyMappingOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Mapping": List["MappingOutputTypeDef"],
-    },
-)
-
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Mapping": Sequence["MappingTypeDef"],
+        "Inputs": List[str],
+        "Mapping": List["MappingTypeDef"],
     },
 )
 
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
         "RequestedColumns": Sequence[str],
         "AllColumnsRequested": bool,
     },
     total=False,
 )
 
-PartitionValueListOutputTypeDef = TypedDict(
-    "PartitionValueListOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
-BasicCatalogTargetOutputTypeDef = TypedDict(
-    "BasicCatalogTargetOutputTypeDef",
+PartitionValueListTypeDef = TypedDict(
+    "PartitionValueListTypeDef",
     {
-        "Name": str,
-        "Inputs": List[str],
-        "Database": str,
-        "Table": str,
+        "Values": Sequence[str],
     },
 )
 
 BasicCatalogTargetTypeDef = TypedDict(
     "BasicCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -1213,15 +1080,14 @@
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BlueprintDetailsTypeDef = TypedDict(
     "BlueprintDetailsTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
     total=False,
@@ -1321,16 +1187,16 @@
         "ImportCompleted": bool,
         "ImportTime": datetime,
         "ImportedBy": str,
     },
     total=False,
 )
 
-KafkaStreamingSourceOptionsOutputTypeDef = TypedDict(
-    "KafkaStreamingSourceOptionsOutputTypeDef",
+KafkaStreamingSourceOptionsTypeDef = TypedDict(
+    "KafkaStreamingSourceOptionsTypeDef",
     {
         "BootstrapServers": str,
         "SecurityProtocol": str,
         "ConnectionName": str,
         "TopicName": str,
         "Assign": str,
         "SubscribePattern": str,
@@ -1356,16 +1222,16 @@
     {
         "PollingTime": int,
         "RecordPollingLimit": int,
     },
     total=False,
 )
 
-KinesisStreamingSourceOptionsOutputTypeDef = TypedDict(
-    "KinesisStreamingSourceOptionsOutputTypeDef",
+KinesisStreamingSourceOptionsTypeDef = TypedDict(
+    "KinesisStreamingSourceOptionsTypeDef",
     {
         "EndpointUrl": str,
         "StreamName": str,
         "Classification": str,
         "Delimiter": str,
         "StartingPosition": StartingPositionType,
         "MaxFetchTimeInMs": int,
@@ -1402,41 +1268,19 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredCatalogTargetOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "Tables": List[str],
-    },
-)
-_OptionalCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalCatalogTargetOutputTypeDef",
-    {
-        "ConnectionName": str,
-        "EventQueueArn": str,
-        "DlqEventQueueArn": str,
-    },
-    total=False,
-)
-
-class CatalogTargetOutputTypeDef(
-    _RequiredCatalogTargetOutputTypeDef, _OptionalCatalogTargetOutputTypeDef
-):
-    pass
-
 _RequiredCatalogTargetTypeDef = TypedDict(
     "_RequiredCatalogTargetTypeDef",
     {
         "DatabaseName": str,
-        "Tables": Sequence[str],
+        "Tables": List[str],
     },
 )
 _OptionalCatalogTargetTypeDef = TypedDict(
     "_OptionalCatalogTargetTypeDef",
     {
         "ConnectionName": str,
         "EventQueueArn": str,
@@ -1572,36 +1416,34 @@
     },
     total=False,
 )
 
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
-_RequiredDropDuplicatesOutputTypeDef = TypedDict(
-    "_RequiredDropDuplicatesOutputTypeDef",
+_RequiredDropDuplicatesTypeDef = TypedDict(
+    "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
-_OptionalDropDuplicatesOutputTypeDef = TypedDict(
-    "_OptionalDropDuplicatesOutputTypeDef",
+_OptionalDropDuplicatesTypeDef = TypedDict(
+    "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
-class DropDuplicatesOutputTypeDef(
-    _RequiredDropDuplicatesOutputTypeDef, _OptionalDropDuplicatesOutputTypeDef
-):
+class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
-DropFieldsOutputTypeDef = TypedDict(
-    "DropFieldsOutputTypeDef",
+DropFieldsTypeDef = TypedDict(
+    "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
 )
 
@@ -1610,37 +1452,37 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredFillMissingValuesOutputTypeDef = TypedDict(
-    "_RequiredFillMissingValuesOutputTypeDef",
+_RequiredFillMissingValuesTypeDef = TypedDict(
+    "_RequiredFillMissingValuesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ImputedPath": str,
     },
 )
-_OptionalFillMissingValuesOutputTypeDef = TypedDict(
-    "_OptionalFillMissingValuesOutputTypeDef",
+_OptionalFillMissingValuesTypeDef = TypedDict(
+    "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
-class FillMissingValuesOutputTypeDef(
-    _RequiredFillMissingValuesOutputTypeDef, _OptionalFillMissingValuesOutputTypeDef
+class FillMissingValuesTypeDef(
+    _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
-MergeOutputTypeDef = TypedDict(
-    "MergeOutputTypeDef",
+MergeTypeDef = TypedDict(
+    "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
     },
 )
@@ -1650,16 +1492,16 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-MicrosoftSQLServerCatalogTargetOutputTypeDef = TypedDict(
-    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1669,16 +1511,16 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-MySQLCatalogTargetOutputTypeDef = TypedDict(
-    "MySQLCatalogTargetOutputTypeDef",
+MySQLCatalogTargetTypeDef = TypedDict(
+    "MySQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1688,60 +1530,58 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-OracleSQLCatalogTargetOutputTypeDef = TypedDict(
-    "OracleSQLCatalogTargetOutputTypeDef",
+OracleSQLCatalogTargetTypeDef = TypedDict(
+    "OracleSQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 
-_RequiredPIIDetectionOutputTypeDef = TypedDict(
-    "_RequiredPIIDetectionOutputTypeDef",
+_RequiredPIIDetectionTypeDef = TypedDict(
+    "_RequiredPIIDetectionTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "PiiType": PiiTypeType,
         "EntityTypesToDetect": List[str],
     },
 )
-_OptionalPIIDetectionOutputTypeDef = TypedDict(
-    "_OptionalPIIDetectionOutputTypeDef",
+_OptionalPIIDetectionTypeDef = TypedDict(
+    "_OptionalPIIDetectionTypeDef",
     {
         "OutputColumnName": str,
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
-class PIIDetectionOutputTypeDef(
-    _RequiredPIIDetectionOutputTypeDef, _OptionalPIIDetectionOutputTypeDef
-):
+class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-PostgreSQLCatalogTargetOutputTypeDef = TypedDict(
-    "PostgreSQLCatalogTargetOutputTypeDef",
+PostgreSQLCatalogTargetTypeDef = TypedDict(
+    "PostgreSQLCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
@@ -1771,234 +1611,47 @@
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
-RenameFieldOutputTypeDef = TypedDict(
-    "RenameFieldOutputTypeDef",
+RenameFieldTypeDef = TypedDict(
+    "RenameFieldTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SourcePath": List[str],
         "TargetPath": List[str],
     },
 )
 
-SelectFieldsOutputTypeDef = TypedDict(
-    "SelectFieldsOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
-    },
-)
-
-SelectFromCollectionOutputTypeDef = TypedDict(
-    "SelectFromCollectionOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Index": int,
-    },
-)
-
-_RequiredSpigotOutputTypeDef = TypedDict(
-    "_RequiredSpigotOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-    },
-)
-_OptionalSpigotOutputTypeDef = TypedDict(
-    "_OptionalSpigotOutputTypeDef",
-    {
-        "Topk": int,
-        "Prob": float,
-    },
-    total=False,
-)
-
-class SpigotOutputTypeDef(_RequiredSpigotOutputTypeDef, _OptionalSpigotOutputTypeDef):
-    pass
-
-SplitFieldsOutputTypeDef = TypedDict(
-    "SplitFieldsOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
-    },
-)
-
-UnionOutputTypeDef = TypedDict(
-    "UnionOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "UnionType": UnionTypeType,
-    },
-)
-
-_RequiredDropDuplicatesTypeDef = TypedDict(
-    "_RequiredDropDuplicatesTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-    },
-)
-_OptionalDropDuplicatesTypeDef = TypedDict(
-    "_OptionalDropDuplicatesTypeDef",
-    {
-        "Columns": Sequence[Sequence[str]],
-    },
-    total=False,
-)
-
-class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
-    pass
-
-DropFieldsTypeDef = TypedDict(
-    "DropFieldsTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
-    },
-)
-
-_RequiredFillMissingValuesTypeDef = TypedDict(
-    "_RequiredFillMissingValuesTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "ImputedPath": str,
-    },
-)
-_OptionalFillMissingValuesTypeDef = TypedDict(
-    "_OptionalFillMissingValuesTypeDef",
-    {
-        "FilledPath": str,
-    },
-    total=False,
-)
-
-class FillMissingValuesTypeDef(
-    _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
-):
-    pass
-
-MergeTypeDef = TypedDict(
-    "MergeTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Source": str,
-        "PrimaryKeys": Sequence[Sequence[str]],
-    },
-)
-
-MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
-    "MicrosoftSQLServerCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-MySQLCatalogTargetTypeDef = TypedDict(
-    "MySQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-OracleSQLCatalogTargetTypeDef = TypedDict(
-    "OracleSQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-_RequiredPIIDetectionTypeDef = TypedDict(
-    "_RequiredPIIDetectionTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "PiiType": PiiTypeType,
-        "EntityTypesToDetect": Sequence[str],
-    },
-)
-_OptionalPIIDetectionTypeDef = TypedDict(
-    "_OptionalPIIDetectionTypeDef",
-    {
-        "OutputColumnName": str,
-        "SampleFraction": float,
-        "ThresholdFraction": float,
-        "MaskValue": str,
-    },
-    total=False,
-)
-
-class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
-    pass
-
-PostgreSQLCatalogTargetTypeDef = TypedDict(
-    "PostgreSQLCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-
-RenameFieldTypeDef = TypedDict(
-    "RenameFieldTypeDef",
-    {
-        "Name": str,
-        "Inputs": Sequence[str],
-        "SourcePath": Sequence[str],
-        "TargetPath": Sequence[str],
-    },
-)
-
 SelectFieldsTypeDef = TypedDict(
     "SelectFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
+        "Inputs": List[str],
+        "Paths": List[List[str]],
     },
 )
 
 SelectFromCollectionTypeDef = TypedDict(
     "SelectFromCollectionTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Index": int,
     },
 )
 
 _RequiredSpigotTypeDef = TypedDict(
     "_RequiredSpigotTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
     },
 )
 _OptionalSpigotTypeDef = TypedDict(
     "_OptionalSpigotTypeDef",
     {
         "Topk": int,
@@ -2010,24 +1663,24 @@
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Paths": Sequence[Sequence[str]],
+        "Inputs": List[str],
+        "Paths": List[List[str]],
     },
 )
 
 UnionTypeDef = TypedDict(
     "UnionTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "UnionType": UnionTypeType,
     },
 )
 
 _RequiredCodeGenEdgeTypeDef = TypedDict(
     "_RequiredCodeGenEdgeTypeDef",
     {
@@ -2069,60 +1722,41 @@
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
 )
 
-_RequiredColumnOutputTypeDef = TypedDict(
-    "_RequiredColumnOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalColumnOutputTypeDef = TypedDict(
-    "_OptionalColumnOutputTypeDef",
-    {
-        "Type": str,
-        "Comment": str,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class ColumnOutputTypeDef(_RequiredColumnOutputTypeDef, _OptionalColumnOutputTypeDef):
-    pass
-
 ColumnRowFilterTypeDef = TypedDict(
     "ColumnRowFilterTypeDef",
     {
         "ColumnName": str,
         "RowFilterExpression": str,
     },
     total=False,
 )
 
-_RequiredDateColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredDateColumnStatisticsDataOutputTypeDef",
+_RequiredDateColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredDateColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
-_OptionalDateColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalDateColumnStatisticsDataOutputTypeDef",
+_OptionalDateColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalDateColumnStatisticsDataTypeDef",
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
-class DateColumnStatisticsDataOutputTypeDef(
-    _RequiredDateColumnStatisticsDataOutputTypeDef, _OptionalDateColumnStatisticsDataOutputTypeDef
+class DateColumnStatisticsDataTypeDef(
+    _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
@@ -2170,15 +1804,14 @@
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 _RequiredColumnTypeDef = TypedDict(
     "_RequiredColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalColumnTypeDef = TypedDict(
@@ -2242,36 +1875,18 @@
 )
 
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
-PhysicalConnectionRequirementsOutputTypeDef = TypedDict(
-    "PhysicalConnectionRequirementsOutputTypeDef",
-    {
-        "SubnetId": str,
-        "SecurityGroupIdList": List[str],
-        "AvailabilityZone": str,
-    },
-    total=False,
-)
-
-ConnectionsListOutputTypeDef = TypedDict(
-    "ConnectionsListOutputTypeDef",
-    {
-        "Connections": List[str],
-    },
-    total=False,
-)
-
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
-        "Connections": Sequence[str],
+        "Connections": List[str],
     },
     total=False,
 )
 
 CrawlTypeDef = TypedDict(
     "CrawlTypeDef",
     {
@@ -2313,16 +1928,16 @@
         "TablesCreated": int,
         "TablesUpdated": int,
         "TablesDeleted": int,
     },
     total=False,
 )
 
-DeltaTargetOutputTypeDef = TypedDict(
-    "DeltaTargetOutputTypeDef",
+DeltaTargetTypeDef = TypedDict(
+    "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
         "CreateNativeDeltaTable": bool,
     },
     total=False,
@@ -2334,16 +1949,16 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
-JdbcTargetOutputTypeDef = TypedDict(
-    "JdbcTargetOutputTypeDef",
+JdbcTargetTypeDef = TypedDict(
+    "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
         "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
@@ -2355,54 +1970,19 @@
         "ConnectionName": str,
         "Path": str,
         "ScanAll": bool,
     },
     total=False,
 )
 
-S3TargetOutputTypeDef = TypedDict(
-    "S3TargetOutputTypeDef",
-    {
-        "Path": str,
-        "Exclusions": List[str],
-        "ConnectionName": str,
-        "SampleSize": int,
-        "EventQueueArn": str,
-        "DlqEventQueueArn": str,
-    },
-    total=False,
-)
-
-DeltaTargetTypeDef = TypedDict(
-    "DeltaTargetTypeDef",
-    {
-        "DeltaTables": Sequence[str],
-        "ConnectionName": str,
-        "WriteManifest": bool,
-        "CreateNativeDeltaTable": bool,
-    },
-    total=False,
-)
-
-JdbcTargetTypeDef = TypedDict(
-    "JdbcTargetTypeDef",
-    {
-        "ConnectionName": str,
-        "Path": str,
-        "Exclusions": Sequence[str],
-        "EnableAdditionalMetadata": Sequence[JdbcMetadataEntryType],
-    },
-    total=False,
-)
-
 S3TargetTypeDef = TypedDict(
     "S3TargetTypeDef",
     {
         "Path": str,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "ConnectionName": str,
         "SampleSize": int,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
@@ -2673,14 +2253,34 @@
         "LastCommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+_RequiredGlueTableTypeDef = TypedDict(
+    "_RequiredGlueTableTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGlueTableTypeDef = TypedDict(
+    "_OptionalGlueTableTypeDef",
+    {
+        "CatalogId": str,
+        "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+    total=False,
+)
+
+class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
+    pass
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2813,66 +2413,27 @@
     {
         "CloudWatchMetricsEnabled": bool,
         "ResultsS3Prefix": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DataQualityRuleResultTypeDef = TypedDict(
     "DataQualityRuleResultTypeDef",
     {
         "Name": str,
         "Description": str,
         "EvaluationMessage": str,
         "Result": DataQualityRuleResultStatusType,
         "EvaluatedMetrics": Dict[str, float],
     },
     total=False,
 )
 
-_RequiredGlueTableOutputTypeDef = TypedDict(
-    "_RequiredGlueTableOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGlueTableOutputTypeDef = TypedDict(
-    "_OptionalGlueTableOutputTypeDef",
-    {
-        "CatalogId": str,
-        "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-    total=False,
-)
-
-class GlueTableOutputTypeDef(_RequiredGlueTableOutputTypeDef, _OptionalGlueTableOutputTypeDef):
-    pass
-
-_RequiredGlueTableTypeDef = TypedDict(
-    "_RequiredGlueTableTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGlueTableTypeDef = TypedDict(
-    "_OptionalGlueTableTypeDef",
-    {
-        "CatalogId": str,
-        "ConnectionName": str,
-        "AdditionalOptions": Mapping[str, str],
-    },
-    total=False,
-)
-
-class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
-    pass
-
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Region": str,
     },
@@ -2892,16 +2453,16 @@
     "DatatypeTypeDef",
     {
         "Id": str,
         "Label": str,
     },
 )
 
-DecimalNumberOutputTypeDef = TypedDict(
-    "DecimalNumberOutputTypeDef",
+DecimalNumberTypeDef = TypedDict(
+    "DecimalNumberTypeDef",
     {
         "UnscaledValue": bytes,
         "Scale": int,
     },
 )
 
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
@@ -3235,51 +2796,27 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
-_RequiredTransformConfigParameterOutputTypeDef = TypedDict(
-    "_RequiredTransformConfigParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParamTypeType,
-    },
-)
-_OptionalTransformConfigParameterOutputTypeDef = TypedDict(
-    "_OptionalTransformConfigParameterOutputTypeDef",
-    {
-        "ValidationRule": str,
-        "ValidationMessage": str,
-        "Value": List[str],
-        "ListType": ParamTypeType,
-        "IsOptional": bool,
-    },
-    total=False,
-)
-
-class TransformConfigParameterOutputTypeDef(
-    _RequiredTransformConfigParameterOutputTypeDef, _OptionalTransformConfigParameterOutputTypeDef
-):
-    pass
-
 _RequiredTransformConfigParameterTypeDef = TypedDict(
     "_RequiredTransformConfigParameterTypeDef",
     {
         "Name": str,
         "Type": ParamTypeType,
     },
 )
 _OptionalTransformConfigParameterTypeDef = TypedDict(
     "_OptionalTransformConfigParameterTypeDef",
     {
         "ValidationRule": str,
         "ValidationMessage": str,
-        "Value": Sequence[str],
+        "Value": List[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
 class TransformConfigParameterTypeDef(
@@ -3337,27 +2874,19 @@
         "Identifier": str,
         "DatabaseIdentifier": str,
         "ConnectionName": str,
     },
     total=False,
 )
 
-FilterValueOutputTypeDef = TypedDict(
-    "FilterValueOutputTypeDef",
-    {
-        "Type": FilterValueTypeType,
-        "Value": List[str],
-    },
-)
-
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
-        "Value": Sequence[str],
+        "Value": List[str],
     },
 )
 
 FindMatchesParametersTypeDef = TypedDict(
     "FindMatchesParametersTypeDef",
     {
         "PrimaryKeyColumnName": str,
@@ -4162,66 +3691,43 @@
     {
         "InputS3Path": str,
         "Replace": bool,
     },
     total=False,
 )
 
-JDBCConnectorOptionsOutputTypeDef = TypedDict(
-    "JDBCConnectorOptionsOutputTypeDef",
-    {
-        "FilterPredicate": str,
-        "PartitionColumn": str,
-        "LowerBound": int,
-        "UpperBound": int,
-        "NumPartitions": int,
-        "JobBookmarkKeys": List[str],
-        "JobBookmarkKeysSortOrder": str,
-        "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
-    },
-    total=False,
-)
-
 JDBCConnectorOptionsTypeDef = TypedDict(
     "JDBCConnectorOptionsTypeDef",
     {
         "FilterPredicate": str,
         "PartitionColumn": str,
         "LowerBound": int,
         "UpperBound": int,
         "NumPartitions": int,
-        "JobBookmarkKeys": Sequence[str],
+        "JobBookmarkKeys": List[str],
         "JobBookmarkKeysSortOrder": str,
-        "DataTypeMapping": Mapping[JDBCDataTypeType, GlueRecordTypeType],
+        "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
     },
     total=False,
 )
 
 PredecessorTypeDef = TypedDict(
     "PredecessorTypeDef",
     {
         "JobName": str,
         "RunId": str,
     },
     total=False,
 )
 
-JoinColumnOutputTypeDef = TypedDict(
-    "JoinColumnOutputTypeDef",
-    {
-        "From": str,
-        "Keys": List[List[str]],
-    },
-)
-
 JoinColumnTypeDef = TypedDict(
     "JoinColumnTypeDef",
     {
         "From": str,
-        "Keys": Sequence[Sequence[str]],
+        "Keys": List[List[str]],
     },
 )
 
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "Name": str,
@@ -4401,36 +3907,23 @@
 )
 
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
-MappingOutputTypeDef = TypedDict(
-    "MappingOutputTypeDef",
-    {
-        "ToKey": str,
-        "FromPath": List[str],
-        "FromType": str,
-        "ToType": str,
-        "Dropped": bool,
-        "Children": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
-        "FromPath": Sequence[str],
+        "FromPath": List[str],
         "FromType": str,
         "ToType": str,
         "Dropped": bool,
-        "Children": Sequence[Dict[str, Any]],
+        "Children": List[Dict[str, Any]],
     },
     total=False,
 )
 
 OtherMetadataValueListItemTypeDef = TypedDict(
     "OtherMetadataValueListItemTypeDef",
     {
@@ -4453,21 +3946,14 @@
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
     },
 )
 
-PartitionValueListTypeDef = TypedDict(
-    "PartitionValueListTypeDef",
-    {
-        "Values": Sequence[str],
-    },
-)
-
 PropertyPredicateTypeDef = TypedDict(
     "PropertyPredicateTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparator": ComparatorType,
     },
@@ -4501,30 +3987,20 @@
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
-UpsertRedshiftTargetOptionsOutputTypeDef = TypedDict(
-    "UpsertRedshiftTargetOptionsOutputTypeDef",
-    {
-        "TableLocation": str,
-        "ConnectionName": str,
-        "UpsertKeys": List[str],
-    },
-    total=False,
-)
-
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
-        "UpsertKeys": Sequence[str],
+        "UpsertKeys": List[str],
     },
     total=False,
 )
 
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
@@ -4598,44 +4074,24 @@
     {
         "FieldName": str,
         "Sort": SortType,
     },
     total=False,
 )
 
-SerDeInfoOutputTypeDef = TypedDict(
-    "SerDeInfoOutputTypeDef",
-    {
-        "Name": str,
-        "SerializationLibrary": str,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
 SerDeInfoTypeDef = TypedDict(
     "SerDeInfoTypeDef",
     {
         "Name": str,
         "SerializationLibrary": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-SkewedInfoOutputTypeDef = TypedDict(
-    "SkewedInfoOutputTypeDef",
-    {
-        "SkewedColumnNames": List[str],
-        "SkewedColumnValues": List[str],
-        "SkewedColumnValueLocationMaps": Dict[str, str],
-    },
-    total=False,
-)
-
 SkewedInfoTypeDef = TypedDict(
     "SkewedInfoTypeDef",
     {
         "SkewedColumnNames": Sequence[str],
         "SkewedColumnValues": Sequence[str],
         "SkewedColumnValueLocationMaps": Mapping[str, str],
     },
@@ -5057,32 +4513,19 @@
         "RunningActions": int,
         "ErroredActions": int,
         "WaitingActions": int,
     },
     total=False,
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "JobName": str,
-        "Arguments": Dict[str, str],
-        "Timeout": int,
-        "SecurityConfiguration": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "CrawlerName": str,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "JobName": str,
-        "Arguments": Mapping[str, str],
+        "Arguments": Dict[str, str],
         "Timeout": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "CrawlerName": str,
     },
     total=False,
 )
@@ -5111,36 +4554,26 @@
 )
 
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-AggregateOutputTypeDef = TypedDict(
-    "AggregateOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Groups": List[List[str]],
-        "Aggs": List[AggregateOperationOutputTypeDef],
-    },
-)
-
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
-        "Groups": Sequence[Sequence[str]],
-        "Aggs": Sequence[AggregateOperationTypeDef],
+        "Inputs": List[str],
+        "Groups": List[List[str]],
+        "Aggs": List[AggregateOperationTypeDef],
     },
 )
 
-AmazonRedshiftNodeDataOutputTypeDef = TypedDict(
-    "AmazonRedshiftNodeDataOutputTypeDef",
+AmazonRedshiftNodeDataTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataTypeDef",
     {
         "AccessType": str,
         "SourceType": str,
         "Connection": OptionTypeDef,
         "Schema": OptionTypeDef,
         "Table": OptionTypeDef,
         "CatalogDatabase": OptionTypeDef,
@@ -5164,47 +4597,14 @@
         "TableSchema": List[OptionTypeDef],
         "StagingTable": str,
         "SelectedColumns": List[OptionTypeDef],
     },
     total=False,
 )
 
-AmazonRedshiftNodeDataTypeDef = TypedDict(
-    "AmazonRedshiftNodeDataTypeDef",
-    {
-        "AccessType": str,
-        "SourceType": str,
-        "Connection": OptionTypeDef,
-        "Schema": OptionTypeDef,
-        "Table": OptionTypeDef,
-        "CatalogDatabase": OptionTypeDef,
-        "CatalogTable": OptionTypeDef,
-        "CatalogRedshiftSchema": str,
-        "CatalogRedshiftTable": str,
-        "TempDir": str,
-        "IamRole": OptionTypeDef,
-        "AdvancedOptions": Sequence[AmazonRedshiftAdvancedOptionTypeDef],
-        "SampleQuery": str,
-        "PreAction": str,
-        "PostAction": str,
-        "Action": str,
-        "TablePrefix": str,
-        "Upsert": bool,
-        "MergeAction": str,
-        "MergeWhenMatched": str,
-        "MergeWhenNotMatched": str,
-        "MergeClause": str,
-        "CrawlerConnection": str,
-        "TableSchema": Sequence[OptionTypeDef],
-        "StagingTable": str,
-        "SelectedColumns": Sequence[OptionTypeDef],
-    },
-    total=False,
-)
-
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -5248,19 +4648,62 @@
 ):
     pass
 
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
-        "Partitions": List[PartitionValueListOutputTypeDef],
+        "Partitions": List[PartitionValueListTypeDef],
     },
     total=False,
 )
 
+_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchDeletePartitionRequestRequestTypeDef(
+    _RequiredBatchDeletePartitionRequestRequestTypeDef,
+    _OptionalBatchDeletePartitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetPartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetPartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchGetPartitionRequestRequestTypeDef(
+    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
+):
+    pass
+
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6003,22 +5446,14 @@
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DecimalNumberTypeDef = TypedDict(
-    "DecimalNumberTypeDef",
-    {
-        "UnscaledValue": BlobTypeDef,
-        "Scale": int,
-    },
-)
-
 GetBlueprintRunResponseTypeDef = TypedDict(
     "GetBlueprintRunResponseTypeDef",
     {
         "BlueprintRun": BlueprintRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6053,282 +5488,188 @@
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCatalogKafkaSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogKafkaSourceOutputTypeDef",
+_RequiredCatalogKafkaSourceTypeDef = TypedDict(
+    "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
 )
-_OptionalCatalogKafkaSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogKafkaSourceOutputTypeDef",
+_OptionalCatalogKafkaSourceTypeDef = TypedDict(
+    "_OptionalCatalogKafkaSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-class CatalogKafkaSourceOutputTypeDef(
-    _RequiredCatalogKafkaSourceOutputTypeDef, _OptionalCatalogKafkaSourceOutputTypeDef
+class CatalogKafkaSourceTypeDef(
+    _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
-_RequiredDirectKafkaSourceOutputTypeDef = TypedDict(
-    "_RequiredDirectKafkaSourceOutputTypeDef",
+_RequiredDirectKafkaSourceTypeDef = TypedDict(
+    "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalDirectKafkaSourceOutputTypeDef = TypedDict(
-    "_OptionalDirectKafkaSourceOutputTypeDef",
+_OptionalDirectKafkaSourceTypeDef = TypedDict(
+    "_OptionalDirectKafkaSourceTypeDef",
     {
-        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-class DirectKafkaSourceOutputTypeDef(
-    _RequiredDirectKafkaSourceOutputTypeDef, _OptionalDirectKafkaSourceOutputTypeDef
+class DirectKafkaSourceTypeDef(
+    _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
-_RequiredCatalogKinesisSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogKinesisSourceOutputTypeDef",
+_RequiredCatalogKinesisSourceTypeDef = TypedDict(
+    "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
 )
-_OptionalCatalogKinesisSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogKinesisSourceOutputTypeDef",
+_OptionalCatalogKinesisSourceTypeDef = TypedDict(
+    "_OptionalCatalogKinesisSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-class CatalogKinesisSourceOutputTypeDef(
-    _RequiredCatalogKinesisSourceOutputTypeDef, _OptionalCatalogKinesisSourceOutputTypeDef
+class CatalogKinesisSourceTypeDef(
+    _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
-_RequiredDirectKinesisSourceOutputTypeDef = TypedDict(
-    "_RequiredDirectKinesisSourceOutputTypeDef",
+_RequiredDirectKinesisSourceTypeDef = TypedDict(
+    "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalDirectKinesisSourceOutputTypeDef = TypedDict(
-    "_OptionalDirectKinesisSourceOutputTypeDef",
+_OptionalDirectKinesisSourceTypeDef = TypedDict(
+    "_OptionalDirectKinesisSourceTypeDef",
     {
         "WindowSize": int,
         "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-class DirectKinesisSourceOutputTypeDef(
-    _RequiredDirectKinesisSourceOutputTypeDef, _OptionalDirectKinesisSourceOutputTypeDef
-):
-    pass
-
-_RequiredGovernedCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredGovernedCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalGovernedCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalGovernedCatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class GovernedCatalogTargetOutputTypeDef(
-    _RequiredGovernedCatalogTargetOutputTypeDef, _OptionalGovernedCatalogTargetOutputTypeDef
+class DirectKinesisSourceTypeDef(
+    _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalGovernedCatalogTargetTypeDef = TypedDict(
     "_OptionalGovernedCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
-_RequiredS3CatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3CatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3CatalogTargetOutputTypeDef(
-    _RequiredS3CatalogTargetOutputTypeDef, _OptionalS3CatalogTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3CatalogTargetTypeDef = TypedDict(
     "_OptionalS3CatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
-    pass
-
-_RequiredS3DeltaCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3DeltaCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaCatalogTargetOutputTypeDef",
-    {
         "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-class S3DeltaCatalogTargetOutputTypeDef(
-    _RequiredS3DeltaCatalogTargetOutputTypeDef, _OptionalS3DeltaCatalogTargetOutputTypeDef
-):
+class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
     "_OptionalS3DeltaCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "AdditionalOptions": Mapping[str, str],
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
-_RequiredS3HudiCatalogTargetOutputTypeDef = TypedDict(
-    "_RequiredS3HudiCatalogTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiCatalogTargetOutputTypeDef = TypedDict(
-    "_OptionalS3HudiCatalogTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3HudiCatalogTargetOutputTypeDef(
-    _RequiredS3HudiCatalogTargetOutputTypeDef, _OptionalS3HudiCatalogTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Table": str,
         "Database": str,
-        "AdditionalOptions": Mapping[str, str],
+        "AdditionalOptions": Dict[str, str],
     },
 )
 _OptionalS3HudiCatalogTargetTypeDef = TypedDict(
     "_OptionalS3HudiCatalogTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3HudiCatalogTargetTypeDef(
     _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
@@ -6342,35 +5683,14 @@
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
     },
     total=False,
 )
 
-_RequiredCodeGenNodeOutputTypeDef = TypedDict(
-    "_RequiredCodeGenNodeOutputTypeDef",
-    {
-        "Id": str,
-        "NodeType": str,
-        "Args": List[CodeGenNodeArgTypeDef],
-    },
-)
-_OptionalCodeGenNodeOutputTypeDef = TypedDict(
-    "_OptionalCodeGenNodeOutputTypeDef",
-    {
-        "LineNumber": int,
-    },
-    total=False,
-)
-
-class CodeGenNodeOutputTypeDef(
-    _RequiredCodeGenNodeOutputTypeDef, _OptionalCodeGenNodeOutputTypeDef
-):
-    pass
-
 _RequiredCodeGenNodeTypeDef = TypedDict(
     "_RequiredCodeGenNodeTypeDef",
     {
         "Id": str,
         "NodeType": str,
         "Args": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -6392,160 +5712,19 @@
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
     total=False,
 )
 
-_RequiredDateColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredDateColumnStatisticsDataTypeDef",
-    {
-        "NumberOfNulls": int,
-        "NumberOfDistinctValues": int,
-    },
-)
-_OptionalDateColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalDateColumnStatisticsDataTypeDef",
-    {
-        "MinimumValue": TimestampTypeDef,
-        "MaximumValue": TimestampTypeDef,
-    },
-    total=False,
-)
-
-class DateColumnStatisticsDataTypeDef(
-    _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
-):
-    pass
-
-_RequiredGetTableRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "Name": str,
-    },
-)
-_OptionalGetTableRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-class GetTableRequestRequestTypeDef(
-    _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
-):
-    pass
-
-_RequiredGetTablesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTablesRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalGetTablesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTablesRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "Expression": str,
-        "NextToken": str,
-        "MaxResults": int,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-class GetTablesRequestRequestTypeDef(
-    _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
-):
-    pass
-
-KafkaStreamingSourceOptionsTypeDef = TypedDict(
-    "KafkaStreamingSourceOptionsTypeDef",
-    {
-        "BootstrapServers": str,
-        "SecurityProtocol": str,
-        "ConnectionName": str,
-        "TopicName": str,
-        "Assign": str,
-        "SubscribePattern": str,
-        "Classification": str,
-        "Delimiter": str,
-        "StartingOffsets": str,
-        "EndingOffsets": str,
-        "PollTimeoutMs": int,
-        "NumRetries": int,
-        "RetryIntervalMs": int,
-        "MaxOffsetsPerTrigger": int,
-        "MinPartitions": int,
-        "IncludeHeaders": bool,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": TimestampTypeDef,
-    },
-    total=False,
-)
-
-KinesisStreamingSourceOptionsTypeDef = TypedDict(
-    "KinesisStreamingSourceOptionsTypeDef",
-    {
-        "EndpointUrl": str,
-        "StreamName": str,
-        "Classification": str,
-        "Delimiter": str,
-        "StartingPosition": StartingPositionType,
-        "MaxFetchTimeInMs": int,
-        "MaxFetchRecordsPerShard": int,
-        "MaxRecordPerRead": int,
-        "AddIdleTimeBetweenReads": bool,
-        "IdleTimeBetweenReadsInMs": int,
-        "DescribeShardInterval": int,
-        "NumRetries": int,
-        "RetryIntervalMs": int,
-        "MaxRetryIntervalMs": int,
-        "AvoidEmptyBatches": bool,
-        "StreamArn": str,
-        "RoleArn": str,
-        "RoleSessionName": str,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": TimestampTypeDef,
-    },
-    total=False,
-)
-
-TaskRunFilterCriteriaTypeDef = TypedDict(
-    "TaskRunFilterCriteriaTypeDef",
-    {
-        "TaskRunType": TaskTypeType,
-        "Status": TaskStatusTypeType,
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
-    },
-    total=False,
-)
-
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "Logical": LogicalType,
-        "Conditions": List[ConditionTypeDef],
-    },
-    total=False,
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Logical": LogicalType,
-        "Conditions": Sequence[ConditionTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
     total=False,
 )
 
 FindMatchesMetricsTypeDef = TypedDict(
     "FindMatchesMetricsTypeDef",
     {
@@ -6584,23 +5763,22 @@
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
         "ConnectionProperties": Dict[ConnectionPropertyKeyType, str],
-        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsOutputTypeDef,
+        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
     total=False,
 )
 
-ConnectionsListUnionTypeDef = Union[ConnectionsListTypeDef, ConnectionsListOutputTypeDef]
 CrawlerNodeDetailsTypeDef = TypedDict(
     "CrawlerNodeDetailsTypeDef",
     {
         "Crawls": List[CrawlTypeDef],
     },
     total=False,
 )
@@ -6619,36 +5797,23 @@
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CrawlerTargetsOutputTypeDef = TypedDict(
-    "CrawlerTargetsOutputTypeDef",
-    {
-        "S3Targets": List[S3TargetOutputTypeDef],
-        "JdbcTargets": List[JdbcTargetOutputTypeDef],
-        "MongoDBTargets": List[MongoDBTargetTypeDef],
-        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
-        "CatalogTargets": List[CatalogTargetOutputTypeDef],
-        "DeltaTargets": List[DeltaTargetOutputTypeDef],
-    },
-    total=False,
-)
-
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
-        "S3Targets": Sequence[S3TargetTypeDef],
-        "JdbcTargets": Sequence[JdbcTargetTypeDef],
-        "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
-        "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
-        "CatalogTargets": Sequence[CatalogTargetTypeDef],
-        "DeltaTargets": Sequence[DeltaTargetTypeDef],
+        "S3Targets": List[S3TargetTypeDef],
+        "JdbcTargets": List[JdbcTargetTypeDef],
+        "MongoDBTargets": List[MongoDBTargetTypeDef],
+        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
+        "CatalogTargets": List[CatalogTargetTypeDef],
+        "DeltaTargets": List[DeltaTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -6701,28 +5866,14 @@
 
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
-DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedBefore": TimestampTypeDef,
-        "CreatedAfter": TimestampTypeDef,
-        "LastModifiedBefore": TimestampTypeDef,
-        "LastModifiedAfter": TimestampTypeDef,
-        "TargetTable": DataQualityTargetTableTypeDef,
-    },
-    total=False,
-)
-
 DataQualityRulesetListDetailsTypeDef = TypedDict(
     "DataQualityRulesetListDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
@@ -6743,14 +5894,21 @@
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "RecommendationRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "GlueTable": GlueTableTypeDef,
+    },
+)
+
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -6864,100 +6022,52 @@
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
         "Description": str,
         "Role": str,
         "Command": SessionCommandTypeDef,
         "DefaultArguments": Dict[str, str],
-        "Connections": ConnectionsListOutputTypeDef,
+        "Connections": ConnectionsListTypeDef,
         "Progress": float,
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
-_RequiredEvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityMultiFrameOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityMultiFrameOutputTypeDef",
-    {
-        "AdditionalDataSources": Dict[str, str],
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-class EvaluateDataQualityMultiFrameOutputTypeDef(
-    _RequiredEvaluateDataQualityMultiFrameOutputTypeDef,
-    _OptionalEvaluateDataQualityMultiFrameOutputTypeDef,
-):
-    pass
-
 _RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityMultiFrameTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityMultiFrameTypeDef",
     {
-        "AdditionalDataSources": Mapping[str, str],
+        "AdditionalDataSources": Dict[str, str],
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Mapping[Literal["performanceTuning.caching"], str],
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
-_RequiredEvaluateDataQualityOutputTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityOutputTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityOutputTypeDef",
-    {
-        "Output": DQTransformOutputType,
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-class EvaluateDataQualityOutputTypeDef(
-    _RequiredEvaluateDataQualityOutputTypeDef, _OptionalEvaluateDataQualityOutputTypeDef
-):
-    pass
-
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityTypeDef",
     {
         "Output": DQTransformOutputType,
@@ -6977,74 +6087,120 @@
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
 )
 
-PrincipalPermissionsOutputTypeDef = TypedDict(
-    "PrincipalPermissionsOutputTypeDef",
+PrincipalPermissionsTypeDef = TypedDict(
+    "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
-PrincipalPermissionsTypeDef = TypedDict(
-    "PrincipalPermissionsTypeDef",
+DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
+    "DataQualityRulesetFilterCriteriaTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": Sequence[PermissionType],
+        "Name": str,
+        "Description": str,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+        "LastModifiedBefore": TimestampTypeDef,
+        "LastModifiedAfter": TimestampTypeDef,
+        "TargetTable": DataQualityTargetTableTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTableRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "Name": str,
+    },
+)
+_OptionalGetTableRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+class GetTableRequestRequestTypeDef(
+    _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetTablesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTablesRequestRequestTypeDef",
     {
-        "GlueTable": GlueTableOutputTypeDef,
+        "DatabaseName": str,
+    },
+)
+_OptionalGetTablesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTablesRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "Expression": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
     },
+    total=False,
 )
 
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
+class GetTablesRequestRequestTypeDef(
+    _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
+):
+    pass
+
+TaskRunFilterCriteriaTypeDef = TypedDict(
+    "TaskRunFilterCriteriaTypeDef",
     {
-        "GlueTable": GlueTableTypeDef,
+        "TaskRunType": TaskTypeType,
+        "Status": TaskStatusTypeType,
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-GlueTableUnionTypeDef = Union[GlueTableTypeDef, GlueTableOutputTypeDef]
 NullValueFieldTypeDef = TypedDict(
     "NullValueFieldTypeDef",
     {
         "Value": str,
         "Datatype": DatatypeTypeDef,
     },
 )
 
-_RequiredDecimalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredDecimalColumnStatisticsDataOutputTypeDef",
+_RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredDecimalColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
-_OptionalDecimalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalDecimalColumnStatisticsDataOutputTypeDef",
+_OptionalDecimalColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalDecimalColumnStatisticsDataTypeDef",
     {
-        "MinimumValue": DecimalNumberOutputTypeDef,
-        "MaximumValue": DecimalNumberOutputTypeDef,
+        "MinimumValue": DecimalNumberTypeDef,
+        "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
-class DecimalColumnStatisticsDataOutputTypeDef(
-    _RequiredDecimalColumnStatisticsDataOutputTypeDef,
-    _OptionalDecimalColumnStatisticsDataOutputTypeDef,
+class DecimalColumnStatisticsDataTypeDef(
+    _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
@@ -7133,216 +6289,109 @@
 )
 
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-_RequiredS3DeltaDirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaDirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": DeltaTargetCompressionTypeType,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DeltaDirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaDirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3DeltaDirectTargetOutputTypeDef(
-    _RequiredS3DeltaDirectTargetOutputTypeDef, _OptionalS3DeltaDirectTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DeltaDirectTargetTypeDef = TypedDict(
     "_OptionalS3DeltaDirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
-        "AdditionalOptions": Mapping[str, str],
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
-_RequiredS3DirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3DirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3DirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "Compression": str,
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3DirectTargetOutputTypeDef(
-    _RequiredS3DirectTargetOutputTypeDef, _OptionalS3DirectTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DirectTargetTypeDef = TypedDict(
     "_OptionalS3DirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
-_RequiredS3GlueParquetTargetOutputTypeDef = TypedDict(
-    "_RequiredS3GlueParquetTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-    },
-)
-_OptionalS3GlueParquetTargetOutputTypeDef = TypedDict(
-    "_OptionalS3GlueParquetTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "Compression": ParquetCompressionTypeType,
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3GlueParquetTargetOutputTypeDef(
-    _RequiredS3GlueParquetTargetOutputTypeDef, _OptionalS3GlueParquetTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
     },
 )
 _OptionalS3GlueParquetTargetTypeDef = TypedDict(
     "_OptionalS3GlueParquetTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
-_RequiredS3HudiDirectTargetOutputTypeDef = TypedDict(
-    "_RequiredS3HudiDirectTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": HudiTargetCompressionTypeType,
-        "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiDirectTargetOutputTypeDef = TypedDict(
-    "_OptionalS3HudiDirectTargetOutputTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3HudiDirectTargetOutputTypeDef(
-    _RequiredS3HudiDirectTargetOutputTypeDef, _OptionalS3HudiDirectTargetOutputTypeDef
-):
-    pass
-
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
         "Format": TargetFormatType,
-        "AdditionalOptions": Mapping[str, str],
+        "AdditionalOptions": Dict[str, str],
     },
 )
 _OptionalS3HudiDirectTargetTypeDef = TypedDict(
     "_OptionalS3HudiDirectTargetTypeDef",
     {
-        "PartitionKeys": Sequence[Sequence[str]],
+        "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
-EncryptionConfigurationOutputTypeDef = TypedDict(
-    "EncryptionConfigurationOutputTypeDef",
-    {
-        "S3Encryption": List[S3EncryptionTypeDef],
-        "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
-        "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -7354,39 +6403,19 @@
     {
         "VersionNumber": int,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredFilterExpressionOutputTypeDef = TypedDict(
-    "_RequiredFilterExpressionOutputTypeDef",
-    {
-        "Operation": FilterOperationType,
-        "Values": List[FilterValueOutputTypeDef],
-    },
-)
-_OptionalFilterExpressionOutputTypeDef = TypedDict(
-    "_OptionalFilterExpressionOutputTypeDef",
-    {
-        "Negated": bool,
-    },
-    total=False,
-)
-
-class FilterExpressionOutputTypeDef(
-    _RequiredFilterExpressionOutputTypeDef, _OptionalFilterExpressionOutputTypeDef
-):
-    pass
-
 _RequiredFilterExpressionTypeDef = TypedDict(
     "_RequiredFilterExpressionTypeDef",
     {
         "Operation": FilterOperationType,
-        "Values": Sequence[FilterValueTypeDef],
+        "Values": List[FilterValueTypeDef],
     },
 )
 _OptionalFilterExpressionTypeDef = TypedDict(
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
@@ -7828,26 +6857,18 @@
 )
 
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
-GlueSchemaOutputTypeDef = TypedDict(
-    "GlueSchemaOutputTypeDef",
-    {
-        "Columns": List[GlueStudioSchemaColumnTypeDef],
-    },
-    total=False,
-)
-
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
-        "Columns": Sequence[GlueStudioSchemaColumnTypeDef],
+        "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
 
 _RequiredGovernedCatalogSourceTypeDef = TypedDict(
     "_RequiredGovernedCatalogSourceTypeDef",
     {
@@ -7917,31 +6938,21 @@
         "GlueVersion": str,
         "DPUSeconds": float,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
-JoinOutputTypeDef = TypedDict(
-    "JoinOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "JoinType": JoinTypeType,
-        "Columns": List[JoinColumnOutputTypeDef],
-    },
-)
-
 JoinTypeDef = TypedDict(
     "JoinTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "JoinType": JoinTypeType,
-        "Columns": Sequence[JoinColumnTypeDef],
+        "Columns": List[JoinColumnTypeDef],
     },
 )
 
 TaskRunPropertiesTypeDef = TypedDict(
     "TaskRunPropertiesTypeDef",
     {
         "TaskType": TaskTypeType,
@@ -8052,44 +7063,19 @@
 
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
-PartitionValueListUnionTypeDef = Union[PartitionValueListTypeDef, PartitionValueListOutputTypeDef]
-_RequiredRedshiftTargetOutputTypeDef = TypedDict(
-    "_RequiredRedshiftTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalRedshiftTargetOutputTypeDef = TypedDict(
-    "_OptionalRedshiftTargetOutputTypeDef",
-    {
-        "RedshiftTmpDir": str,
-        "TmpDirIAMRole": str,
-        "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class RedshiftTargetOutputTypeDef(
-    _RequiredRedshiftTargetOutputTypeDef, _OptionalRedshiftTargetOutputTypeDef
-):
-    pass
-
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Database": str,
         "Table": str,
     },
 )
 _OptionalRedshiftTargetTypeDef = TypedDict(
     "_OptionalRedshiftTargetTypeDef",
     {
@@ -8164,49 +7150,29 @@
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
-AmazonRedshiftSourceOutputTypeDef = TypedDict(
-    "AmazonRedshiftSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Data": AmazonRedshiftNodeDataOutputTypeDef,
-    },
-    total=False,
-)
-
-AmazonRedshiftTargetOutputTypeDef = TypedDict(
-    "AmazonRedshiftTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Data": AmazonRedshiftNodeDataOutputTypeDef,
-        "Inputs": List[str],
-    },
-    total=False,
-)
-
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
     },
     total=False,
 )
 
 AmazonRedshiftTargetTypeDef = TypedDict(
     "AmazonRedshiftTargetTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
     },
     total=False,
 )
 
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
@@ -8273,35 +7239,14 @@
     "BatchDeleteTableVersionResponseTypeDef",
     {
         "Errors": List[TableVersionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredDecimalColumnStatisticsDataTypeDef",
-    {
-        "NumberOfNulls": int,
-        "NumberOfDistinctValues": int,
-    },
-)
-_OptionalDecimalColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalDecimalColumnStatisticsDataTypeDef",
-    {
-        "MinimumValue": DecimalNumberTypeDef,
-        "MaximumValue": DecimalNumberTypeDef,
-    },
-    total=False,
-)
-
-class DecimalColumnStatisticsDataTypeDef(
-    _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
-):
-    pass
-
 BatchGetBlueprintsResponseTypeDef = TypedDict(
     "BatchGetBlueprintsResponseTypeDef",
     {
         "Blueprints": List[BlueprintTypeDef],
         "MissingBlueprints": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8328,24 +7273,33 @@
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateScriptRequestRequestTypeDef = TypedDict(
+    "CreateScriptRequestRequestTypeDef",
+    {
+        "DagNodes": Sequence[CodeGenNodeTypeDef],
+        "DagEdges": Sequence[CodeGenEdgeTypeDef],
+        "Language": LanguageType,
+    },
+    total=False,
+)
+
 GetDataflowGraphResponseTypeDef = TypedDict(
     "GetDataflowGraphResponseTypeDef",
     {
-        "DagNodes": List[CodeGenNodeOutputTypeDef],
+        "DagNodes": List[CodeGenNodeTypeDef],
         "DagEdges": List[CodeGenEdgeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CodeGenNodeUnionTypeDef = Union[CodeGenNodeTypeDef, CodeGenNodeOutputTypeDef]
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
     },
 )
 _OptionalGetMappingRequestRequestTypeDef = TypedDict(
@@ -8381,146 +7335,58 @@
 )
 
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
-_RequiredCatalogKafkaSourceTypeDef = TypedDict(
-    "_RequiredCatalogKafkaSourceTypeDef",
-    {
-        "Name": str,
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalCatalogKafkaSourceTypeDef = TypedDict(
-    "_OptionalCatalogKafkaSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-class CatalogKafkaSourceTypeDef(
-    _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
-):
-    pass
-
-_RequiredDirectKafkaSourceTypeDef = TypedDict(
-    "_RequiredDirectKafkaSourceTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDirectKafkaSourceTypeDef = TypedDict(
-    "_OptionalDirectKafkaSourceTypeDef",
-    {
-        "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-class DirectKafkaSourceTypeDef(
-    _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
-):
-    pass
-
-_RequiredCatalogKinesisSourceTypeDef = TypedDict(
-    "_RequiredCatalogKinesisSourceTypeDef",
-    {
-        "Name": str,
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalCatalogKinesisSourceTypeDef = TypedDict(
-    "_OptionalCatalogKinesisSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-class CatalogKinesisSourceTypeDef(
-    _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
-):
-    pass
-
-_RequiredDirectKinesisSourceTypeDef = TypedDict(
-    "_RequiredDirectKinesisSourceTypeDef",
+_RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
+        "Type": TriggerTypeType,
+        "Actions": Sequence[ActionTypeDef],
     },
 )
-_OptionalDirectKinesisSourceTypeDef = TypedDict(
-    "_OptionalDirectKinesisSourceTypeDef",
-    {
-        "WindowSize": int,
-        "DetectSchema": bool,
-        "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
-        "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
-    },
-    total=False,
-)
-
-class DirectKinesisSourceTypeDef(
-    _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
-):
-    pass
-
-_RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetMLTaskRunsRequestRequestTypeDef",
-    {
-        "TransformId": str,
-    },
-)
-_OptionalGetMLTaskRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetMLTaskRunsRequestRequestTypeDef",
+_OptionalCreateTriggerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTriggerRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TaskRunFilterCriteriaTypeDef,
-        "Sort": TaskRunSortCriteriaTypeDef,
+        "WorkflowName": str,
+        "Schedule": str,
+        "Predicate": PredicateTypeDef,
+        "Description": str,
+        "StartOnCreation": bool,
+        "Tags": Mapping[str, str],
+        "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-class GetMLTaskRunsRequestRequestTypeDef(
-    _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
+class CreateTriggerRequestRequestTypeDef(
+    _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
         "State": TriggerStateType,
         "Description": str,
         "Schedule": str,
-        "Actions": List[ActionOutputTypeDef],
-        "Predicate": PredicateOutputTypeDef,
+        "Actions": List[ActionTypeDef],
+        "Predicate": PredicateTypeDef,
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-PredicateUnionTypeDef = Union[PredicateTypeDef, PredicateOutputTypeDef]
 TriggerUpdateTypeDef = TypedDict(
     "TriggerUpdateTypeDef",
     {
         "Name": str,
         "Description": str,
         "Schedule": str,
         "Actions": Sequence[ActionTypeDef],
@@ -8607,15 +7473,15 @@
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
         "Role": str,
-        "Targets": CrawlerTargetsOutputTypeDef,
+        "Targets": CrawlerTargetsTypeDef,
         "DatabaseName": str,
         "Description": str,
         "Classifiers": List[str],
         "RecrawlPolicy": RecrawlPolicyTypeDef,
         "SchemaChangePolicy": SchemaChangePolicyTypeDef,
         "LineageConfiguration": LineageConfigurationTypeDef,
         "State": CrawlerStateType,
@@ -8629,15 +7495,14 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
     },
     total=False,
 )
 
-CrawlerTargetsUnionTypeDef = Union[CrawlerTargetsTypeDef, CrawlerTargetsOutputTypeDef]
 _RequiredCreateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
         "Targets": CrawlerTargetsTypeDef,
     },
@@ -8693,152 +7558,53 @@
 )
 
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
-ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 ListDataQualityRulesetsResponseTypeDef = TypedDict(
     "ListDataQualityRulesetsResponseTypeDef",
     {
         "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSessionsResponseTypeDef = TypedDict(
-    "ListSessionsResponseTypeDef",
-    {
-        "Ids": List[str],
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
-    "GetDataCatalogEncryptionSettingsResponseTypeDef",
-    {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-    },
-)
-_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
-    _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredDatabaseTypeDef = TypedDict(
-    "_RequiredDatabaseTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseTypeDef = TypedDict(
-    "_OptionalDatabaseTypeDef",
-    {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Dict[str, str],
-        "CreateTime": datetime,
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "CatalogId": str,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
-    },
-    total=False,
-)
-
-class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
-    pass
-
-_RequiredDatabaseInputTypeDef = TypedDict(
-    "_RequiredDatabaseInputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDatabaseInputTypeDef = TypedDict(
-    "_OptionalDatabaseInputTypeDef",
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
     {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Mapping[str, str],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
+        "ResultId": str,
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
     },
     total=False,
 )
 
-class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
-    pass
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
+DataQualityResultFilterCriteriaTypeDef = TypedDict(
+    "DataQualityResultFilterCriteriaTypeDef",
     {
-        "ResultId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "JobName": str,
         "JobRunId": str,
-        "StartedOn": datetime,
+        "StartedAfter": TimestampTypeDef,
+        "StartedBefore": TimestampTypeDef,
     },
     total=False,
 )
 
 DataQualityResultTypeDef = TypedDict(
     "DataQualityResultTypeDef",
     {
         "ResultId": str,
         "Score": float,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "RulesetName": str,
         "EvaluationContext": str,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "JobName": str,
         "JobRunId": str,
         "RulesetEvaluationRunId": str,
@@ -8849,36 +7615,78 @@
 
 DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
     "DataQualityRuleRecommendationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+class DataQualityRuleRecommendationRunFilterTypeDef(
+    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
+    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+):
+    pass
+
 DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "StartedBefore": TimestampTypeDef,
+        "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+class DataQualityRulesetEvaluationRunFilterTypeDef(
+    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
+    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+):
+    pass
+
 GetDataQualityResultResponseTypeDef = TypedDict(
     "GetDataQualityResultResponseTypeDef",
     {
         "ResultId": str,
         "Score": float,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "RulesetName": str,
         "EvaluationContext": str,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "JobName": str,
         "JobRunId": str,
         "RulesetEvaluationRunId": str,
@@ -8887,15 +7695,15 @@
     },
 )
 
 GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
     "GetDataQualityRuleRecommendationRunResponseTypeDef",
     {
         "RunId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Role": str,
         "NumberOfWorkers": int,
         "Timeout": int,
         "Status": TaskStatusTypeType,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
@@ -8907,197 +7715,259 @@
     },
 )
 
 GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
     "GetDataQualityRulesetEvaluationRunResponseTypeDef",
     {
         "RunId": str,
-        "DataSource": DataSourceOutputTypeDef,
+        "DataSource": DataSourceTypeDef,
         "Role": str,
         "NumberOfWorkers": int,
         "Timeout": int,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "Status": TaskStatusTypeType,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
         "RulesetNames": List[str],
         "ResultIds": List[str],
-        "AdditionalDataSources": Dict[str, DataSourceOutputTypeDef],
+        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataQualityResultFilterCriteriaTypeDef = TypedDict(
-    "DataQualityResultFilterCriteriaTypeDef",
+_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedAfter": TimestampTypeDef,
-        "StartedBefore": TimestampTypeDef,
+        "Role": str,
+    },
+)
+_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "CreatedRulesetName": str,
+        "ClientToken": str,
     },
     total=False,
 )
 
-_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "RulesetNames": Sequence[str],
     },
 )
-_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "ClientToken": str,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
-class DataQualityRuleRecommendationRunFilterTypeDef(
-    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
-    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
     {
-        "DataSource": DataSourceTypeDef,
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
     {
-        "StartedBefore": TimestampTypeDef,
-        "StartedAfter": TimestampTypeDef,
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "Ids": List[str],
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
+    "GetDataCatalogEncryptionSettingsResponseTypeDef",
+    {
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    {
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+    },
+)
+_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
     },
     total=False,
 )
 
-class DataQualityRulesetEvaluationRunFilterTypeDef(
-    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
-    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
+    _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
+    _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
-DataSourceUnionTypeDef = Union[DataSourceTypeDef, DataSourceOutputTypeDef]
-_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+_RequiredDatabaseInputTypeDef = TypedDict(
+    "_RequiredDatabaseInputTypeDef",
     {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
+        "Name": str,
     },
 )
-_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+_OptionalDatabaseInputTypeDef = TypedDict(
+    "_OptionalDatabaseInputTypeDef",
     {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "CreatedRulesetName": str,
-        "ClientToken": str,
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Mapping[str, str],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "TargetDatabase": DatabaseIdentifierTypeDef,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
-class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-):
+class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
-_RequiredDropNullFieldsOutputTypeDef = TypedDict(
-    "_RequiredDropNullFieldsOutputTypeDef",
+_RequiredDatabaseTypeDef = TypedDict(
+    "_RequiredDatabaseTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
     },
 )
-_OptionalDropNullFieldsOutputTypeDef = TypedDict(
-    "_OptionalDropNullFieldsOutputTypeDef",
+_OptionalDatabaseTypeDef = TypedDict(
+    "_OptionalDatabaseTypeDef",
     {
-        "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": List[NullValueFieldTypeDef],
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Dict[str, str],
+        "CreateTime": datetime,
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "TargetDatabase": DatabaseIdentifierTypeDef,
+        "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
-class DropNullFieldsOutputTypeDef(
-    _RequiredDropNullFieldsOutputTypeDef, _OptionalDropNullFieldsOutputTypeDef
+class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
+    pass
+
+ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+_RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetMLTaskRunsRequestRequestTypeDef",
+    {
+        "TransformId": str,
+    },
+)
+_OptionalGetMLTaskRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetMLTaskRunsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TaskRunFilterCriteriaTypeDef,
+        "Sort": TaskRunSortCriteriaTypeDef,
+    },
+    total=False,
+)
+
+class GetMLTaskRunsRequestRequestTypeDef(
+    _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
     },
 )
 _OptionalDropNullFieldsTypeDef = TypedDict(
     "_OptionalDropNullFieldsTypeDef",
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": Sequence[NullValueFieldTypeDef],
+        "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
-_RequiredColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_RequiredColumnStatisticsDataOutputTypeDef",
+_RequiredColumnStatisticsDataTypeDef = TypedDict(
+    "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
-_OptionalColumnStatisticsDataOutputTypeDef = TypedDict(
-    "_OptionalColumnStatisticsDataOutputTypeDef",
+_OptionalColumnStatisticsDataTypeDef = TypedDict(
+    "_OptionalColumnStatisticsDataTypeDef",
     {
         "BooleanColumnStatisticsData": BooleanColumnStatisticsDataTypeDef,
-        "DateColumnStatisticsData": DateColumnStatisticsDataOutputTypeDef,
-        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataOutputTypeDef,
+        "DateColumnStatisticsData": DateColumnStatisticsDataTypeDef,
+        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataTypeDef,
         "DoubleColumnStatisticsData": DoubleColumnStatisticsDataTypeDef,
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
-class ColumnStatisticsDataOutputTypeDef(
-    _RequiredColumnStatisticsDataOutputTypeDef, _OptionalColumnStatisticsDataOutputTypeDef
+class ColumnStatisticsDataTypeDef(
+    _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
-StorageDescriptorOutputTypeDef = TypedDict(
-    "StorageDescriptorOutputTypeDef",
-    {
-        "Columns": List[ColumnOutputTypeDef],
-        "Location": str,
-        "AdditionalLocations": List[str],
-        "InputFormat": str,
-        "OutputFormat": str,
-        "Compressed": bool,
-        "NumberOfBuckets": int,
-        "SerdeInfo": SerDeInfoOutputTypeDef,
-        "BucketColumns": List[str],
-        "SortColumns": List[OrderTypeDef],
-        "Parameters": Dict[str, str],
-        "SkewedInfo": SkewedInfoOutputTypeDef,
-        "StoredAsSubDirectories": bool,
-        "SchemaReference": SchemaReferenceTypeDef,
-    },
-    total=False,
-)
-
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -9111,60 +7981,47 @@
         "SkewedInfo": SkewedInfoTypeDef,
         "StoredAsSubDirectories": bool,
         "SchemaReference": SchemaReferenceTypeDef,
     },
     total=False,
 )
 
-SecurityConfigurationTypeDef = TypedDict(
-    "SecurityConfigurationTypeDef",
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
-        "CreatedTimeStamp": datetime,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
-    total=False,
 )
 
-CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateSecurityConfigurationRequestRequestTypeDef",
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
     {
         "Name": str,
+        "CreatedTimeStamp": datetime,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
+    total=False,
 )
 
-EncryptionConfigurationUnionTypeDef = Union[
-    EncryptionConfigurationTypeDef, EncryptionConfigurationOutputTypeDef
-]
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": List[FilterExpressionOutputTypeDef],
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": Sequence[FilterExpressionTypeDef],
+        "Filters": List[FilterExpressionTypeDef],
     },
 )
 
 _RequiredUpdateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -9211,441 +8068,29 @@
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredAthenaConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredAthenaConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-        "SchemaName": str,
-    },
-)
-_OptionalAthenaConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalAthenaConnectorSourceOutputTypeDef",
-    {
-        "ConnectionTable": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class AthenaConnectorSourceOutputTypeDef(
-    _RequiredAthenaConnectorSourceOutputTypeDef, _OptionalAthenaConnectorSourceOutputTypeDef
-):
-    pass
-
-_RequiredCatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogDeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogDeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class CatalogDeltaSourceOutputTypeDef(
-    _RequiredCatalogDeltaSourceOutputTypeDef, _OptionalCatalogDeltaSourceOutputTypeDef
-):
-    pass
-
-_RequiredCatalogHudiSourceOutputTypeDef = TypedDict(
-    "_RequiredCatalogHudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogHudiSourceOutputTypeDef = TypedDict(
-    "_OptionalCatalogHudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class CatalogHudiSourceOutputTypeDef(
-    _RequiredCatalogHudiSourceOutputTypeDef, _OptionalCatalogHudiSourceOutputTypeDef
-):
-    pass
-
-_RequiredCustomCodeOutputTypeDef = TypedDict(
-    "_RequiredCustomCodeOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Code": str,
-        "ClassName": str,
-    },
-)
-_OptionalCustomCodeOutputTypeDef = TypedDict(
-    "_OptionalCustomCodeOutputTypeDef",
-    {
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class CustomCodeOutputTypeDef(_RequiredCustomCodeOutputTypeDef, _OptionalCustomCodeOutputTypeDef):
-    pass
-
-_RequiredDynamicTransformOutputTypeDef = TypedDict(
-    "_RequiredDynamicTransformOutputTypeDef",
-    {
-        "Name": str,
-        "TransformName": str,
-        "Inputs": List[str],
-        "FunctionName": str,
-        "Path": str,
-    },
-)
-_OptionalDynamicTransformOutputTypeDef = TypedDict(
-    "_OptionalDynamicTransformOutputTypeDef",
-    {
-        "Parameters": List[TransformConfigParameterOutputTypeDef],
-        "Version": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class DynamicTransformOutputTypeDef(
-    _RequiredDynamicTransformOutputTypeDef, _OptionalDynamicTransformOutputTypeDef
-):
-    pass
-
-_RequiredJDBCConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredJDBCConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalJDBCConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalJDBCConnectorSourceOutputTypeDef",
-    {
-        "AdditionalOptions": JDBCConnectorOptionsOutputTypeDef,
-        "ConnectionTable": str,
-        "Query": str,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class JDBCConnectorSourceOutputTypeDef(
-    _RequiredJDBCConnectorSourceOutputTypeDef, _OptionalJDBCConnectorSourceOutputTypeDef
-):
-    pass
-
-_RequiredJDBCConnectorTargetOutputTypeDef = TypedDict(
-    "_RequiredJDBCConnectorTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "ConnectionName": str,
-        "ConnectionTable": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalJDBCConnectorTargetOutputTypeDef = TypedDict(
-    "_OptionalJDBCConnectorTargetOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class JDBCConnectorTargetOutputTypeDef(
-    _RequiredJDBCConnectorTargetOutputTypeDef, _OptionalJDBCConnectorTargetOutputTypeDef
-):
-    pass
-
-_RequiredS3CatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogDeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogDeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogDeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3CatalogDeltaSourceOutputTypeDef(
-    _RequiredS3CatalogDeltaSourceOutputTypeDef, _OptionalS3CatalogDeltaSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3CatalogHudiSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CatalogHudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogHudiSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CatalogHudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3CatalogHudiSourceOutputTypeDef(
-    _RequiredS3CatalogHudiSourceOutputTypeDef, _OptionalS3CatalogHudiSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3CsvSourceOutputTypeDef = TypedDict(
-    "_RequiredS3CsvSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-        "Separator": SeparatorType,
-        "QuoteChar": QuoteCharType,
-    },
-)
-_OptionalS3CsvSourceOutputTypeDef = TypedDict(
-    "_OptionalS3CsvSourceOutputTypeDef",
-    {
-        "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "Escaper": str,
-        "Multiline": bool,
-        "WithHeader": bool,
-        "WriteHeader": bool,
-        "SkipFirst": bool,
-        "OptimizePerformance": bool,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3CsvSourceOutputTypeDef(
-    _RequiredS3CsvSourceOutputTypeDef, _OptionalS3CsvSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3DeltaSourceOutputTypeDef = TypedDict(
-    "_RequiredS3DeltaSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3DeltaSourceOutputTypeDef = TypedDict(
-    "_OptionalS3DeltaSourceOutputTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3DeltaSourceOutputTypeDef(
-    _RequiredS3DeltaSourceOutputTypeDef, _OptionalS3DeltaSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3HudiSourceOutputTypeDef = TypedDict(
-    "_RequiredS3HudiSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3HudiSourceOutputTypeDef = TypedDict(
-    "_OptionalS3HudiSourceOutputTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3HudiSourceOutputTypeDef(
-    _RequiredS3HudiSourceOutputTypeDef, _OptionalS3HudiSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3JsonSourceOutputTypeDef = TypedDict(
-    "_RequiredS3JsonSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3JsonSourceOutputTypeDef = TypedDict(
-    "_OptionalS3JsonSourceOutputTypeDef",
-    {
-        "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "JsonPath": str,
-        "Multiline": bool,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3JsonSourceOutputTypeDef(
-    _RequiredS3JsonSourceOutputTypeDef, _OptionalS3JsonSourceOutputTypeDef
-):
-    pass
-
-_RequiredS3ParquetSourceOutputTypeDef = TypedDict(
-    "_RequiredS3ParquetSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3ParquetSourceOutputTypeDef = TypedDict(
-    "_OptionalS3ParquetSourceOutputTypeDef",
-    {
-        "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": List[str],
-        "GroupSize": str,
-        "GroupFiles": str,
-        "Recurse": bool,
-        "MaxBand": int,
-        "MaxFilesInBand": int,
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class S3ParquetSourceOutputTypeDef(
-    _RequiredS3ParquetSourceOutputTypeDef, _OptionalS3ParquetSourceOutputTypeDef
-):
-    pass
-
-_RequiredSparkConnectorSourceOutputTypeDef = TypedDict(
-    "_RequiredSparkConnectorSourceOutputTypeDef",
-    {
-        "Name": str,
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalSparkConnectorSourceOutputTypeDef = TypedDict(
-    "_OptionalSparkConnectorSourceOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class SparkConnectorSourceOutputTypeDef(
-    _RequiredSparkConnectorSourceOutputTypeDef, _OptionalSparkConnectorSourceOutputTypeDef
-):
-    pass
-
-_RequiredSparkConnectorTargetOutputTypeDef = TypedDict(
-    "_RequiredSparkConnectorTargetOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "ConnectionName": str,
-        "ConnectorName": str,
-        "ConnectionType": str,
-    },
-)
-_OptionalSparkConnectorTargetOutputTypeDef = TypedDict(
-    "_OptionalSparkConnectorTargetOutputTypeDef",
-    {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class SparkConnectorTargetOutputTypeDef(
-    _RequiredSparkConnectorTargetOutputTypeDef, _OptionalSparkConnectorTargetOutputTypeDef
-):
-    pass
-
-_RequiredSparkSQLOutputTypeDef = TypedDict(
-    "_RequiredSparkSQLOutputTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "SqlQuery": str,
-        "SqlAliases": List[SqlAliasTypeDef],
-    },
-)
-_OptionalSparkSQLOutputTypeDef = TypedDict(
-    "_OptionalSparkSQLOutputTypeDef",
-    {
-        "OutputSchemas": List[GlueSchemaOutputTypeDef],
-    },
-    total=False,
-)
-
-class SparkSQLOutputTypeDef(_RequiredSparkSQLOutputTypeDef, _OptionalSparkSQLOutputTypeDef):
-    pass
-
 _RequiredAthenaConnectorSourceTypeDef = TypedDict(
     "_RequiredAthenaConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
         "SchemaName": str,
     },
 )
 _OptionalAthenaConnectorSourceTypeDef = TypedDict(
     "_OptionalAthenaConnectorSourceTypeDef",
     {
         "ConnectionTable": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
@@ -9658,16 +8103,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalCatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
 ):
@@ -9680,61 +8125,61 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogHudiSourceTypeDef = TypedDict(
     "_OptionalCatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
 ):
     pass
 
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "Code": str,
         "ClassName": str,
     },
 )
 _OptionalCustomCodeTypeDef = TypedDict(
     "_OptionalCustomCodeTypeDef",
     {
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "FunctionName": str,
         "Path": str,
     },
 )
 _OptionalDynamicTransformTypeDef = TypedDict(
     "_OptionalDynamicTransformTypeDef",
     {
-        "Parameters": Sequence[TransformConfigParameterTypeDef],
+        "Parameters": List[TransformConfigParameterTypeDef],
         "Version": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
 
@@ -9749,40 +8194,40 @@
 )
 _OptionalJDBCConnectorSourceTypeDef = TypedDict(
     "_OptionalJDBCConnectorSourceTypeDef",
     {
         "AdditionalOptions": JDBCConnectorOptionsTypeDef,
         "ConnectionTable": str,
         "Query": str,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalJDBCConnectorTargetTypeDef = TypedDict(
     "_OptionalJDBCConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
@@ -9795,16 +8240,16 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalS3CatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
 ):
@@ -9817,146 +8262,146 @@
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogHudiSourceTypeDef = TypedDict(
     "_OptionalS3CatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
 ):
     pass
 
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
     },
 )
 _OptionalS3CsvSourceTypeDef = TypedDict(
     "_OptionalS3CsvSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "Escaper": str,
         "Multiline": bool,
         "WithHeader": bool,
         "WriteHeader": bool,
         "SkipFirst": bool,
         "OptimizePerformance": bool,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3DeltaSourceTypeDef = TypedDict(
     "_OptionalS3DeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Mapping[str, str],
+        "AdditionalDeltaOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3HudiSourceTypeDef = TypedDict(
     "_OptionalS3HudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Mapping[str, str],
+        "AdditionalHudiOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3JsonSourceTypeDef = TypedDict(
     "_OptionalS3JsonSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "JsonPath": str,
         "Multiline": bool,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
-        "Paths": Sequence[str],
+        "Paths": List[str],
     },
 )
 _OptionalS3ParquetSourceTypeDef = TypedDict(
     "_OptionalS3ParquetSourceTypeDef",
     {
         "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": Sequence[str],
+        "Exclusions": List[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
@@ -9968,62 +8413,62 @@
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorSourceTypeDef = TypedDict(
     "_OptionalSparkConnectorSourceTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorTargetTypeDef = TypedDict(
     "_OptionalSparkConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Mapping[str, str],
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
-        "Inputs": Sequence[str],
+        "Inputs": List[str],
         "SqlQuery": str,
-        "SqlAliases": Sequence[SqlAliasTypeDef],
+        "SqlAliases": List[SqlAliasTypeDef],
     },
 )
 _OptionalSparkSQLTypeDef = TypedDict(
     "_OptionalSparkSQLTypeDef",
     {
-        "OutputSchemas": Sequence[GlueSchemaTypeDef],
+        "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
@@ -10086,15 +8531,15 @@
     total=False,
 )
 
 _RequiredCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMLTransformRequestRequestTypeDef",
     {
         "Name": str,
-        "InputRecordTables": Sequence[GlueTableUnionTypeDef],
+        "InputRecordTables": Sequence[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "Role": str,
     },
 )
 _OptionalCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMLTransformRequestRequestTypeDef",
     {
@@ -10122,57 +8567,14 @@
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToDelete": Sequence[PartitionValueListUnionTypeDef],
-    },
-)
-_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchDeletePartitionRequestRequestTypeDef(
-    _RequiredBatchDeletePartitionRequestRequestTypeDef,
-    _OptionalBatchDeletePartitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToGet": Sequence[PartitionValueListUnionTypeDef],
-    },
-)
-_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchGetPartitionRequestRequestTypeDef(
-    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
 )
@@ -10239,85 +8641,23 @@
         "Progress": float,
         "StartedOn": int,
         "CompletedOn": int,
     },
     total=False,
 )
 
-_RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTriggerRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Type": TriggerTypeType,
-        "Actions": Sequence[ActionUnionTypeDef],
-    },
-)
-_OptionalCreateTriggerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTriggerRequestRequestTypeDef",
-    {
-        "WorkflowName": str,
-        "Schedule": str,
-        "Predicate": PredicateTypeDef,
-        "Description": str,
-        "StartOnCreation": bool,
-        "Tags": Mapping[str, str],
-        "EventBatchingCondition": EventBatchingConditionTypeDef,
-    },
-    total=False,
-)
-
-class CreateTriggerRequestRequestTypeDef(
-    _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
-):
-    pass
-
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredColumnStatisticsDataTypeDef = TypedDict(
-    "_RequiredColumnStatisticsDataTypeDef",
-    {
-        "Type": ColumnStatisticsTypeType,
-    },
-)
-_OptionalColumnStatisticsDataTypeDef = TypedDict(
-    "_OptionalColumnStatisticsDataTypeDef",
-    {
-        "BooleanColumnStatisticsData": BooleanColumnStatisticsDataTypeDef,
-        "DateColumnStatisticsData": DateColumnStatisticsDataTypeDef,
-        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataTypeDef,
-        "DoubleColumnStatisticsData": DoubleColumnStatisticsDataTypeDef,
-        "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
-        "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
-        "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
-    },
-    total=False,
-)
-
-class ColumnStatisticsDataTypeDef(
-    _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
-):
-    pass
-
-CreateScriptRequestRequestTypeDef = TypedDict(
-    "CreateScriptRequestRequestTypeDef",
-    {
-        "DagNodes": Sequence[CodeGenNodeUnionTypeDef],
-        "DagEdges": Sequence[CodeGenEdgeTypeDef],
-        "Language": LanguageType,
-    },
-    total=False,
-)
-
 BatchGetTriggersResponseTypeDef = TypedDict(
     "BatchGetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "TriggersNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -10369,15 +8709,15 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "InputRecordTables": List[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
         "Schema": List[SchemaColumnTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
@@ -10395,15 +8735,15 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "InputRecordTables": List[GlueTableTypeDef],
         "Parameters": TransformParametersTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
         "Schema": List[SchemaColumnTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
@@ -10438,78 +8778,31 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDatabaseResponseTypeDef = TypedDict(
-    "GetDatabaseResponseTypeDef",
-    {
-        "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDatabasesResponseTypeDef = TypedDict(
-    "GetDatabasesResponseTypeDef",
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
     {
-        "DatabaseList": List[DatabaseTypeDef],
+        "Results": List[DataQualityResultDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatabaseRequestRequestTypeDef",
-    {
-        "DatabaseInput": DatabaseInputTypeDef,
-    },
-)
-_OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatabaseRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDatabaseRequestRequestTypeDef(
-    _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDatabaseRequestRequestTypeDef",
-    {
-        "Name": str,
-        "DatabaseInput": DatabaseInputTypeDef,
-    },
-)
-_OptionalUpdateDatabaseRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDatabaseRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class UpdateDatabaseRequestRequestTypeDef(
-    _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
-):
-    pass
-
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
+ListDataQualityResultsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityResultsRequestRequestTypeDef",
     {
-        "Results": List[DataQualityResultDescriptionTypeDef],
+        "Filter": DataQualityResultFilterCriteriaTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxResults": int,
     },
+    total=False,
 )
 
 BatchGetDataQualityResultResponseTypeDef = TypedDict(
     "BatchGetDataQualityResultResponseTypeDef",
     {
         "Results": List[DataQualityResultTypeDef],
         "ResultsNotFound": List[str],
@@ -10522,179 +8815,200 @@
     {
         "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
     "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
     {
         "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityResultsRequestRequestTypeDef",
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     {
-        "Filter": DataQualityResultFilterCriteriaTypeDef,
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+_RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "DatabaseInput": DatabaseInputTypeDef,
     },
-    total=False,
 )
-
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+_OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatabaseRequestRequestTypeDef",
     {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "CatalogId": str,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+class CreateDatabaseRequestRequestTypeDef(
+    _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "RulesetNames": Sequence[str],
+        "Name": str,
+        "DatabaseInput": DatabaseInputTypeDef,
     },
 )
-_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+_OptionalUpdateDatabaseRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "ClientToken": str,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "AdditionalDataSources": Mapping[str, DataSourceUnionTypeDef],
+        "CatalogId": str,
     },
     total=False,
 )
 
-class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+class UpdateDatabaseRequestRequestTypeDef(
+    _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
-ColumnStatisticsOutputTypeDef = TypedDict(
-    "ColumnStatisticsOutputTypeDef",
+GetDatabaseResponseTypeDef = TypedDict(
+    "GetDatabaseResponseTypeDef",
+    {
+        "Database": DatabaseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDatabasesResponseTypeDef = TypedDict(
+    "GetDatabasesResponseTypeDef",
+    {
+        "DatabaseList": List[DatabaseTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ColumnStatisticsTypeDef = TypedDict(
+    "ColumnStatisticsTypeDef",
     {
         "ColumnName": str,
         "ColumnType": str,
         "AnalyzedTime": datetime,
-        "StatisticsData": ColumnStatisticsDataOutputTypeDef,
+        "StatisticsData": ColumnStatisticsDataTypeDef,
+    },
+)
+
+PartitionInputTypeDef = TypedDict(
+    "PartitionInputTypeDef",
+    {
+        "Values": Sequence[str],
+        "LastAccessTime": TimestampTypeDef,
+        "StorageDescriptor": StorageDescriptorTypeDef,
+        "Parameters": Mapping[str, str],
+        "LastAnalyzedTime": TimestampTypeDef,
     },
+    total=False,
 )
 
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "Values": List[str],
         "DatabaseName": str,
         "TableName": str,
         "CreationTime": datetime,
         "LastAccessTime": datetime,
-        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "StorageDescriptor": StorageDescriptorTypeDef,
         "Parameters": Dict[str, str],
         "LastAnalyzedTime": datetime,
         "CatalogId": str,
     },
     total=False,
 )
 
-_RequiredTableTypeDef = TypedDict(
-    "_RequiredTableTypeDef",
+_RequiredTableInputTypeDef = TypedDict(
+    "_RequiredTableInputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalTableTypeDef = TypedDict(
-    "_OptionalTableTypeDef",
+_OptionalTableInputTypeDef = TypedDict(
+    "_OptionalTableInputTypeDef",
     {
-        "DatabaseName": str,
         "Description": str,
         "Owner": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "LastAccessTime": datetime,
-        "LastAnalyzedTime": datetime,
+        "LastAccessTime": TimestampTypeDef,
+        "LastAnalyzedTime": TimestampTypeDef,
         "Retention": int,
-        "StorageDescriptor": StorageDescriptorOutputTypeDef,
-        "PartitionKeys": List[ColumnOutputTypeDef],
+        "StorageDescriptor": StorageDescriptorTypeDef,
+        "PartitionKeys": Sequence[ColumnTypeDef],
         "ViewOriginalText": str,
         "ViewExpandedText": str,
         "TableType": str,
-        "Parameters": Dict[str, str],
-        "CreatedBy": str,
-        "IsRegisteredWithLakeFormation": bool,
+        "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
-        "CatalogId": str,
-        "VersionId": str,
-        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
-class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
+class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
-PartitionInputTypeDef = TypedDict(
-    "PartitionInputTypeDef",
-    {
-        "Values": Sequence[str],
-        "LastAccessTime": TimestampTypeDef,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "Parameters": Mapping[str, str],
-        "LastAnalyzedTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTableInputTypeDef = TypedDict(
-    "_RequiredTableInputTypeDef",
+_RequiredTableTypeDef = TypedDict(
+    "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalTableInputTypeDef = TypedDict(
-    "_OptionalTableInputTypeDef",
+_OptionalTableTypeDef = TypedDict(
+    "_OptionalTableTypeDef",
     {
+        "DatabaseName": str,
         "Description": str,
         "Owner": str,
-        "LastAccessTime": TimestampTypeDef,
-        "LastAnalyzedTime": TimestampTypeDef,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "LastAccessTime": datetime,
+        "LastAnalyzedTime": datetime,
         "Retention": int,
         "StorageDescriptor": StorageDescriptorTypeDef,
-        "PartitionKeys": Sequence[ColumnTypeDef],
+        "PartitionKeys": List[ColumnTypeDef],
         "ViewOriginalText": str,
         "ViewExpandedText": str,
         "TableType": str,
-        "Parameters": Mapping[str, str],
+        "Parameters": Dict[str, str],
+        "CreatedBy": str,
+        "IsRegisteredWithLakeFormation": bool,
         "TargetTable": TableIdentifierTypeDef,
+        "CatalogId": str,
+        "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
-class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
+class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10706,87 +9020,14 @@
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CodeGenConfigurationNodeOutputTypeDef = TypedDict(
-    "CodeGenConfigurationNodeOutputTypeDef",
-    {
-        "AthenaConnectorSource": AthenaConnectorSourceOutputTypeDef,
-        "JDBCConnectorSource": JDBCConnectorSourceOutputTypeDef,
-        "SparkConnectorSource": SparkConnectorSourceOutputTypeDef,
-        "CatalogSource": CatalogSourceTypeDef,
-        "RedshiftSource": RedshiftSourceTypeDef,
-        "S3CatalogSource": S3CatalogSourceTypeDef,
-        "S3CsvSource": S3CsvSourceOutputTypeDef,
-        "S3JsonSource": S3JsonSourceOutputTypeDef,
-        "S3ParquetSource": S3ParquetSourceOutputTypeDef,
-        "RelationalCatalogSource": RelationalCatalogSourceTypeDef,
-        "DynamoDBCatalogSource": DynamoDBCatalogSourceTypeDef,
-        "JDBCConnectorTarget": JDBCConnectorTargetOutputTypeDef,
-        "SparkConnectorTarget": SparkConnectorTargetOutputTypeDef,
-        "CatalogTarget": BasicCatalogTargetOutputTypeDef,
-        "RedshiftTarget": RedshiftTargetOutputTypeDef,
-        "S3CatalogTarget": S3CatalogTargetOutputTypeDef,
-        "S3GlueParquetTarget": S3GlueParquetTargetOutputTypeDef,
-        "S3DirectTarget": S3DirectTargetOutputTypeDef,
-        "ApplyMapping": ApplyMappingOutputTypeDef,
-        "SelectFields": SelectFieldsOutputTypeDef,
-        "DropFields": DropFieldsOutputTypeDef,
-        "RenameField": RenameFieldOutputTypeDef,
-        "Spigot": SpigotOutputTypeDef,
-        "Join": JoinOutputTypeDef,
-        "SplitFields": SplitFieldsOutputTypeDef,
-        "SelectFromCollection": SelectFromCollectionOutputTypeDef,
-        "FillMissingValues": FillMissingValuesOutputTypeDef,
-        "Filter": FilterOutputTypeDef,
-        "CustomCode": CustomCodeOutputTypeDef,
-        "SparkSQL": SparkSQLOutputTypeDef,
-        "DirectKinesisSource": DirectKinesisSourceOutputTypeDef,
-        "DirectKafkaSource": DirectKafkaSourceOutputTypeDef,
-        "CatalogKinesisSource": CatalogKinesisSourceOutputTypeDef,
-        "CatalogKafkaSource": CatalogKafkaSourceOutputTypeDef,
-        "DropNullFields": DropNullFieldsOutputTypeDef,
-        "Merge": MergeOutputTypeDef,
-        "Union": UnionOutputTypeDef,
-        "PIIDetection": PIIDetectionOutputTypeDef,
-        "Aggregate": AggregateOutputTypeDef,
-        "DropDuplicates": DropDuplicatesOutputTypeDef,
-        "GovernedCatalogTarget": GovernedCatalogTargetOutputTypeDef,
-        "GovernedCatalogSource": GovernedCatalogSourceTypeDef,
-        "MicrosoftSQLServerCatalogSource": MicrosoftSQLServerCatalogSourceTypeDef,
-        "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
-        "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
-        "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
-        "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetOutputTypeDef,
-        "MySQLCatalogTarget": MySQLCatalogTargetOutputTypeDef,
-        "OracleSQLCatalogTarget": OracleSQLCatalogTargetOutputTypeDef,
-        "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetOutputTypeDef,
-        "DynamicTransform": DynamicTransformOutputTypeDef,
-        "EvaluateDataQuality": EvaluateDataQualityOutputTypeDef,
-        "S3CatalogHudiSource": S3CatalogHudiSourceOutputTypeDef,
-        "CatalogHudiSource": CatalogHudiSourceOutputTypeDef,
-        "S3HudiSource": S3HudiSourceOutputTypeDef,
-        "S3HudiCatalogTarget": S3HudiCatalogTargetOutputTypeDef,
-        "S3HudiDirectTarget": S3HudiDirectTargetOutputTypeDef,
-        "DirectJDBCSource": DirectJDBCSourceTypeDef,
-        "S3CatalogDeltaSource": S3CatalogDeltaSourceOutputTypeDef,
-        "CatalogDeltaSource": CatalogDeltaSourceOutputTypeDef,
-        "S3DeltaSource": S3DeltaSourceOutputTypeDef,
-        "S3DeltaCatalogTarget": S3DeltaCatalogTargetOutputTypeDef,
-        "S3DeltaDirectTarget": S3DeltaDirectTargetOutputTypeDef,
-        "AmazonRedshiftSource": AmazonRedshiftSourceOutputTypeDef,
-        "AmazonRedshiftTarget": AmazonRedshiftTargetOutputTypeDef,
-        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameOutputTypeDef,
-    },
-    total=False,
-)
-
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
         "JDBCConnectorSource": JDBCConnectorSourceTypeDef,
         "SparkConnectorSource": SparkConnectorSourceTypeDef,
         "CatalogSource": CatalogSourceTypeDef,
@@ -10878,24 +9119,14 @@
     {
         "Statements": List[StatementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnStatisticsTypeDef = TypedDict(
-    "ColumnStatisticsTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnType": str,
-        "AnalyzedTime": TimestampTypeDef,
-        "StatisticsData": ColumnStatisticsDataTypeDef,
-    },
-)
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Type": NodeTypeType,
         "Name": str,
         "UniqueId": str,
         "TriggerDetails": TriggerNodeDetailsTypeDef,
@@ -10913,130 +9144,83 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
-        "ColumnStatistics": ColumnStatisticsOutputTypeDef,
+        "ColumnStatistics": ColumnStatisticsTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetPartitionResponseTypeDef = TypedDict(
-    "BatchGetPartitionResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "UnprocessedKeys": List[PartitionValueListOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionResponseTypeDef = TypedDict(
-    "GetPartitionResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionsResponseTypeDef = TypedDict(
-    "GetPartitionsResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionMetadataResponseTypeDef",
+_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionValues": Sequence[str],
+        "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
 )
-
-UnfilteredPartitionTypeDef = TypedDict(
-    "UnfilteredPartitionTypeDef",
+_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
+        "CatalogId": str,
     },
     total=False,
 )
 
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTablesResponseTypeDef = TypedDict(
-    "GetTablesResponseTypeDef",
-    {
-        "TableList": List[TableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredTableMetadataResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
+    _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
+    _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
+):
+    pass
 
-SearchTablesResponseTypeDef = TypedDict(
-    "SearchTablesResponseTypeDef",
+_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DatabaseName": str,
+        "TableName": str,
+        "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
 )
-
-TableVersionTypeDef = TypedDict(
-    "TableVersionTypeDef",
+_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
-        "Table": TableTypeDef,
-        "VersionId": str,
+        "CatalogId": str,
     },
     total=False,
 )
 
+class UpdateColumnStatisticsForTableRequestRequestTypeDef(
+    _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
+    _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
+):
+    pass
+
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -11102,14 +9286,60 @@
 )
 
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
+BatchGetPartitionResponseTypeDef = TypedDict(
+    "BatchGetPartitionResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "UnprocessedKeys": List[PartitionValueListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionResponseTypeDef = TypedDict(
+    "GetPartitionResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionsResponseTypeDef = TypedDict(
+    "GetPartitionsResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionMetadataResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnfilteredPartitionTypeDef = TypedDict(
+    "UnfilteredPartitionTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+    },
+    total=False,
+)
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -11147,47 +9377,129 @@
 )
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTablesResponseTypeDef = TypedDict(
+    "GetTablesResponseTypeDef",
+    {
+        "TableList": List[TableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredTableMetadataResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "CellFilters": List[ColumnRowFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchTablesResponseTypeDef = TypedDict(
+    "SearchTablesResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableVersionTypeDef = TypedDict(
+    "TableVersionTypeDef",
+    {
+        "Table": TableTypeDef,
+        "VersionId": str,
+    },
+    total=False,
+)
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Role": str,
+        "Command": JobCommandTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LogUri": str,
+        "ExecutionProperty": ExecutionPropertyTypeDef,
+        "DefaultArguments": Mapping[str, str],
+        "NonOverridableArguments": Mapping[str, str],
+        "Connections": ConnectionsListTypeDef,
+        "MaxRetries": int,
+        "AllocatedCapacity": int,
+        "Timeout": int,
+        "MaxCapacity": float,
+        "SecurityConfiguration": str,
+        "Tags": Mapping[str, str],
+        "NotificationProperty": NotificationPropertyTypeDef,
+        "GlueVersion": str,
+        "NumberOfWorkers": int,
+        "WorkerType": WorkerTypeType,
+        "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
+        "ExecutionClass": ExecutionClassType,
+        "SourceControlDetails": SourceControlDetailsTypeDef,
+    },
+    total=False,
+)
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "ExecutionProperty": ExecutionPropertyTypeDef,
         "Command": JobCommandTypeDef,
         "DefaultArguments": Dict[str, str],
         "NonOverridableArguments": Dict[str, str],
-        "Connections": ConnectionsListOutputTypeDef,
+        "Connections": ConnectionsListTypeDef,
         "MaxRetries": int,
         "AllocatedCapacity": int,
         "Timeout": int,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "GlueVersion": str,
-        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeOutputTypeDef],
+        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-CodeGenConfigurationNodeUnionTypeDef = Union[
-    CodeGenConfigurationNodeTypeDef, CodeGenConfigurationNodeOutputTypeDef
-]
 JobUpdateTypeDef = TypedDict(
     "JobUpdateTypeDef",
     {
         "Description": str,
         "LogUri": str,
         "Role": str,
         "ExecutionProperty": ExecutionPropertyTypeDef,
@@ -11207,15 +9519,14 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-ColumnStatisticsUnionTypeDef = Union[ColumnStatisticsTypeDef, ColumnStatisticsOutputTypeDef]
 WorkflowGraphTypeDef = TypedDict(
     "WorkflowGraphTypeDef",
     {
         "Nodes": List[NodeTypeDef],
         "Edges": List[EdgeTypeDef],
     },
     total=False,
@@ -11233,14 +9544,36 @@
     "UpdateColumnStatisticsForTableResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "Entries": Sequence[BatchUpdatePartitionRequestEntryTypeDef],
+    },
+)
+_OptionalBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchUpdatePartitionRequestRequestTypeDef(
+    _RequiredBatchUpdatePartitionRequestRequestTypeDef,
+    _OptionalBatchUpdatePartitionRequestRequestTypeDef,
+):
+    pass
+
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11259,36 +9592,14 @@
     {
         "TableVersions": List[TableVersionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "Entries": Sequence[BatchUpdatePartitionRequestEntryTypeDef],
-    },
-)
-_OptionalBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchUpdatePartitionRequestRequestTypeDef(
-    _RequiredBatchUpdatePartitionRequestRequestTypeDef,
-    _OptionalBatchUpdatePartitionRequestRequestTypeDef,
-):
-    pass
-
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11307,106 +9618,22 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Role": str,
-        "Command": JobCommandTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LogUri": str,
-        "ExecutionProperty": ExecutionPropertyTypeDef,
-        "DefaultArguments": Mapping[str, str],
-        "NonOverridableArguments": Mapping[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "MaxRetries": int,
-        "AllocatedCapacity": int,
-        "Timeout": int,
-        "MaxCapacity": float,
-        "SecurityConfiguration": str,
-        "Tags": Mapping[str, str],
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "GlueVersion": str,
-        "NumberOfWorkers": int,
-        "WorkerType": WorkerTypeType,
-        "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeUnionTypeDef],
-        "ExecutionClass": ExecutionClassType,
-        "SourceControlDetails": SourceControlDetailsTypeDef,
-    },
-    total=False,
-)
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
 UpdateJobRequestRequestTypeDef = TypedDict(
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
         "JobUpdate": JobUpdateTypeDef,
     },
 )
 
-_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionValues": Sequence[str],
-        "ColumnStatisticsList": Sequence[ColumnStatisticsUnionTypeDef],
-    },
-)
-_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
-    _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
-    _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "ColumnStatisticsList": Sequence[ColumnStatisticsUnionTypeDef],
-    },
-)
-_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class UpdateColumnStatisticsForTableRequestRequestTypeDef(
-    _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
-    _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
-):
-    pass
-
 WorkflowRunTypeDef = TypedDict(
     "WorkflowRunTypeDef",
     {
         "Name": str,
         "WorkflowRunId": str,
         "PreviousRunId": str,
         "WorkflowRunProperties": Dict[str, str],
```

### Comparing `types-aiobotocore-glue-2.5.2.post1/types_aiobotocore_glue.egg-info/SOURCES.txt` & `types-aiobotocore-glue-2.5.2.post2/types_aiobotocore_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

