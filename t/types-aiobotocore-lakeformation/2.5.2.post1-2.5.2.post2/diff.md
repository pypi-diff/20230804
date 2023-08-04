# Comparing `tmp/types-aiobotocore-lakeformation-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lakeformation-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lakeformation-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lakeformation-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lakeformation-2.5.2.post1.tar` & `types-aiobotocore-lakeformation-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39583 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39522 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55269 2023-08-02 14:41:44.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55171 2023-08-02 14:41:44.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13882 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12340 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:42:19.000000 types-aiobotocore-lakeformation-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1583 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1582 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39384 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39323 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10579 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10577 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7069 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7062 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48362 2023-08-04 13:42:22.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48277 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13882 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/LICENSE` & `types-aiobotocore-lakeformation-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/setup.py` & `types-aiobotocore-lakeformation-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lakeformation",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.py` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.pyi` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.py` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
+    BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterUnionTypeDef,
+    DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsUnionTypeDef,
+    DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -58,31 +58,31 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairUnionTypeDef,
-    LFTagUnionTypeDef,
+    LFTagPairTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
     TimestampTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -138,19 +138,15 @@
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#exceptions)
         """
 
     async def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -163,25 +159,25 @@
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#assume_decorated_role_with_saml)
         """
 
     async def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_grant_permissions)
         """
 
     async def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_revoke_permissions)
         """
@@ -215,15 +211,15 @@
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#commit_transaction)
         """
 
     async def create_data_cells_filter(
-        self, *, TableData: DataCellsFilterUnionTypeDef
+        self, *, TableData: DataCellsFilterTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#create_data_cells_filter)
@@ -383,19 +379,15 @@
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_query_statistics)
         """
 
     async def get_resource_lf_tags(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_resource_lf_tags)
         """
@@ -420,35 +412,35 @@
         """
 
     async def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
 
     async def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_temporary_glue_table_credentials)
@@ -474,29 +466,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_work_units)
         """
 
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#grant_permissions)
         """
 
     async def list_data_cells_filter(
-        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_data_cells_filter)
         """
@@ -518,15 +510,15 @@
 
     async def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceUnionTypeDef = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -579,15 +571,15 @@
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
 
     async def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#put_data_lake_settings)
@@ -605,32 +597,28 @@
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
 
     async def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#remove_lf_tags_from_resource)
         """
 
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
@@ -638,30 +626,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#revoke_permissions)
         """
 
     async def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
 
     async def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -686,15 +674,15 @@
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#start_transaction)
         """
 
     async def update_data_cells_filter(
-        self, *, TableData: DataCellsFilterUnionTypeDef
+        self, *, TableData: DataCellsFilterTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_data_cells_filter)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.pyi` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
+    BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterUnionTypeDef,
+    DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsUnionTypeDef,
+    DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -58,31 +58,31 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairUnionTypeDef,
-    LFTagUnionTypeDef,
+    LFTagPairTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
     TimestampTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -133,19 +133,15 @@
         """
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#exceptions)
         """
     async def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -156,24 +152,24 @@
         Allows a caller to assume an IAM role decorated as the SAML user specified in
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#assume_decorated_role_with_saml)
         """
     async def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_grant_permissions)
         """
     async def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_revoke_permissions)
         """
@@ -202,15 +198,15 @@
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#commit_transaction)
         """
     async def create_data_cells_filter(
-        self, *, TableData: DataCellsFilterUnionTypeDef
+        self, *, TableData: DataCellsFilterTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#create_data_cells_filter)
@@ -354,19 +350,15 @@
         """
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_query_statistics)
         """
     async def get_resource_lf_tags(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_resource_lf_tags)
         """
@@ -389,34 +381,34 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_table_objects)
         """
     async def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
     async def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_temporary_glue_table_credentials)
@@ -439,28 +431,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_units)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_work_units)
         """
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#grant_permissions)
         """
     async def list_data_cells_filter(
-        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_data_cells_filter)
         """
@@ -480,15 +472,15 @@
         """
     async def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceUnionTypeDef = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -537,15 +529,15 @@
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
     async def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#put_data_lake_settings)
@@ -561,60 +553,56 @@
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
     async def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#remove_lf_tags_from_resource)
         """
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#revoke_permissions)
         """
     async def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
     async def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -636,15 +624,15 @@
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#start_transaction)
         """
     async def update_data_cells_filter(
-        self, *, TableData: DataCellsFilterUnionTypeDef
+        self, *, TableData: DataCellsFilterTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_data_cells_filter)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.py` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ComparisonOperatorType",
     "DataLakeResourceTypeType",
     "FieldNameStringType",
     "GetWorkUnitsPaginatorName",
     "ListDataCellsFilterPaginatorName",
     "ListLFTagsPaginatorName",
@@ -40,15 +39,14 @@
     "LakeFormationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ComparisonOperatorType = Literal[
     "BEGINS_WITH", "BETWEEN", "CONTAINS", "EQ", "GE", "GT", "IN", "LE", "LT", "NE", "NOT_CONTAINS"
 ]
 DataLakeResourceTypeType = Literal[
     "CATALOG",
     "DATABASE",
     "DATA_LOCATION",
@@ -64,24 +62,27 @@
 ListLFTagsPaginatorName = Literal["list_lf_tags"]
 OptimizerTypeType = Literal["ALL", "COMPACTION", "GARBAGE_COLLECTION"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "ASSOCIATE",
     "CREATE_DATABASE",
+    "CREATE_LF_TAG",
     "CREATE_TABLE",
-    "CREATE_TAG",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DESCRIBE",
     "DROP",
+    "GRANT_WITH_LF_TAG_EXPRESSION",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 QueryStateStringType = Literal["ERROR", "EXPIRED", "FINISHED", "PENDING", "WORKUNITS_AVAILABLE"]
 ResourceShareTypeType = Literal["ALL", "FOREIGN"]
 ResourceTypeType = Literal["DATABASE", "TABLE"]
 SearchDatabasesByLFTagsPaginatorName = Literal["search_databases_by_lf_tags"]
 SearchTablesByLFTagsPaginatorName = Literal["search_tables_by_lf_tags"]
 TransactionStatusFilterType = Literal["ABORTED", "ACTIVE", "ALL", "COMMITTED", "COMPLETED"]
 TransactionStatusType = Literal["ABORTED", "ACTIVE", "COMMITTED", "COMMIT_IN_PROGRESS"]
@@ -98,14 +99,15 @@
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
@@ -201,14 +203,15 @@
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
@@ -287,26 +290,28 @@
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
@@ -460,26 +465,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.pyi` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ComparisonOperatorType",
     "DataLakeResourceTypeType",
     "FieldNameStringType",
     "GetWorkUnitsPaginatorName",
     "ListDataCellsFilterPaginatorName",
     "ListLFTagsPaginatorName",
@@ -39,14 +40,15 @@
     "LakeFormationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ComparisonOperatorType = Literal[
     "BEGINS_WITH", "BETWEEN", "CONTAINS", "EQ", "GE", "GT", "IN", "LE", "LT", "NE", "NOT_CONTAINS"
 ]
 DataLakeResourceTypeType = Literal[
     "CATALOG",
     "DATABASE",
     "DATA_LOCATION",
@@ -62,24 +64,27 @@
 ListLFTagsPaginatorName = Literal["list_lf_tags"]
 OptimizerTypeType = Literal["ALL", "COMPACTION", "GARBAGE_COLLECTION"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "ASSOCIATE",
     "CREATE_DATABASE",
+    "CREATE_LF_TAG",
     "CREATE_TABLE",
-    "CREATE_TAG",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DESCRIBE",
     "DROP",
+    "GRANT_WITH_LF_TAG_EXPRESSION",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 QueryStateStringType = Literal["ERROR", "EXPIRED", "FINISHED", "PENDING", "WORKUNITS_AVAILABLE"]
 ResourceShareTypeType = Literal["ALL", "FOREIGN"]
 ResourceTypeType = Literal["DATABASE", "TABLE"]
 SearchDatabasesByLFTagsPaginatorName = Literal["search_databases_by_lf_tags"]
 SearchTablesByLFTagsPaginatorName = Literal["search_tables_by_lf_tags"]
 TransactionStatusFilterType = Literal["ABORTED", "ACTIVE", "ALL", "COMMITTED", "COMPLETED"]
 TransactionStatusType = Literal["ABORTED", "ACTIVE", "COMMITTED", "COMMIT_IN_PROGRESS"]
@@ -96,14 +101,15 @@
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
@@ -199,14 +205,15 @@
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
@@ -285,26 +292,28 @@
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
@@ -458,26 +467,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.py` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagUnionTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
@@ -82,18 +82,15 @@
 class ListDataCellsFilterPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: TableResourceUnionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 
@@ -121,15 +118,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
@@ -140,15 +137,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.pyi` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagUnionTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
@@ -78,18 +78,15 @@
 class ListDataCellsFilterPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: TableResourceUnionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 class ListLFTagsPaginator(AioPaginator):
@@ -115,15 +112,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
@@ -133,15 +130,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.py` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lakeformation.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: LFTagPairTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,29 +33,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
-    "LFTagPairOutputTypeDef",
-    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
-    "RowFilterOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
@@ -78,50 +75,43 @@
     "PlanningStatisticsTypeDef",
     "TimestampTypeDef",
     "PartitionValueListTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
-    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
-    "LFTagOutputTypeDef",
-    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
     "TableObjectTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "ColumnLFTagTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "GetLFTagResponseTypeDef",
     "GetQueryStateResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsResponseTypeDef",
+    "ListLFTagsResponseTypeDef",
     "StartQueryPlanningResponseTypeDef",
     "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "PrincipalPermissionsOutputTypeDef",
-    "PrincipalPermissionsTypeDef",
-    "ColumnLFTagTypeDef",
     "LFTagErrorTypeDef",
-    "ListLFTagsResponseTypeDef",
-    "TableWithColumnsResourceOutputTypeDef",
+    "PrincipalPermissionsTypeDef",
     "TableWithColumnsResourceTypeDef",
-    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
@@ -130,68 +120,75 @@
     "GetQueryStatisticsResponseTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
-    "LFTagPolicyResourceOutputTypeDef",
-    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "LFTagUnionTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "TableResourceUnionTypeDef",
-    "DataLakeSettingsOutputTypeDef",
-    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
+    "DataLakeSettingsTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
-    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
-    "BatchPermissionsRequestEntryOutputTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
-    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
-    "BatchPermissionsRequestEntryUnionTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
 )
 
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -211,19 +208,17 @@
     "_OptionalAddObjectInputTypeDef",
     {
         "PartitionValues": Sequence[str],
     },
     total=False,
 )
 
-
 class AddObjectInputTypeDef(_RequiredAddObjectInputTypeDef, _OptionalAddObjectInputTypeDef):
     pass
 
-
 _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     {
         "SAMLAssertion": str,
         "RoleArn": str,
         "PrincipalArn": str,
     },
@@ -232,22 +227,20 @@
     "_OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     {
         "DurationSeconds": int,
     },
     total=False,
 )
 
-
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -272,42 +265,14 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
-
-ColumnWildcardOutputTypeDef = TypedDict(
-    "ColumnWildcardOutputTypeDef",
-    {
-        "ExcludedColumnNames": List[str],
-    },
-    total=False,
-)
-
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -330,30 +295,19 @@
     "_OptionalCreateLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
-
-RowFilterOutputTypeDef = TypedDict(
-    "RowFilterOutputTypeDef",
-    {
-        "FilterExpression": str,
-        "AllRowsWildcard": Dict[str, Any],
-    },
-    total=False,
-)
-
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -380,40 +334,36 @@
     "_OptionalDataLocationResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
-
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
     "_OptionalDatabaseResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DatabaseResourceTypeDef(_RequiredDatabaseResourceTypeDef, _OptionalDatabaseResourceTypeDef):
     pass
 
-
 DeleteDataCellsFilterRequestRequestTypeDef = TypedDict(
     "DeleteDataCellsFilterRequestRequestTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -431,21 +381,19 @@
     "_OptionalDeleteLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteLFTagRequestRequestTypeDef(
     _RequiredDeleteLFTagRequestRequestTypeDef, _OptionalDeleteLFTagRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteObjectInputTypeDef = TypedDict(
     "_RequiredDeleteObjectInputTypeDef",
     {
         "Uri": str,
     },
 )
 _OptionalDeleteObjectInputTypeDef = TypedDict(
@@ -453,40 +401,36 @@
     {
         "ETag": str,
         "PartitionValues": Sequence[str],
     },
     total=False,
 )
 
-
 class DeleteObjectInputTypeDef(
     _RequiredDeleteObjectInputTypeDef, _OptionalDeleteObjectInputTypeDef
 ):
     pass
 
-
 _RequiredVirtualObjectTypeDef = TypedDict(
     "_RequiredVirtualObjectTypeDef",
     {
         "Uri": str,
     },
 )
 _OptionalVirtualObjectTypeDef = TypedDict(
     "_OptionalVirtualObjectTypeDef",
     {
         "ETag": str,
     },
     total=False,
 )
 
-
 class VirtualObjectTypeDef(_RequiredVirtualObjectTypeDef, _OptionalVirtualObjectTypeDef):
     pass
 
-
 DeregisterResourceRequestRequestTypeDef = TypedDict(
     "DeregisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -592,43 +536,39 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetEffectivePermissionsForPathRequestRequestTypeDef(
     _RequiredGetEffectivePermissionsForPathRequestRequestTypeDef,
     _OptionalGetEffectivePermissionsForPathRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredGetLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalGetLFTagRequestRequestTypeDef = TypedDict(
     "_OptionalGetLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -688,52 +628,28 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class GetWorkUnitsRequestRequestTypeDef(
     _RequiredGetWorkUnitsRequestRequestTypeDef, _OptionalGetWorkUnitsRequestRequestTypeDef
 ):
     pass
 
-
 WorkUnitRangeTypeDef = TypedDict(
     "WorkUnitRangeTypeDef",
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -741,47 +657,17 @@
     "_OptionalLFTagKeyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
-
-LFTagOutputTypeDef = TypedDict(
-    "LFTagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
-
-
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -798,19 +684,17 @@
         "CatalogId": str,
         "Name": str,
         "TableWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
-
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -832,22 +716,20 @@
         "StorageOptimizerType": OptimizerTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTableStorageOptimizersRequestRequestTypeDef(
     _RequiredListTableStorageOptimizersRequestRequestTypeDef,
     _OptionalListTableStorageOptimizersRequestRequestTypeDef,
 ):
     pass
 
-
 StorageOptimizerTypeDef = TypedDict(
     "StorageOptimizerTypeDef",
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
@@ -889,44 +771,19 @@
         "UseServiceLinkedRole": bool,
         "RoleArn": str,
         "WithFederation": bool,
     },
     total=False,
 )
 
-
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-        "Name": str,
-        "TableWildcard": Dict[str, Any],
-    },
-    total=False,
-)
-
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -943,21 +800,19 @@
         "CatalogId": str,
         "TagValuesToDelete": Sequence[str],
         "TagValuesToAdd": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateLFTagRequestRequestTypeDef(
     _RequiredUpdateLFTagRequestRequestTypeDef, _OptionalUpdateLFTagRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "RoleArn": str,
         "ResourceArn": str,
     },
 )
@@ -965,21 +820,19 @@
     "_OptionalUpdateResourceRequestRequestTypeDef",
     {
         "WithFederation": bool,
     },
     total=False,
 )
 
-
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "StorageOptimizerConfig": Mapping[OptimizerTypeType, Mapping[str, str]],
     },
@@ -988,21 +841,28 @@
     "_OptionalUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairTypeDef],
+    },
+    total=False,
+)
 
 AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
@@ -1064,14 +924,23 @@
     "GetWorkUnitResultsResponseTypeDef",
     {
         "ResultStream": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartQueryPlanningResponseTypeDef = TypedDict(
     "StartQueryPlanningResponseTypeDef",
     {
         "QueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1092,104 +961,51 @@
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
-
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
-PrincipalPermissionsOutputTypeDef = TypedDict(
-    "PrincipalPermissionsOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
-    },
-    total=False,
-)
-
-PrincipalPermissionsTypeDef = TypedDict(
-    "PrincipalPermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": Sequence[PermissionType],
-    },
-    total=False,
-)
-
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
-    {
-        "Name": str,
-        "LFTags": List[LFTagPairOutputTypeDef],
-    },
-    total=False,
-)
-
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
-        "LFTag": LFTagPairOutputTypeDef,
+        "LFTag": LFTagPairTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
-    {
-        "LFTags": List[LFTagPairOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
+PrincipalPermissionsTypeDef = TypedDict(
+    "PrincipalPermissionsTypeDef",
     {
-        "CatalogId": str,
-        "ColumnNames": List[str],
-        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "Principal": DataLakePrincipalTypeDef,
+        "Permissions": List[PermissionType],
     },
     total=False,
 )
 
-
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1199,48 +1015,19 @@
         "CatalogId": str,
         "ColumnNames": Sequence[str],
         "ColumnWildcard": ColumnWildcardTypeDef,
     },
     total=False,
 )
 
-
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
-    {
-        "TableCatalogId": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
-        "RowFilter": RowFilterOutputTypeDef,
-        "ColumnNames": List[str],
-        "ColumnWildcard": ColumnWildcardOutputTypeDef,
-        "VersionId": str,
-    },
-    total=False,
-)
-
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1253,24 +1040,22 @@
         "ColumnNames": Sequence[str],
         "ColumnWildcard": ColumnWildcardTypeDef,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
-
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairOutputTypeDef],
+        "LFTags": List[LFTagPairTypeDef],
     },
     total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
@@ -1293,22 +1078,20 @@
     "_OptionalDeleteObjectsOnCancelRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteObjectsOnCancelRequestRequestTypeDef(
     _RequiredDeleteObjectsOnCancelRequestRequestTypeDef,
     _OptionalDeleteObjectsOnCancelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1375,21 +1158,19 @@
         "PartitionPredicate": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTableObjectsRequestRequestTypeDef(
     _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalQueryPlanningContextTypeDef = TypedDict(
@@ -1399,69 +1180,63 @@
         "QueryAsOfTime": TimestampTypeDef,
         "QueryParameters": Mapping[str, str],
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class QueryPlanningContextTypeDef(
     _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
 ):
     pass
 
-
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
-
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
     "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
     _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
 ):
     pass
 
-
 ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1474,60 +1249,120 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Expression": List[LFTagOutputTypeDef],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
 
-LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
-        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+):
+    pass
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+):
+    pass
 
-LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1557,61 +1392,30 @@
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
     total=False,
 )
 
-TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
-DataLakeSettingsOutputTypeDef = TypedDict(
-    "DataLakeSettingsOutputTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "Parameters": Mapping[str, str],
-        "TrustedResourceOwners": Sequence[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": Sequence[str],
-    },
-    total=False,
-)
-
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
-        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
+        "LFTagOnDatabase": List[LFTagPairTypeDef],
+        "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceOutputTypeDef,
-        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
-        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
+        "Table": TableResourceTypeDef,
+        "LFTagOnDatabase": List[LFTagPairTypeDef],
+        "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
@@ -1625,39 +1429,55 @@
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+    total=False,
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
+    },
+)
+
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
+        "DataCellsFilters": List[DataCellsFilterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
-    },
-)
-
-DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
@@ -1683,45 +1503,28 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
-
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
-        "Table": TableResourceOutputTypeDef,
-        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
-        "LFTag": LFTagKeyResourceOutputTypeDef,
-        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1729,217 +1532,81 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+GetTableObjectsResponseTypeDef = TypedDict(
+    "GetTableObjectsResponseTypeDef",
     {
+        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-):
-    pass
-
-
-GetTableObjectsResponseTypeDef = TypedDict(
-    "GetTableObjectsResponseTypeDef",
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
     {
-        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "DataLakeSettings": DataLakeSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_OptionalPutDataLakeSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
-
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceOutputTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-    },
-    total=False,
-)
-
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceOutputTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class AddLFTagsToResourceRequestRequestTypeDef(
     _RequiredAddLFTagsToResourceRequestRequestTypeDef,
     _OptionalAddLFTagsToResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchPermissionsRequestEntryTypeDef = TypedDict(
     "_RequiredBatchPermissionsRequestEntryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalBatchPermissionsRequestEntryTypeDef = TypedDict(
@@ -1949,21 +1616,19 @@
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
-
 class BatchPermissionsRequestEntryTypeDef(
     _RequiredBatchPermissionsRequestEntryTypeDef, _OptionalBatchPermissionsRequestEntryTypeDef
 ):
     pass
 
-
 _RequiredGetResourceLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceLFTagsRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
     },
 )
 _OptionalGetResourceLFTagsRequestRequestTypeDef = TypedDict(
@@ -1971,21 +1636,19 @@
     {
         "CatalogId": str,
         "ShowAssignedLFTags": bool,
     },
     total=False,
 )
 
-
 class GetResourceLFTagsRequestRequestTypeDef(
     _RequiredGetResourceLFTagsRequestRequestTypeDef, _OptionalGetResourceLFTagsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredGrantPermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1995,59 +1658,66 @@
     {
         "CatalogId": str,
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
-
 class GrantPermissionsRequestRequestTypeDef(
     _RequiredGrantPermissionsRequestRequestTypeDef, _OptionalGrantPermissionsRequestRequestTypeDef
 ):
     pass
 
-
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "Principal": DataLakePrincipalTypeDef,
         "ResourceType": DataLakeResourceTypeType,
         "Resource": ResourceTypeDef,
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
-
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -2057,30 +1727,68 @@
     {
         "CatalogId": str,
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
-
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
+_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+    },
+)
+_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchGrantPermissionsRequestRequestTypeDef(
+    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
+    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
+):
+    pass
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
-        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
+        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+    },
+)
+_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchRevokePermissionsRequestRequestTypeDef(
+    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
+    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
+):
+    pass
+
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2091,17 +1799,14 @@
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPermissionsRequestEntryUnionTypeDef = Union[
-    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
-]
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2109,50 +1814,7 @@
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
-    },
-)
-_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchGrantPermissionsRequestRequestTypeDef(
-    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
-    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
-    },
-)
-_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchRevokePermissionsRequestRequestTypeDef(
-    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
-    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.pyi` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lakeformation.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: LFTagPairTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,28 +33,27 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
-    "LFTagPairOutputTypeDef",
-    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
-    "RowFilterOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
@@ -77,50 +76,43 @@
     "PlanningStatisticsTypeDef",
     "TimestampTypeDef",
     "PartitionValueListTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
-    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
-    "LFTagOutputTypeDef",
-    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
     "TableObjectTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "ColumnLFTagTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "GetLFTagResponseTypeDef",
     "GetQueryStateResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsResponseTypeDef",
+    "ListLFTagsResponseTypeDef",
     "StartQueryPlanningResponseTypeDef",
     "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "PrincipalPermissionsOutputTypeDef",
-    "PrincipalPermissionsTypeDef",
-    "ColumnLFTagTypeDef",
     "LFTagErrorTypeDef",
-    "ListLFTagsResponseTypeDef",
-    "TableWithColumnsResourceOutputTypeDef",
+    "PrincipalPermissionsTypeDef",
     "TableWithColumnsResourceTypeDef",
-    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
@@ -129,68 +121,77 @@
     "GetQueryStatisticsResponseTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
-    "LFTagPolicyResourceOutputTypeDef",
-    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "LFTagUnionTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "TableResourceUnionTypeDef",
-    "DataLakeSettingsOutputTypeDef",
-    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
+    "DataLakeSettingsTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
-    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
-    "BatchPermissionsRequestEntryOutputTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
-    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
-    "BatchPermissionsRequestEntryUnionTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
 )
 
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -210,17 +211,19 @@
     "_OptionalAddObjectInputTypeDef",
     {
         "PartitionValues": Sequence[str],
     },
     total=False,
 )
 
+
 class AddObjectInputTypeDef(_RequiredAddObjectInputTypeDef, _OptionalAddObjectInputTypeDef):
     pass
 
+
 _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     {
         "SAMLAssertion": str,
         "RoleArn": str,
         "PrincipalArn": str,
     },
@@ -229,20 +232,22 @@
     "_OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     {
         "DurationSeconds": int,
     },
     total=False,
 )
 
+
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
+
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -267,40 +272,14 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
-ColumnWildcardOutputTypeDef = TypedDict(
-    "ColumnWildcardOutputTypeDef",
-    {
-        "ExcludedColumnNames": List[str],
-    },
-    total=False,
-)
-
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -323,27 +302,20 @@
     "_OptionalCreateLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
-RowFilterOutputTypeDef = TypedDict(
-    "RowFilterOutputTypeDef",
-    {
-        "FilterExpression": str,
-        "AllRowsWildcard": Dict[str, Any],
-    },
-    total=False,
-)
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
@@ -371,36 +343,40 @@
     "_OptionalDataLocationResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
     "_OptionalDatabaseResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DatabaseResourceTypeDef(_RequiredDatabaseResourceTypeDef, _OptionalDatabaseResourceTypeDef):
     pass
 
+
 DeleteDataCellsFilterRequestRequestTypeDef = TypedDict(
     "DeleteDataCellsFilterRequestRequestTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -418,19 +394,21 @@
     "_OptionalDeleteLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteLFTagRequestRequestTypeDef(
     _RequiredDeleteLFTagRequestRequestTypeDef, _OptionalDeleteLFTagRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteObjectInputTypeDef = TypedDict(
     "_RequiredDeleteObjectInputTypeDef",
     {
         "Uri": str,
     },
 )
 _OptionalDeleteObjectInputTypeDef = TypedDict(
@@ -438,36 +416,40 @@
     {
         "ETag": str,
         "PartitionValues": Sequence[str],
     },
     total=False,
 )
 
+
 class DeleteObjectInputTypeDef(
     _RequiredDeleteObjectInputTypeDef, _OptionalDeleteObjectInputTypeDef
 ):
     pass
 
+
 _RequiredVirtualObjectTypeDef = TypedDict(
     "_RequiredVirtualObjectTypeDef",
     {
         "Uri": str,
     },
 )
 _OptionalVirtualObjectTypeDef = TypedDict(
     "_OptionalVirtualObjectTypeDef",
     {
         "ETag": str,
     },
     total=False,
 )
 
+
 class VirtualObjectTypeDef(_RequiredVirtualObjectTypeDef, _OptionalVirtualObjectTypeDef):
     pass
 
+
 DeregisterResourceRequestRequestTypeDef = TypedDict(
     "DeregisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -573,39 +555,43 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetEffectivePermissionsForPathRequestRequestTypeDef(
     _RequiredGetEffectivePermissionsForPathRequestRequestTypeDef,
     _OptionalGetEffectivePermissionsForPathRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredGetLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalGetLFTagRequestRequestTypeDef = TypedDict(
     "_OptionalGetLFTagRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
+
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -665,48 +651,30 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class GetWorkUnitsRequestRequestTypeDef(
     _RequiredGetWorkUnitsRequestRequestTypeDef, _OptionalGetWorkUnitsRequestRequestTypeDef
 ):
     pass
 
+
 WorkUnitRangeTypeDef = TypedDict(
     "WorkUnitRangeTypeDef",
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -714,42 +682,18 @@
     "_OptionalLFTagKeyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
-LFTagOutputTypeDef = TypedDict(
-    "LFTagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
 
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -767,17 +711,19 @@
         "CatalogId": str,
         "Name": str,
         "TableWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
+
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -799,20 +745,22 @@
         "StorageOptimizerType": OptimizerTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTableStorageOptimizersRequestRequestTypeDef(
     _RequiredListTableStorageOptimizersRequestRequestTypeDef,
     _OptionalListTableStorageOptimizersRequestRequestTypeDef,
 ):
     pass
 
+
 StorageOptimizerTypeDef = TypedDict(
     "StorageOptimizerTypeDef",
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
@@ -854,39 +802,20 @@
         "UseServiceLinkedRole": bool,
         "RoleArn": str,
         "WithFederation": bool,
     },
     total=False,
 )
 
+
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-        "Name": str,
-        "TableWildcard": Dict[str, Any],
-    },
-    total=False,
-)
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
 
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
@@ -904,19 +833,21 @@
         "CatalogId": str,
         "TagValuesToDelete": Sequence[str],
         "TagValuesToAdd": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateLFTagRequestRequestTypeDef(
     _RequiredUpdateLFTagRequestRequestTypeDef, _OptionalUpdateLFTagRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceRequestRequestTypeDef",
     {
         "RoleArn": str,
         "ResourceArn": str,
     },
 )
@@ -924,19 +855,21 @@
     "_OptionalUpdateResourceRequestRequestTypeDef",
     {
         "WithFederation": bool,
     },
     total=False,
 )
 
+
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "StorageOptimizerConfig": Mapping[OptimizerTypeType, Mapping[str, str]],
     },
@@ -945,20 +878,31 @@
     "_OptionalUpdateTableStorageOptimizerRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
+
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairTypeDef],
+    },
+    total=False,
+)
+
 AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
         "Expiration": datetime,
@@ -1019,14 +963,23 @@
     "GetWorkUnitResultsResponseTypeDef",
     {
         "ResultStream": StreamingBody,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartQueryPlanningResponseTypeDef = TypedDict(
     "StartQueryPlanningResponseTypeDef",
     {
         "QueryId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1047,100 +1000,53 @@
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
+
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
-PrincipalPermissionsOutputTypeDef = TypedDict(
-    "PrincipalPermissionsOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
-    },
-    total=False,
-)
-
-PrincipalPermissionsTypeDef = TypedDict(
-    "PrincipalPermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Permissions": Sequence[PermissionType],
-    },
-    total=False,
-)
-
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
-    {
-        "Name": str,
-        "LFTags": List[LFTagPairOutputTypeDef],
-    },
-    total=False,
-)
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
-        "LFTag": LFTagPairOutputTypeDef,
+        "LFTag": LFTagPairTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
-    {
-        "LFTags": List[LFTagPairOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
+PrincipalPermissionsTypeDef = TypedDict(
+    "PrincipalPermissionsTypeDef",
     {
-        "CatalogId": str,
-        "ColumnNames": List[str],
-        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "Principal": DataLakePrincipalTypeDef,
+        "Permissions": List[PermissionType],
     },
     total=False,
 )
 
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1150,43 +1056,20 @@
         "CatalogId": str,
         "ColumnNames": Sequence[str],
         "ColumnWildcard": ColumnWildcardTypeDef,
     },
     total=False,
 )
 
+
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
-    {
-        "TableCatalogId": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
-        "RowFilter": RowFilterOutputTypeDef,
-        "ColumnNames": List[str],
-        "ColumnWildcard": ColumnWildcardOutputTypeDef,
-        "VersionId": str,
-    },
-    total=False,
-)
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
 
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
@@ -1200,22 +1083,24 @@
         "ColumnNames": Sequence[str],
         "ColumnWildcard": ColumnWildcardTypeDef,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
+
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairOutputTypeDef],
+        "LFTags": List[LFTagPairTypeDef],
     },
     total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
@@ -1238,20 +1123,22 @@
     "_OptionalDeleteObjectsOnCancelRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteObjectsOnCancelRequestRequestTypeDef(
     _RequiredDeleteObjectsOnCancelRequestRequestTypeDef,
     _OptionalDeleteObjectsOnCancelRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1318,19 +1205,21 @@
         "PartitionPredicate": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTableObjectsRequestRequestTypeDef(
     _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalQueryPlanningContextTypeDef = TypedDict(
@@ -1340,63 +1229,69 @@
         "QueryAsOfTime": TimestampTypeDef,
         "QueryParameters": Mapping[str, str],
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class QueryPlanningContextTypeDef(
     _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
 ):
     pass
 
+
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
+
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
     "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
     _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
 ):
     pass
 
+
 ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1409,56 +1304,130 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Expression": List[LFTagOutputTypeDef],
+        "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
+
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
-LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "CatalogId": str,
     },
     total=False,
 )
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
 ):
     pass
 
-LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
+
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+):
+    pass
+
+
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1488,61 +1457,30 @@
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
     total=False,
 )
 
-TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
-DataLakeSettingsOutputTypeDef = TypedDict(
-    "DataLakeSettingsOutputTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
-        "Parameters": Mapping[str, str],
-        "TrustedResourceOwners": Sequence[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": Sequence[str],
-    },
-    total=False,
-)
-
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
-        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
+        "LFTagOnDatabase": List[LFTagPairTypeDef],
+        "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceOutputTypeDef,
-        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
-        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
+        "Table": TableResourceTypeDef,
+        "LFTagOnDatabase": List[LFTagPairTypeDef],
+        "LFTagsOnTable": List[LFTagPairTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
@@ -1556,39 +1494,55 @@
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+    total=False,
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
+    },
+)
+
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
+        "DataCellsFilters": List[DataCellsFilterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
-    },
-)
-
-DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
@@ -1614,43 +1568,30 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
+
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
-        "Table": TableResourceOutputTypeDef,
-        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
-        "LFTag": LFTagKeyResourceOutputTypeDef,
-        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1658,203 +1599,85 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-):
-    pass
-
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+GetTableObjectsResponseTypeDef = TypedDict(
+    "GetTableObjectsResponseTypeDef",
     {
+        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-):
-    pass
-
-GetTableObjectsResponseTypeDef = TypedDict(
-    "GetTableObjectsResponseTypeDef",
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
     {
-        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "DataLakeSettings": DataLakeSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_OptionalPutDataLakeSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceOutputTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-    },
-    total=False,
-)
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceOutputTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class AddLFTagsToResourceRequestRequestTypeDef(
     _RequiredAddLFTagsToResourceRequestRequestTypeDef,
     _OptionalAddLFTagsToResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchPermissionsRequestEntryTypeDef = TypedDict(
     "_RequiredBatchPermissionsRequestEntryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalBatchPermissionsRequestEntryTypeDef = TypedDict(
@@ -1864,19 +1687,21 @@
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
+
 class BatchPermissionsRequestEntryTypeDef(
     _RequiredBatchPermissionsRequestEntryTypeDef, _OptionalBatchPermissionsRequestEntryTypeDef
 ):
     pass
 
+
 _RequiredGetResourceLFTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceLFTagsRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
     },
 )
 _OptionalGetResourceLFTagsRequestRequestTypeDef = TypedDict(
@@ -1884,19 +1709,21 @@
     {
         "CatalogId": str,
         "ShowAssignedLFTags": bool,
     },
     total=False,
 )
 
+
 class GetResourceLFTagsRequestRequestTypeDef(
     _RequiredGetResourceLFTagsRequestRequestTypeDef, _OptionalGetResourceLFTagsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredGrantPermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1906,55 +1733,70 @@
     {
         "CatalogId": str,
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
+
 class GrantPermissionsRequestRequestTypeDef(
     _RequiredGrantPermissionsRequestRequestTypeDef, _OptionalGrantPermissionsRequestRequestTypeDef
 ):
     pass
 
+
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "Principal": DataLakePrincipalTypeDef,
         "ResourceType": DataLakeResourceTypeType,
         "Resource": ResourceTypeDef,
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+    total=False,
+)
+
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
+
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1964,28 +1806,74 @@
     {
         "CatalogId": str,
         "PermissionsWithGrantOption": Sequence[PermissionType],
     },
     total=False,
 )
 
+
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+    },
+)
+_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class BatchGrantPermissionsRequestRequestTypeDef(
+    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
+    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
-        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
+        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+    },
+)
+_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class BatchRevokePermissionsRequestRequestTypeDef(
+    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
+    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
+):
+    pass
+
+
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1996,17 +1884,14 @@
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPermissionsRequestEntryUnionTypeDef = Union[
-    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
-]
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2014,47 +1899,7 @@
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
-    },
-)
-_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchGrantPermissionsRequestRequestTypeDef(
-    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
-    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
-    },
-)
-_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchRevokePermissionsRequestRequestTypeDef(
-    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
-    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt` & `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

