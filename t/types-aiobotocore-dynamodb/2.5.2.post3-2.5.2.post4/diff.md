# Comparing `tmp/types-aiobotocore-dynamodb-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.2.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post3.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post4.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.2.post3.tar` & `types-aiobotocore-dynamodb-2.5.2.post4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodb-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-08-02 14:52:12.241600 types-aiobotocore-dynamodb-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodb-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.237600 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50026 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49957 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   104451 2023-08-02 14:36:53.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104312 2023-08-02 14:36:52.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.241600 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.651961 types-aiobotocore-dynamodb-2.5.2.post4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-08-04 12:00:47.647961 types-aiobotocore-dynamodb-2.5.2.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.651961 types-aiobotocore-dynamodb-2.5.2.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.639961 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49966 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49897 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24190 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   110199 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110060 2023-08-04 11:44:15.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:12.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-04 11:44:13.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.647961 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/LICENSE` & `types-aiobotocore-dynamodb-2.5.2.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/setup.py` & `types-aiobotocore-dynamodb-2.5.2.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.2.post3",
+    version="2.5.2.post4",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post3")
+    print("2.5.2.post4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexUnionTypeDef,
+    GlobalSecondaryIndexTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsUnionTypeDef,
-    KeysAndAttributesUnionTypeDef,
+    InputFormatOptionsTypeDef,
+    KeysAndAttributesTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -105,15 +105,15 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersUnionTypeDef,
+    TableCreationParametersTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
@@ -122,15 +122,15 @@
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestUnionTypeDef,
+    WriteRequestTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -212,29 +212,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
 
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_get_item)
         """
 
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
@@ -279,15 +279,15 @@
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
@@ -565,17 +565,17 @@
         """
 
     async def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: TableCreationParametersUnionTypeDef,
+        TableCreationParameters: TableCreationParametersTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
+        InputFormatOptions: InputFormatOptionsTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
@@ -712,15 +712,15 @@
 
     async def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
@@ -733,15 +733,15 @@
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexUnionTypeDef,
+    GlobalSecondaryIndexTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsUnionTypeDef,
-    KeysAndAttributesUnionTypeDef,
+    InputFormatOptionsTypeDef,
+    KeysAndAttributesTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -105,15 +105,15 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersUnionTypeDef,
+    TableCreationParametersTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
@@ -122,15 +122,15 @@
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestUnionTypeDef,
+    WriteRequestTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -206,28 +206,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_get_item)
         """
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
@@ -267,15 +267,15 @@
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
@@ -529,17 +529,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_item)
         """
     async def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: TableCreationParametersUnionTypeDef,
+        TableCreationParameters: TableCreationParametersTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
+        InputFormatOptions: InputFormatOptionsTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
@@ -666,15 +666,15 @@
         """
     async def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
@@ -686,15 +686,15 @@
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     SelectType,
 )
 from .type_defs import (
-    ConditionTypeDef,
+    ConditionTableTypeDef,
     ListBackupsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    QueryOutputTypeDef,
-    ScanOutputTypeDef,
+    QueryOutputTableTypeDef,
+    ScanOutputTableTypeDef,
     TableAttributeValueTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
@@ -131,26 +131,26 @@
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[QueryOutputTypeDef]:
+    ) -> AsyncIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 
 class ScanPaginator(AioPaginator):
@@ -162,23 +162,23 @@
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ScanOutputTypeDef]:
+    ) -> AsyncIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     SelectType,
 )
 from .type_defs import (
-    ConditionTypeDef,
+    ConditionTableTypeDef,
     ListBackupsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    QueryOutputTypeDef,
-    ScanOutputTypeDef,
+    QueryOutputTableTypeDef,
+    ScanOutputTableTypeDef,
     TableAttributeValueTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
@@ -125,26 +125,26 @@
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[QueryOutputTypeDef]:
+    ) -> AsyncIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(AioPaginator):
     """
@@ -155,23 +155,23 @@
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ScanOutputTypeDef]:
+    ) -> AsyncIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,48 +31,48 @@
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueUpdateTypeDef,
-    BatchGetItemOutputTypeDef,
-    BatchWriteItemOutputTypeDef,
+    AttributeValueUpdateTableTypeDef,
+    BatchGetItemOutputServiceResourceTypeDef,
+    BatchWriteItemOutputServiceResourceTypeDef,
     BillingModeSummaryResponseTypeDef,
     ConditionBaseImportTypeDef,
-    ConditionTypeDef,
-    DeleteItemOutputTypeDef,
-    DeleteTableOutputTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemOutputTypeDef,
-    GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexUnionTypeDef,
-    GlobalSecondaryIndexUpdateTypeDef,
-    KeysAndAttributesUnionTypeDef,
+    ConditionTableTypeDef,
+    DeleteItemOutputTableTypeDef,
+    DeleteTableOutputTableTypeDef,
+    ExpectedAttributeValueTableTypeDef,
+    GetItemOutputTableTypeDef,
+    GlobalSecondaryIndexDescriptionTableTypeDef,
+    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUpdateTableTypeDef,
+    KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     ProvisionedThroughputTypeDef,
-    PutItemOutputTypeDef,
-    QueryOutputTypeDef,
+    PutItemOutputTableTypeDef,
+    QueryOutputTableTypeDef,
     ReplicaDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
     RestoreSummaryResponseTypeDef,
-    ScanOutputTypeDef,
+    ScanOutputTableTypeDef,
     SSEDescriptionResponseTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationResponseTypeDef,
     StreamSpecificationTypeDef,
     TableAttributeValueTypeDef,
     TableClassSummaryResponseTypeDef,
     TagTypeDef,
-    UpdateItemOutputTypeDef,
-    WriteRequestUnionTypeDef,
+    UpdateItemOutputTableTypeDef,
+    WriteRequestServiceResourceTypeDef,
 )
 
 try:
     from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
     from builtins import object as BatchWriter
 try:
@@ -170,16 +170,16 @@
     creation_date_time: Awaitable[datetime]
     provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
     billing_mode_summary: Awaitable[BillingModeSummaryResponseTypeDef]
-    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTypeDef]]
-    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTypeDef]]
+    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
+    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
     stream_specification: Awaitable[StreamSpecificationResponseTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
     replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
     restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
     sse_description: Awaitable[SSEDescriptionResponseTypeDef]
@@ -197,35 +197,35 @@
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
         """
 
-    async def delete(self) -> DeleteTableOutputTypeDef:
+    async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
 
     async def delete_item(
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> DeleteItemOutputTypeDef:
+    ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
 
@@ -242,15 +242,15 @@
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTypeDef:
+    ) -> GetItemOutputTableTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_item-method)
         """
@@ -264,23 +264,23 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableload-method)
         """
 
     async def put_item(
         self,
         *,
         Item: Mapping[str, TableAttributeValueTypeDef],
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> PutItemOutputTypeDef:
+    ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
 
@@ -288,26 +288,26 @@
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> QueryOutputTypeDef:
+    ) -> QueryOutputTableTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablequery-method)
         """
@@ -324,41 +324,41 @@
     async def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTypeDef:
+    ) -> ScanOutputTableTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablescan-method)
         """
 
     async def update(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
@@ -369,25 +369,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate-method)
         """
 
     async def update_item(
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> UpdateItemOutputTypeDef:
+    ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -432,32 +432,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
 
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputTypeDef:
+    ) -> BatchGetItemOutputServiceResourceTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
 
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputTypeDef:
+    ) -> BatchWriteItemOutputServiceResourceTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
@@ -465,15 +465,15 @@
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,48 +31,48 @@
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueUpdateTypeDef,
-    BatchGetItemOutputTypeDef,
-    BatchWriteItemOutputTypeDef,
+    AttributeValueUpdateTableTypeDef,
+    BatchGetItemOutputServiceResourceTypeDef,
+    BatchWriteItemOutputServiceResourceTypeDef,
     BillingModeSummaryResponseTypeDef,
     ConditionBaseImportTypeDef,
-    ConditionTypeDef,
-    DeleteItemOutputTypeDef,
-    DeleteTableOutputTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemOutputTypeDef,
-    GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexUnionTypeDef,
-    GlobalSecondaryIndexUpdateTypeDef,
-    KeysAndAttributesUnionTypeDef,
+    ConditionTableTypeDef,
+    DeleteItemOutputTableTypeDef,
+    DeleteTableOutputTableTypeDef,
+    ExpectedAttributeValueTableTypeDef,
+    GetItemOutputTableTypeDef,
+    GlobalSecondaryIndexDescriptionTableTypeDef,
+    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUpdateTableTypeDef,
+    KeysAndAttributesServiceResourceTypeDef,
     KeySchemaElementTypeDef,
-    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexDescriptionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     ProvisionedThroughputTypeDef,
-    PutItemOutputTypeDef,
-    QueryOutputTypeDef,
+    PutItemOutputTableTypeDef,
+    QueryOutputTableTypeDef,
     ReplicaDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
     RestoreSummaryResponseTypeDef,
-    ScanOutputTypeDef,
+    ScanOutputTableTypeDef,
     SSEDescriptionResponseTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationResponseTypeDef,
     StreamSpecificationTypeDef,
     TableAttributeValueTypeDef,
     TableClassSummaryResponseTypeDef,
     TagTypeDef,
-    UpdateItemOutputTypeDef,
-    WriteRequestUnionTypeDef,
+    UpdateItemOutputTableTypeDef,
+    WriteRequestServiceResourceTypeDef,
 )
 
 try:
     from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
     from builtins import object as BatchWriter
 try:
@@ -161,16 +161,16 @@
     creation_date_time: Awaitable[datetime]
     provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
     billing_mode_summary: Awaitable[BillingModeSummaryResponseTypeDef]
-    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTypeDef]]
-    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTypeDef]]
+    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
+    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
     stream_specification: Awaitable[StreamSpecificationResponseTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
     replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
     restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
     sse_description: Awaitable[SSEDescriptionResponseTypeDef]
@@ -187,34 +187,34 @@
     ) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
         """
-    async def delete(self) -> DeleteTableOutputTypeDef:
+    async def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
     async def delete_item(
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> DeleteItemOutputTypeDef:
+    ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
     async def get_available_subresources(self) -> Sequence[str]:
@@ -229,15 +229,15 @@
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTypeDef:
+    ) -> GetItemOutputTableTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_item-method)
         """
@@ -249,49 +249,49 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableload-method)
         """
     async def put_item(
         self,
         *,
         Item: Mapping[str, TableAttributeValueTypeDef],
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> PutItemOutputTypeDef:
+    ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
     async def query(
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> QueryOutputTypeDef:
+    ) -> QueryOutputTableTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablequery-method)
         """
@@ -306,40 +306,40 @@
     async def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTypeDef:
+    ) -> ScanOutputTableTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablescan-method)
         """
     async def update(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
@@ -349,25 +349,25 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate-method)
         """
     async def update_item(
         self,
         *,
         Key: Mapping[str, TableAttributeValueTypeDef],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
-    ) -> UpdateItemOutputTypeDef:
+    ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -406,46 +406,46 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputTypeDef:
+    ) -> BatchGetItemOutputServiceResourceTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputTypeDef:
+    ) -> BatchWriteItemOutputServiceResourceTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,42 +60,41 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
+    "TableAttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTypeDef",
-    "TableAttributeValueTypeDef",
     "BatchStatementErrorTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
-    "ProjectionTypeDef",
+    "ProjectionTableTypeDef",
     "ProvisionedThroughputTypeDef",
+    "ProjectionTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
-    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
@@ -113,15 +112,14 @@
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
     "ExportSummaryTypeDef",
     "TimestampTypeDef",
-    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
@@ -144,58 +142,64 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "ItemCollectionMetricsTypeDef",
+    "ItemResponseTypeDef",
     "UniversalAttributeValueTypeDef",
+    "AttributeValueUpdateTableTypeDef",
+    "ConditionTableTypeDef",
+    "DeleteRequestServiceResourceTypeDef",
+    "ExpectedAttributeValueTableTypeDef",
+    "GetItemInputTableGetItemTypeDef",
+    "ItemCollectionMetricsServiceResourceTypeDef",
+    "ItemCollectionMetricsTableTypeDef",
+    "KeysAndAttributesServiceResourceTypeDef",
+    "PutRequestServiceResourceTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTypeDef",
-    "DeleteRequestOutputTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "ItemCollectionMetricsTypeDef",
-    "ItemResponseTypeDef",
-    "KeysAndAttributesOutputTypeDef",
-    "PutRequestOutputTypeDef",
     "BatchStatementResponseTypeDef",
     "ConsumedCapacityTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexTypeDef",
-    "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    "CreateGlobalSecondaryIndexActionTableTypeDef",
     "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
+    "CreateGlobalSecondaryIndexActionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
+    "LocalSecondaryIndexTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
     "GlobalTableTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
     "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "ListBackupsInputRequestTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
-    "GlobalSecondaryIndexOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
@@ -211,105 +215,110 @@
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
+    "PutItemInputTablePutItemTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    "WriteRequestServiceResourceTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "WriteRequestOutputTypeDef",
     "BatchExecuteStatementOutputTypeDef",
-    "BatchGetItemOutputTypeDef",
+    "BatchGetItemOutputServiceResourceTypeDef",
+    "DeleteItemOutputTableTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
+    "GetItemOutputTableTypeDef",
     "GetItemOutputTypeDef",
+    "PutItemOutputTableTypeDef",
     "PutItemOutputTypeDef",
+    "QueryOutputTableTypeDef",
     "QueryOutputTypeDef",
+    "ScanOutputTableTypeDef",
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
+    "UpdateItemOutputTableTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
-    "TableCreationParametersTypeDef",
+    "GlobalSecondaryIndexUpdateTableTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
+    "TableCreationParametersTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
+    "RestoreTableFromBackupInputRequestTypeDef",
+    "RestoreTableToPointInTimeInputRequestTypeDef",
     "ListGlobalTablesOutputTypeDef",
     "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
-    "InputFormatOptionsUnionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "GlobalSecondaryIndexUnionTypeDef",
-    "TableCreationParametersOutputTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputRequestTypeDef",
-    "QueryInputTableQueryTypeDef",
     "ScanInputRequestTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ScanInputTableScanTypeDef",
     "DeleteItemInputRequestTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputRequestTypeDef",
-    "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputRequestTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
     "TransactGetItemTypeDef",
-    "KeysAndAttributesUnionTypeDef",
+    "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemOutputTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "BatchWriteItemOutputServiceResourceTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BatchWriteItemOutputTypeDef",
+    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
+    "BackupDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
+    "TableDescriptionTableTypeDef",
     "TableDescriptionTypeDef",
     "ReplicationGroupUpdateTypeDef",
-    "CreateTableInputRequestTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "RestoreTableFromBackupInputRequestTypeDef",
-    "RestoreTableToPointInTimeInputRequestTypeDef",
-    "ImportTableDescriptionTypeDef",
-    "TableCreationParametersUnionTypeDef",
-    "BackupDescriptionTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchGetItemInputRequestTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "WriteRequestUnionTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemOutputTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "DescribeImportOutputTypeDef",
+    "ImportTableOutputTypeDef",
+    "DeleteBackupOutputTypeDef",
+    "DescribeBackupOutputTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
     "UpdateTableInputRequestTypeDef",
     "UpdateTableInputTableUpdateTypeDef",
-    "DescribeImportOutputTypeDef",
-    "ImportTableOutputTypeDef",
-    "DeleteBackupOutputTypeDef",
-    "DescribeBackupOutputTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
@@ -357,14 +366,30 @@
         "L": Sequence[Any],
         "NULL": bool,
         "BOOL": bool,
     },
     total=False,
 )
 
+TableAttributeValueTypeDef = Union[
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
@@ -373,22 +398,20 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
-
 class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
 ):
     pass
 
-
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -397,22 +420,20 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
-
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-
 _RequiredBackupDetailsTypeDef = TypedDict(
     "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
@@ -424,19 +445,17 @@
     {
         "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
     total=False,
 )
 
-
 class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
     pass
 
-
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
@@ -446,30 +465,14 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
-TableAttributeValueTypeDef = Union[
-    bytes,
-    bytearray,
-    str,
-    int,
-    Decimal,
-    bool,
-    Set[int],
-    Set[Decimal],
-    Set[str],
-    Set[bytes],
-    Set[bytearray],
-    Sequence[Any],
-    Mapping[str, Any],
-    None,
-]
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
     total=False,
@@ -527,31 +530,40 @@
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
 
-ProjectionTypeDef = TypedDict(
-    "ProjectionTypeDef",
+ProjectionTableTypeDef = TypedDict(
+    "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
+        "NonKeyAttributes": List[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
 )
 
+ProjectionTypeDef = TypedDict(
+    "ProjectionTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": Sequence[str],
+    },
+    total=False,
+)
+
 ReplicaTypeDef = TypedDict(
     "ReplicaTypeDef",
     {
         "RegionName": str,
     },
     total=False,
 )
@@ -591,43 +603,32 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CsvOptionsOutputTypeDef = TypedDict(
-    "CsvOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-        "HeaderList": List[str],
-    },
-    total=False,
-)
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": Sequence[str],
+        "HeaderList": List[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -687,22 +688,20 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
     total=False,
@@ -832,23 +831,14 @@
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
 )
 
 TimestampTypeDef = Union[datetime, str]
-ProjectionOutputTypeDef = TypedDict(
-    "ProjectionOutputTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
-    },
-    total=False,
-)
-
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
@@ -868,19 +858,17 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
-
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
@@ -954,21 +942,19 @@
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
-
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
@@ -993,19 +979,17 @@
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
     },
     total=False,
 )
 
-
 class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
     pass
 
-
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
@@ -1048,22 +1032,20 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
-
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-
 ArchivalSummaryResponseTypeDef = TypedDict(
     "ArchivalSummaryResponseTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1174,14 +1156,31 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ItemCollectionMetricsTypeDef = TypedDict(
+    "ItemCollectionMetricsTypeDef",
+    {
+        "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
+        "SizeEstimateRangeGB": List[float],
+    },
+    total=False,
+)
+
+ItemResponseTypeDef = TypedDict(
+    "ItemResponseTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 UniversalAttributeValueTypeDef = Union[
     AttributeValueTypeDef,
     bytes,
     bytearray,
     str,
     int,
     Decimal,
@@ -1191,70 +1190,56 @@
     Set[str],
     Set[bytes],
     Set[bytearray],
     Sequence[Any],
     Mapping[str, Any],
     None,
 ]
-AutoScalingPolicyDescriptionTypeDef = TypedDict(
-    "AutoScalingPolicyDescriptionTypeDef",
+AttributeValueUpdateTableTypeDef = TypedDict(
+    "AttributeValueUpdateTableTypeDef",
     {
-        "PolicyName": str,
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
-        ),
+        "Value": TableAttributeValueTypeDef,
+        "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_RequiredAutoScalingPolicyUpdateTypeDef",
+_RequiredConditionTableTypeDef = TypedDict(
+    "_RequiredConditionTableTypeDef",
     {
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
-        ),
+        "ComparisonOperator": ComparisonOperatorType,
     },
 )
-_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_OptionalAutoScalingPolicyUpdateTypeDef",
+_OptionalConditionTableTypeDef = TypedDict(
+    "_OptionalConditionTableTypeDef",
     {
-        "PolicyName": str,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-
-class AutoScalingPolicyUpdateTypeDef(
-    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
-):
+class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
-
-CreateBackupOutputTypeDef = TypedDict(
-    "CreateBackupOutputTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTypeDef = TypedDict(
-    "ListBackupsOutputTypeDef",
+DeleteRequestServiceResourceTypeDef = TypedDict(
+    "DeleteRequestServiceResourceTypeDef",
     {
-        "BackupSummaries": List[BackupSummaryTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
 
-DeleteRequestOutputTypeDef = TypedDict(
-    "DeleteRequestOutputTypeDef",
+ExpectedAttributeValueTableTypeDef = TypedDict(
+    "ExpectedAttributeValueTableTypeDef",
     {
-        "Key": Dict[str, TableAttributeValueTypeDef],
+        "Value": TableAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[str, TableAttributeValueTypeDef],
     },
@@ -1267,75 +1252,122 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
-
-ItemCollectionMetricsTypeDef = TypedDict(
-    "ItemCollectionMetricsTypeDef",
+ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
+    "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
-ItemResponseTypeDef = TypedDict(
-    "ItemResponseTypeDef",
+ItemCollectionMetricsTableTypeDef = TypedDict(
+    "ItemCollectionMetricsTableTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
+        "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
-_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesOutputTypeDef",
+_RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
-        "Keys": List[Dict[str, TableAttributeValueTypeDef]],
+        "Keys": Sequence[Mapping[str, TableAttributeValueTypeDef]],
     },
 )
-_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesOutputTypeDef",
+_OptionalKeysAndAttributesServiceResourceTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesServiceResourceTypeDef",
     {
-        "AttributesToGet": List[str],
+        "AttributesToGet": Sequence[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
+        "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+class KeysAndAttributesServiceResourceTypeDef(
+    _RequiredKeysAndAttributesServiceResourceTypeDef,
+    _OptionalKeysAndAttributesServiceResourceTypeDef,
+):
+    pass
+
+PutRequestServiceResourceTypeDef = TypedDict(
+    "PutRequestServiceResourceTypeDef",
+    {
+        "Item": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+
+AutoScalingPolicyDescriptionTypeDef = TypedDict(
+    "AutoScalingPolicyDescriptionTypeDef",
+    {
+        "PolicyName": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_RequiredAutoScalingPolicyUpdateTypeDef",
+    {
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
+        ),
+    },
+)
+_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_OptionalAutoScalingPolicyUpdateTypeDef",
+    {
+        "PolicyName": str,
+    },
+    total=False,
+)
 
-class KeysAndAttributesOutputTypeDef(
-    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
+CreateBackupOutputTypeDef = TypedDict(
+    "CreateBackupOutputTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-PutRequestOutputTypeDef = TypedDict(
-    "PutRequestOutputTypeDef",
+ListBackupsOutputTypeDef = TypedDict(
+    "ListBackupsOutputTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "BackupSummaries": List[BackupSummaryTypeDef],
+        "LastEvaluatedBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Item": Dict[str, AttributeValueTypeDef],
     },
     total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
@@ -1360,36 +1392,94 @@
     "_OptionalContinuousBackupsDescriptionTypeDef",
     {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
     total=False,
 )
 
-
 class ContinuousBackupsDescriptionTypeDef(
     _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
 ):
     pass
 
-
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexTypeDef = TypedDict(
-    "LocalSecondaryIndexTypeDef",
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTableTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+    total=False,
+)
+
+_RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
+    "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "Projection": ProjectionTableTypeDef,
+    },
+)
+_OptionalCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
+    "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
+
+class CreateGlobalSecondaryIndexActionTableTypeDef(
+    _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
+    _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
+):
+    pass
+
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
+    total=False,
+)
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
+UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
+    "UpdateGlobalSecondaryIndexActionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
@@ -1401,21 +1491,30 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
 
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
@@ -1425,54 +1524,48 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
-
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
     {
-        "TableName": str,
-        "TableId": str,
+        "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "Projection": ProjectionTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
+    total=False,
 )
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
     {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
     },
     total=False,
 )
 
-
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
-
-
-UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
-    "UpdateGlobalSecondaryIndexActionTypeDef",
+LocalSecondaryIndexTypeDef = TypedDict(
+    "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
     },
 )
 
 CreateGlobalTableInputRequestTypeDef = TypedDict(
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
@@ -1508,21 +1601,19 @@
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
-
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1532,22 +1623,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-InputFormatOptionsOutputTypeDef = TypedDict(
-    "InputFormatOptionsOutputTypeDef",
-    {
-        "Csv": CsvOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -1617,44 +1700,40 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
-
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1685,98 +1764,55 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
-
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
-
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "Limit": int,
         "TimeRangeLowerBound": TimestampTypeDef,
         "TimeRangeUpperBound": TimestampTypeDef,
         "ExclusiveStartBackupArn": str,
         "BackupType": BackupTypeFilterType,
     },
     total=False,
 )
 
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexOutputTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-)
-_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexOutputTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
-
-class GlobalSecondaryIndexOutputTypeDef(
-    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
-):
-    pass
-
-
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
+GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
+        "Projection": ProjectionTableTypeDef,
+        "IndexStatus": IndexStatusType,
+        "Backfilling": bool,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
     total=False,
 )
 
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-    total=False,
-)
-
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
+        "Projection": ProjectionTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
@@ -1828,22 +1864,20 @@
     "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
     _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
 ):
     pass
 
-
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
@@ -1884,21 +1918,19 @@
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
-
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
         "ConditionExpression": str,
     },
@@ -1909,38 +1941,34 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
-
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
     "_OptionalConditionTypeDef",
     {
         "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
-
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
@@ -1958,19 +1986,17 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -1981,21 +2007,19 @@
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
-
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Exists": bool,
         "ComparisonOperator": ComparisonOperatorType,
         "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
@@ -2018,21 +2042,19 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
     },
 )
@@ -2041,19 +2063,17 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
-
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[Mapping[str, UniversalAttributeValueTypeDef]],
     },
 )
 _OptionalKeysAndAttributesTypeDef = TypedDict(
@@ -2063,42 +2083,38 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
-
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
     "_OptionalParameterizedStatementTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
-
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
@@ -2116,19 +2132,17 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
-
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "UpdateExpression": str,
         "TableName": str,
     },
@@ -2140,18 +2154,235 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "KeyConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+    },
+    total=False,
+)
+
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Key": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
+):
+    pass
+
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
+    {
+        "Item": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
+):
+    pass
+
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "Key": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTableTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+WriteRequestServiceResourceTypeDef = TypedDict(
+    "WriteRequestServiceResourceTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceTypeDef,
+    },
+    total=False,
+)
 
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
@@ -2169,110 +2400,154 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
-    },
-    total=False,
-)
-
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetItemOutputTypeDef = TypedDict(
-    "BatchGetItemOutputTypeDef",
+BatchGetItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteItemOutputTableTypeDef = TypedDict(
+    "DeleteItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
-        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetItemOutputTableTypeDef = TypedDict(
+    "GetItemOutputTableTypeDef",
+    {
+        "Item": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutItemOutputTableTypeDef = TypedDict(
+    "PutItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+QueryOutputTableTypeDef = TypedDict(
+    "QueryOutputTableTypeDef",
+    {
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Count": int,
+        "ScannedCount": int,
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
+        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Count": int,
+        "ScannedCount": int,
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScanOutputTableTypeDef = TypedDict(
+    "ScanOutputTableTypeDef",
+    {
         "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
-        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
@@ -2288,18 +2563,28 @@
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateItemOutputTableTypeDef = TypedDict(
+    "UpdateItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
@@ -2314,50 +2599,182 @@
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
+    "GlobalSecondaryIndexUpdateTableTypeDef",
+    {
+        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
+        "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
+        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+    },
+    total=False,
+)
+
+GlobalSecondaryIndexUpdateTypeDef = TypedDict(
+    "GlobalSecondaryIndexUpdateTypeDef",
+    {
+        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
+        "Create": CreateGlobalSecondaryIndexActionTypeDef,
+        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
-
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
+    {
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+    total=False,
+)
 
-GlobalSecondaryIndexUpdateTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTypeDef",
+_RequiredCreateTableInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTableInputRequestTypeDef",
     {
-        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
-        "Create": CreateGlobalSecondaryIndexActionTypeDef,
-        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTableInputRequestTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateTableInputRequestTypeDef(
+    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+):
+    pass
+
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+        "BackupArn": str,
+    },
+)
+_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+class RestoreTableFromBackupInputRequestTypeDef(
+    _RequiredRestoreTableFromBackupInputRequestTypeDef,
+    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+):
+    pass
+
+_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+    },
+)
+_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "SourceTableArn": str,
+        "SourceTableName": str,
+        "UseLatestRestorableTime": bool,
+        "RestoreDateTime": TimestampTypeDef,
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+class RestoreTableToPointInTimeInputRequestTypeDef(
+    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
+    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2392,22 +2809,20 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -2417,72 +2832,28 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
-
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-
-InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
-GlobalSecondaryIndexUnionTypeDef = Union[
-    GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef
-]
-_RequiredTableCreationParametersOutputTypeDef = TypedDict(
-    "_RequiredTableCreationParametersOutputTypeDef",
-    {
-        "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
-    },
-)
-_OptionalTableCreationParametersOutputTypeDef = TypedDict(
-    "_OptionalTableCreationParametersOutputTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class TableCreationParametersOutputTypeDef(
-    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
-):
-    pass
-
-
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2498,57 +2869,20 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -2570,44 +2904,19 @@
         "KeyConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
-
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": ConditionBaseImportTypeDef,
-        "KeyConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -2628,75 +2937,17 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "ConsistentRead": bool,
-    },
-    total=False,
-)
-
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
@@ -2711,49 +2962,19 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
-
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[str, TableAttributeValueTypeDef],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
-
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
@@ -2768,49 +2989,19 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
-
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
-    {
-        "Item": Mapping[str, TableAttributeValueTypeDef],
-    },
-)
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
-
-
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
@@ -2827,59 +3018,55 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
+TransactGetItemTypeDef = TypedDict(
+    "TransactGetItemTypeDef",
+    {
+        "Get": GetTypeDef,
+    },
+)
 
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputRequestTypeDef",
     {
-        "Key": Mapping[str, TableAttributeValueTypeDef],
+        "RequestItems": Mapping[str, KeysAndAttributesTypeDef],
     },
 )
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputRequestTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
-
-TransactGetItemTypeDef = TypedDict(
-    "TransactGetItemTypeDef",
+BatchGetItemOutputTypeDef = TypedDict(
+    "BatchGetItemOutputTypeDef",
     {
-        "Get": GetTypeDef,
+        "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KeysAndAttributesUnionTypeDef = Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -2887,21 +3074,19 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
-
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
     total=False,
@@ -2914,14 +3099,45 @@
         "Put": PutTypeDef,
         "Delete": DeleteTypeDef,
         "Update": UpdateTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -2943,22 +3159,20 @@
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
 ):
     pass
 
-
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -2975,22 +3189,20 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -3007,30 +3219,44 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
     },
+    total=False,
 )
 
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
@@ -3043,33 +3269,71 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
-
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+    total=False,
+)
 
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
     total=False,
 )
 
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
+    {
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTypeDef],
+        "RestoreSummary": RestoreSummaryTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+        "ArchivalSummary": ArchivalSummaryTypeDef,
+        "TableClassSummary": TableClassSummaryTypeDef,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "TableStatus": TableStatusType,
@@ -3102,238 +3366,63 @@
         "Create": CreateReplicationGroupMemberActionTypeDef,
         "Update": UpdateReplicationGroupMemberActionTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateTableInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTableInputRequestTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-
-class CreateTableInputRequestTypeDef(
-    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
-):
-    pass
-
-
-_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-        "BackupArn": str,
-    },
-)
-_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreTableFromBackupInputRequestTypeDef(
-    _RequiredRestoreTableFromBackupInputRequestTypeDef,
-    _OptionalRestoreTableFromBackupInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-    },
-)
-_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "SourceTableArn": str,
-        "SourceTableName": str,
-        "UseLatestRestorableTime": bool,
-        "RestoreDateTime": TimestampTypeDef,
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreTableToPointInTimeInputRequestTypeDef(
-    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
-    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersOutputTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
-
-TableCreationParametersUnionTypeDef = Union[
-    TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
-]
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
     },
 )
 _OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
-
-_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputRequestTypeDef",
+_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputRequestTypeDef",
     {
-        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+        "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
-_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputRequestTypeDef",
+_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
+class BatchWriteItemInputRequestTypeDef(
+    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
-    },
-)
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
-    pass
-
-
-WriteRequestUnionTypeDef = Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
 _OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
@@ -3342,21 +3431,19 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
-
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -3384,21 +3471,19 @@
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaSettingsDescriptionTypeDef(
     _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
 ):
     pass
 
-
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -3408,21 +3493,19 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
-
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
-
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -3434,20 +3517,50 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
-
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+DescribeImportOutputTypeDef = TypedDict(
+    "DescribeImportOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportTableOutputTypeDef = TypedDict(
+    "ImportTableOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupOutputTypeDef = TypedDict(
+    "DeleteBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupOutputTypeDef = TypedDict(
+    "DescribeBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3465,14 +3578,22 @@
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
+    {
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3535,114 +3656,35 @@
         "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-
 class UpdateTableInputRequestTypeDef(
     _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
 ):
     pass
 
-
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
         "StreamSpecification": StreamSpecificationTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
         "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-DescribeImportOutputTypeDef = TypedDict(
-    "DescribeImportOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportTableOutputTypeDef = TypedDict(
-    "ImportTableOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupOutputTypeDef = TypedDict(
-    "DeleteBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupOutputTypeDef = TypedDict(
-    "DescribeBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputRequestTypeDef",
-    {
-        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
-    },
-)
-_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputRequestTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-    },
-    total=False,
-)
-
-
-class BatchWriteItemInputRequestTypeDef(
-    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
-):
-    pass
-
-
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
-    },
-)
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-    },
-    total=False,
-)
-
-
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-):
-    pass
-
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
@@ -3679,22 +3721,20 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -3709,22 +3749,20 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
-
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
-
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,41 +60,42 @@
 else:
     from typing_extensions import TypedDict
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
+
 __all__ = (
     "ResponseMetadataTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
+    "TableAttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTypeDef",
-    "TableAttributeValueTypeDef",
     "BatchStatementErrorTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
-    "ProjectionTypeDef",
+    "ProjectionTableTypeDef",
     "ProvisionedThroughputTypeDef",
+    "ProjectionTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
-    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
     "DeleteReplicaActionTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
@@ -112,15 +113,14 @@
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
     "ExportSummaryTypeDef",
     "TimestampTypeDef",
-    "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
@@ -143,58 +143,64 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "ItemCollectionMetricsTypeDef",
+    "ItemResponseTypeDef",
     "UniversalAttributeValueTypeDef",
+    "AttributeValueUpdateTableTypeDef",
+    "ConditionTableTypeDef",
+    "DeleteRequestServiceResourceTypeDef",
+    "ExpectedAttributeValueTableTypeDef",
+    "GetItemInputTableGetItemTypeDef",
+    "ItemCollectionMetricsServiceResourceTypeDef",
+    "ItemCollectionMetricsTableTypeDef",
+    "KeysAndAttributesServiceResourceTypeDef",
+    "PutRequestServiceResourceTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTypeDef",
-    "DeleteRequestOutputTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "ItemCollectionMetricsTypeDef",
-    "ItemResponseTypeDef",
-    "KeysAndAttributesOutputTypeDef",
-    "PutRequestOutputTypeDef",
     "BatchStatementResponseTypeDef",
     "ConsumedCapacityTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "LocalSecondaryIndexTypeDef",
-    "CreateGlobalSecondaryIndexActionTypeDef",
-    "GlobalSecondaryIndexTypeDef",
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    "CreateGlobalSecondaryIndexActionTableTypeDef",
     "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
+    "CreateGlobalSecondaryIndexActionTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexTypeDef",
+    "LocalSecondaryIndexDescriptionTypeDef",
+    "LocalSecondaryIndexInfoTypeDef",
+    "LocalSecondaryIndexTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
     "GlobalTableTypeDef",
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
     "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "ListBackupsInputRequestTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
-    "GlobalSecondaryIndexOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTypeDef",
-    "LocalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
@@ -210,105 +216,110 @@
     "GetItemInputRequestTypeDef",
     "GetTypeDef",
     "KeysAndAttributesTypeDef",
     "ParameterizedStatementTypeDef",
     "PutRequestTypeDef",
     "PutTypeDef",
     "UpdateTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
+    "PutItemInputTablePutItemTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    "WriteRequestServiceResourceTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "WriteRequestOutputTypeDef",
     "BatchExecuteStatementOutputTypeDef",
-    "BatchGetItemOutputTypeDef",
+    "BatchGetItemOutputServiceResourceTypeDef",
+    "DeleteItemOutputTableTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
+    "GetItemOutputTableTypeDef",
     "GetItemOutputTypeDef",
+    "PutItemOutputTableTypeDef",
     "PutItemOutputTypeDef",
+    "QueryOutputTableTypeDef",
     "QueryOutputTypeDef",
+    "ScanOutputTableTypeDef",
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
+    "UpdateItemOutputTableTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
-    "TableCreationParametersTypeDef",
+    "GlobalSecondaryIndexUpdateTableTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
+    "TableCreationParametersTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
+    "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
+    "RestoreTableFromBackupInputRequestTypeDef",
+    "RestoreTableToPointInTimeInputRequestTypeDef",
     "ListGlobalTablesOutputTypeDef",
     "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
-    "InputFormatOptionsUnionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "GlobalSecondaryIndexUnionTypeDef",
-    "TableCreationParametersOutputTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
-    "QueryInputQueryPaginateTypeDef",
     "QueryInputRequestTypeDef",
-    "QueryInputTableQueryTypeDef",
     "ScanInputRequestTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ScanInputTableScanTypeDef",
     "DeleteItemInputRequestTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputRequestTypeDef",
-    "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputRequestTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
     "TransactGetItemTypeDef",
-    "KeysAndAttributesUnionTypeDef",
+    "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemOutputTypeDef",
     "ExecuteTransactionInputRequestTypeDef",
     "WriteRequestTypeDef",
     "TransactWriteItemTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    "BatchWriteItemOutputServiceResourceTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
-    "BatchWriteItemOutputTypeDef",
+    "ImportTableDescriptionTypeDef",
     "ImportTableInputRequestTypeDef",
+    "BackupDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
+    "TableDescriptionTableTypeDef",
     "TableDescriptionTypeDef",
     "ReplicationGroupUpdateTypeDef",
-    "CreateTableInputRequestTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "RestoreTableFromBackupInputRequestTypeDef",
-    "RestoreTableToPointInTimeInputRequestTypeDef",
-    "ImportTableDescriptionTypeDef",
-    "TableCreationParametersUnionTypeDef",
-    "BackupDescriptionTypeDef",
     "TransactGetItemsInputRequestTypeDef",
-    "BatchGetItemInputRequestTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "WriteRequestUnionTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemOutputTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
+    "DescribeImportOutputTypeDef",
+    "ImportTableOutputTypeDef",
+    "DeleteBackupOutputTypeDef",
+    "DescribeBackupOutputTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
+    "DeleteTableOutputTableTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
     "UpdateTableInputRequestTypeDef",
     "UpdateTableInputTableUpdateTypeDef",
-    "DescribeImportOutputTypeDef",
-    "ImportTableOutputTypeDef",
-    "DeleteBackupOutputTypeDef",
-    "DescribeBackupOutputTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
@@ -356,14 +367,30 @@
         "L": Sequence[Any],
         "NULL": bool,
         "BOOL": bool,
     },
     total=False,
 )
 
+TableAttributeValueTypeDef = Union[
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
@@ -372,20 +399,22 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
+
 class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
 ):
     pass
 
+
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -394,20 +423,22 @@
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
     },
     total=False,
 )
 
+
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
+
 _RequiredBackupDetailsTypeDef = TypedDict(
     "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
@@ -419,17 +450,19 @@
     {
         "BackupSizeBytes": int,
         "BackupExpiryDateTime": datetime,
     },
     total=False,
 )
 
+
 class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
     pass
 
+
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
@@ -439,30 +472,14 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
-TableAttributeValueTypeDef = Union[
-    bytes,
-    bytearray,
-    str,
-    int,
-    Decimal,
-    bool,
-    Set[int],
-    Set[Decimal],
-    Set[str],
-    Set[bytes],
-    Set[bytearray],
-    Sequence[Any],
-    Mapping[str, Any],
-    None,
-]
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
     total=False,
@@ -520,31 +537,40 @@
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
 
-ProjectionTypeDef = TypedDict(
-    "ProjectionTypeDef",
+ProjectionTableTypeDef = TypedDict(
+    "ProjectionTableTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
+        "NonKeyAttributes": List[str],
     },
     total=False,
 )
 
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
 )
 
+ProjectionTypeDef = TypedDict(
+    "ProjectionTypeDef",
+    {
+        "ProjectionType": ProjectionTypeType,
+        "NonKeyAttributes": Sequence[str],
+    },
+    total=False,
+)
+
 ReplicaTypeDef = TypedDict(
     "ReplicaTypeDef",
     {
         "RegionName": str,
     },
     total=False,
 )
@@ -584,41 +610,34 @@
     "_OptionalStreamSpecificationTypeDef",
     {
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
+
 class StreamSpecificationTypeDef(
     _RequiredStreamSpecificationTypeDef, _OptionalStreamSpecificationTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CsvOptionsOutputTypeDef = TypedDict(
-    "CsvOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-        "HeaderList": List[str],
-    },
-    total=False,
-)
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
-        "HeaderList": Sequence[str],
+        "HeaderList": List[str],
     },
     total=False,
 )
 
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
@@ -678,20 +697,22 @@
     "_OptionalDescribeContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class DescribeContributorInsightsInputRequestTypeDef(
     _RequiredDescribeContributorInsightsInputRequestTypeDef,
     _OptionalDescribeContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
     total=False,
@@ -821,23 +842,14 @@
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
 )
 
 TimestampTypeDef = Union[datetime, str]
-ProjectionOutputTypeDef = TypedDict(
-    "ProjectionOutputTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
-    },
-    total=False,
-)
-
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
@@ -857,17 +869,19 @@
     {
         "S3BucketOwner": str,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class S3BucketSourceTypeDef(_RequiredS3BucketSourceTypeDef, _OptionalS3BucketSourceTypeDef):
     pass
 
+
 KinesisStreamingDestinationInputRequestTypeDef = TypedDict(
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
@@ -941,19 +955,21 @@
     "_OptionalListTagsOfResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
+
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
@@ -978,17 +994,19 @@
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
     },
     total=False,
 )
 
+
 class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
     pass
 
+
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
@@ -1031,20 +1049,22 @@
     "_OptionalUpdateContributorInsightsInputRequestTypeDef",
     {
         "IndexName": str,
     },
     total=False,
 )
 
+
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
+
 ArchivalSummaryResponseTypeDef = TypedDict(
     "ArchivalSummaryResponseTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1155,14 +1175,31 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ItemCollectionMetricsTypeDef = TypedDict(
+    "ItemCollectionMetricsTypeDef",
+    {
+        "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
+        "SizeEstimateRangeGB": List[float],
+    },
+    total=False,
+)
+
+ItemResponseTypeDef = TypedDict(
+    "ItemResponseTypeDef",
+    {
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 UniversalAttributeValueTypeDef = Union[
     AttributeValueTypeDef,
     bytes,
     bytearray,
     str,
     int,
     Decimal,
@@ -1172,68 +1209,58 @@
     Set[str],
     Set[bytes],
     Set[bytearray],
     Sequence[Any],
     Mapping[str, Any],
     None,
 ]
-AutoScalingPolicyDescriptionTypeDef = TypedDict(
-    "AutoScalingPolicyDescriptionTypeDef",
+AttributeValueUpdateTableTypeDef = TypedDict(
+    "AttributeValueUpdateTableTypeDef",
     {
-        "PolicyName": str,
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
-        ),
+        "Value": TableAttributeValueTypeDef,
+        "Action": AttributeActionType,
     },
     total=False,
 )
 
-_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_RequiredAutoScalingPolicyUpdateTypeDef",
+_RequiredConditionTableTypeDef = TypedDict(
+    "_RequiredConditionTableTypeDef",
     {
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
-        ),
+        "ComparisonOperator": ComparisonOperatorType,
     },
 )
-_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_OptionalAutoScalingPolicyUpdateTypeDef",
+_OptionalConditionTableTypeDef = TypedDict(
+    "_OptionalConditionTableTypeDef",
     {
-        "PolicyName": str,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-class AutoScalingPolicyUpdateTypeDef(
-    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
-):
+
+class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
-CreateBackupOutputTypeDef = TypedDict(
-    "CreateBackupOutputTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ListBackupsOutputTypeDef = TypedDict(
-    "ListBackupsOutputTypeDef",
+DeleteRequestServiceResourceTypeDef = TypedDict(
+    "DeleteRequestServiceResourceTypeDef",
     {
-        "BackupSummaries": List[BackupSummaryTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
 
-DeleteRequestOutputTypeDef = TypedDict(
-    "DeleteRequestOutputTypeDef",
+ExpectedAttributeValueTableTypeDef = TypedDict(
+    "ExpectedAttributeValueTableTypeDef",
     {
-        "Key": Dict[str, TableAttributeValueTypeDef],
+        "Value": TableAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[str, TableAttributeValueTypeDef],
     },
@@ -1246,71 +1273,128 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
-ItemCollectionMetricsTypeDef = TypedDict(
-    "ItemCollectionMetricsTypeDef",
+
+ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
+    "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
-ItemResponseTypeDef = TypedDict(
-    "ItemResponseTypeDef",
+ItemCollectionMetricsTableTypeDef = TypedDict(
+    "ItemCollectionMetricsTableTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
+        "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
-_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesOutputTypeDef",
+_RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesServiceResourceTypeDef",
     {
-        "Keys": List[Dict[str, TableAttributeValueTypeDef]],
+        "Keys": Sequence[Mapping[str, TableAttributeValueTypeDef]],
     },
 )
-_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesOutputTypeDef",
+_OptionalKeysAndAttributesServiceResourceTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesServiceResourceTypeDef",
     {
-        "AttributesToGet": List[str],
+        "AttributesToGet": Sequence[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
+        "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-class KeysAndAttributesOutputTypeDef(
-    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+
+class KeysAndAttributesServiceResourceTypeDef(
+    _RequiredKeysAndAttributesServiceResourceTypeDef,
+    _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-PutRequestOutputTypeDef = TypedDict(
-    "PutRequestOutputTypeDef",
+
+PutRequestServiceResourceTypeDef = TypedDict(
+    "PutRequestServiceResourceTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Item": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+
+AutoScalingPolicyDescriptionTypeDef = TypedDict(
+    "AutoScalingPolicyDescriptionTypeDef",
+    {
+        "PolicyName": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_RequiredAutoScalingPolicyUpdateTypeDef",
+    {
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
+        ),
+    },
+)
+_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_OptionalAutoScalingPolicyUpdateTypeDef",
+    {
+        "PolicyName": str,
+    },
+    total=False,
+)
+
+
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
+):
+    pass
+
+
+CreateBackupOutputTypeDef = TypedDict(
+    "CreateBackupOutputTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBackupsOutputTypeDef = TypedDict(
+    "ListBackupsOutputTypeDef",
+    {
+        "BackupSummaries": List[BackupSummaryTypeDef],
+        "LastEvaluatedBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Item": Dict[str, AttributeValueTypeDef],
     },
     total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
@@ -1335,34 +1419,100 @@
     "_OptionalContinuousBackupsDescriptionTypeDef",
     {
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
     total=False,
 )
 
+
 class ContinuousBackupsDescriptionTypeDef(
     _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
 ):
     pass
 
+
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexTypeDef = TypedDict(
-    "LocalSecondaryIndexTypeDef",
+LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTableTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTableTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+    total=False,
+)
+
+_RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
+    "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
-        "Projection": ProjectionTypeDef,
+        "Projection": ProjectionTableTypeDef,
+    },
+)
+_OptionalCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
+    "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateGlobalSecondaryIndexActionTableTypeDef(
+    _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
+    _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
+):
+    pass
+
+
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
+    total=False,
+)
+
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
+
+UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
+    "UpdateGlobalSecondaryIndexActionTypeDef",
+    {
+        "IndexName": str,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
 
 _RequiredCreateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "_RequiredCreateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
@@ -1374,20 +1524,33 @@
     "_OptionalCreateGlobalSecondaryIndexActionTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class CreateGlobalSecondaryIndexActionTypeDef(
     _RequiredCreateGlobalSecondaryIndexActionTypeDef,
     _OptionalCreateGlobalSecondaryIndexActionTypeDef,
 ):
     pass
 
+
+GlobalSecondaryIndexInfoTypeDef = TypedDict(
+    "GlobalSecondaryIndexInfoTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -1396,50 +1559,50 @@
     "_OptionalGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
+
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
-_RequiredSourceTableDetailsTypeDef = TypedDict(
-    "_RequiredSourceTableDetailsTypeDef",
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
     {
-        "TableName": str,
-        "TableId": str,
+        "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "Projection": ProjectionTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
+    total=False,
 )
-_OptionalSourceTableDetailsTypeDef = TypedDict(
-    "_OptionalSourceTableDetailsTypeDef",
+
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
     {
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
     },
     total=False,
 )
 
-class SourceTableDetailsTypeDef(
-    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
-):
-    pass
-
-UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
-    "UpdateGlobalSecondaryIndexActionTypeDef",
+LocalSecondaryIndexTypeDef = TypedDict(
+    "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "Projection": ProjectionTypeDef,
     },
 )
 
 CreateGlobalTableInputRequestTypeDef = TypedDict(
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
@@ -1475,19 +1638,21 @@
     "_OptionalReplicaGlobalSecondaryIndexTypeDef",
     {
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
+
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1497,22 +1662,14 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-InputFormatOptionsOutputTypeDef = TypedDict(
-    "InputFormatOptionsOutputTypeDef",
-    {
-        "Csv": CsvOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
@@ -1582,40 +1739,44 @@
     "_OptionalDescribeTableInputTableExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableExistsWaitTypeDef(
     _RequiredDescribeTableInputTableExistsWaitTypeDef,
     _OptionalDescribeTableInputTableExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDescribeTableInputTableNotExistsWaitTypeDef = TypedDict(
     "_OptionalDescribeTableInputTableNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTableInputTableNotExistsWaitTypeDef(
     _RequiredDescribeTableInputTableNotExistsWaitTypeDef,
     _OptionalDescribeTableInputTableNotExistsWaitTypeDef,
 ):
     pass
 
+
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1646,94 +1807,57 @@
         "S3SseAlgorithm": S3SseAlgorithmType,
         "S3SseKmsKeyId": str,
         "ExportFormat": ExportFormatType,
     },
     total=False,
 )
 
+
 class ExportTableToPointInTimeInputRequestTypeDef(
     _RequiredExportTableToPointInTimeInputRequestTypeDef,
     _OptionalExportTableToPointInTimeInputRequestTypeDef,
 ):
     pass
 
+
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "Limit": int,
         "TimeRangeLowerBound": TimestampTypeDef,
         "TimeRangeUpperBound": TimestampTypeDef,
         "ExclusiveStartBackupArn": str,
         "BackupType": BackupTypeFilterType,
     },
     total=False,
 )
 
-GlobalSecondaryIndexInfoTypeDef = TypedDict(
-    "GlobalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexOutputTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-)
-_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexOutputTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-    },
-    total=False,
-)
-
-class GlobalSecondaryIndexOutputTypeDef(
-    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
-):
-    pass
-
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
+GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
+    "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
+        "Projection": ProjectionTableTypeDef,
+        "IndexStatus": IndexStatusType,
+        "Backfilling": bool,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
     total=False,
 )
 
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-    total=False,
-)
-
 GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
-        "Projection": ProjectionOutputTypeDef,
+        "Projection": ProjectionTypeDef,
         "IndexStatus": IndexStatusType,
         "Backfilling": bool,
         "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
         "IndexSizeBytes": int,
         "ItemCount": int,
         "IndexArn": str,
     },
@@ -1785,20 +1909,22 @@
     "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
     _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
 ):
     pass
 
+
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
         "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
@@ -1839,19 +1965,21 @@
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
+
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
+
 _RequiredConditionCheckTypeDef = TypedDict(
     "_RequiredConditionCheckTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
         "ConditionExpression": str,
     },
@@ -1862,34 +1990,38 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
     pass
 
+
 _RequiredConditionTypeDef = TypedDict(
     "_RequiredConditionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
 )
 _OptionalConditionTypeDef = TypedDict(
     "_OptionalConditionTypeDef",
     {
         "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
     pass
 
+
 DeleteRequestTypeDef = TypedDict(
     "DeleteRequestTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
@@ -1907,17 +2039,19 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
+
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalExecuteStatementInputRequestTypeDef = TypedDict(
@@ -1928,19 +2062,21 @@
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
+
 ExpectedAttributeValueTypeDef = TypedDict(
     "ExpectedAttributeValueTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Exists": bool,
         "ComparisonOperator": ComparisonOperatorType,
         "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
@@ -1963,19 +2099,21 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetItemInputRequestTypeDef(
     _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTypeDef = TypedDict(
     "_RequiredGetTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
     },
 )
@@ -1984,17 +2122,19 @@
     {
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
+
 _RequiredKeysAndAttributesTypeDef = TypedDict(
     "_RequiredKeysAndAttributesTypeDef",
     {
         "Keys": Sequence[Mapping[str, UniversalAttributeValueTypeDef]],
     },
 )
 _OptionalKeysAndAttributesTypeDef = TypedDict(
@@ -2004,38 +2144,42 @@
         "ConsistentRead": bool,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
+
 class KeysAndAttributesTypeDef(
     _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
+
 _RequiredParameterizedStatementTypeDef = TypedDict(
     "_RequiredParameterizedStatementTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
     "_OptionalParameterizedStatementTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
+
 PutRequestTypeDef = TypedDict(
     "PutRequestTypeDef",
     {
         "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
@@ -2053,17 +2197,19 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
+
 _RequiredUpdateTypeDef = TypedDict(
     "_RequiredUpdateTypeDef",
     {
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "UpdateExpression": str,
         "TableName": str,
     },
@@ -2075,17 +2221,250 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
+
 class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "KeyConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+    },
+    total=False,
+)
+
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Key": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
+):
+    pass
+
+
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
+    {
+        "Item": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
+):
+    pass
+
+
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "Key": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+    {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTableTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+
+WriteRequestServiceResourceTypeDef = TypedDict(
+    "WriteRequestServiceResourceTypeDef",
+    {
+        "PutRequest": PutRequestServiceResourceTypeDef,
+        "DeleteRequest": DeleteRequestServiceResourceTypeDef,
+    },
+    total=False,
+)
+
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
@@ -2102,110 +2481,154 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
-    },
-    total=False,
-)
-
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetItemOutputTypeDef = TypedDict(
-    "BatchGetItemOutputTypeDef",
+BatchGetItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteItemOutputTableTypeDef = TypedDict(
+    "DeleteItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
-        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetItemOutputTableTypeDef = TypedDict(
+    "GetItemOutputTableTypeDef",
+    {
+        "Item": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Item": Dict[str, AttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutItemOutputTableTypeDef = TypedDict(
+    "PutItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+QueryOutputTableTypeDef = TypedDict(
+    "QueryOutputTableTypeDef",
+    {
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Count": int,
+        "ScannedCount": int,
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
+        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Count": int,
+        "ScannedCount": int,
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScanOutputTableTypeDef = TypedDict(
+    "ScanOutputTableTypeDef",
+    {
         "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
-        "Items": List[Dict[str, TableAttributeValueTypeDef]],
+        "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
@@ -2221,18 +2644,28 @@
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateItemOutputTableTypeDef = TypedDict(
+    "UpdateItemOutputTableTypeDef",
+    {
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
-        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
@@ -2247,48 +2680,192 @@
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
+    "GlobalSecondaryIndexUpdateTableTypeDef",
+    {
+        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
+        "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
+        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+    },
+    total=False,
+)
+
+GlobalSecondaryIndexUpdateTypeDef = TypedDict(
+    "GlobalSecondaryIndexUpdateTypeDef",
+    {
+        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
+        "Create": CreateGlobalSecondaryIndexActionTypeDef,
+        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
     },
 )
 _OptionalTableCreationParametersTypeDef = TypedDict(
     "_OptionalTableCreationParametersTypeDef",
     {
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexTypeDef],
     },
     total=False,
 )
 
+
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
-GlobalSecondaryIndexUpdateTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTypeDef",
+
+SourceTableFeatureDetailsTypeDef = TypedDict(
+    "SourceTableFeatureDetailsTypeDef",
     {
-        "Update": UpdateGlobalSecondaryIndexActionTypeDef,
-        "Create": CreateGlobalSecondaryIndexActionTypeDef,
-        "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
+        "StreamDescription": StreamSpecificationTypeDef,
+        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateTableInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTableInputRequestTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputRequestTypeDef(
+    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+        "BackupArn": str,
+    },
+)
+_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreTableFromBackupInputRequestTypeDef(
+    _RequiredRestoreTableFromBackupInputRequestTypeDef,
+    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+    },
+)
+_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "SourceTableArn": str,
+        "SourceTableName": str,
+        "UseLatestRestorableTime": bool,
+        "RestoreDateTime": TimestampTypeDef,
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
     },
     total=False,
 )
 
+
+class RestoreTableToPointInTimeInputRequestTypeDef(
+    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
+    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
+
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2323,20 +2900,22 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class CreateReplicationGroupMemberActionTypeDef(
     _RequiredCreateReplicationGroupMemberActionTypeDef,
     _OptionalCreateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+
 _RequiredUpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredUpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalUpdateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -2346,68 +2925,30 @@
         "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
         "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTypeDef],
         "TableClassOverride": TableClassType,
     },
     total=False,
 )
 
+
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
-InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
+
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
-GlobalSecondaryIndexUnionTypeDef = Union[
-    GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef
-]
-_RequiredTableCreationParametersOutputTypeDef = TypedDict(
-    "_RequiredTableCreationParametersOutputTypeDef",
-    {
-        "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
-        "KeySchema": List[KeySchemaElementTypeDef],
-    },
-)
-_OptionalTableCreationParametersOutputTypeDef = TypedDict(
-    "_OptionalTableCreationParametersOutputTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
-    },
-    total=False,
-)
-
-class TableCreationParametersOutputTypeDef(
-    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
-):
-    pass
-
-SourceTableFeatureDetailsTypeDef = TypedDict(
-    "SourceTableFeatureDetailsTypeDef",
-    {
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationTypeDef,
-        "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-    },
-    total=False,
-)
-
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2423,52 +2964,21 @@
     "_OptionalBatchExecuteStatementInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
 
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
@@ -2491,41 +3001,20 @@
         "KeyConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class QueryInputRequestTypeDef(
     _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": ConditionBaseImportTypeDef,
-        "KeyConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
 
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
@@ -2547,70 +3036,18 @@
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
     },
     total=False,
 )
 
-class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
-    pass
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
+class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-        "ConsistentRead": bool,
-    },
-    total=False,
-)
 
 _RequiredDeleteItemInputRequestTypeDef = TypedDict(
     "_RequiredDeleteItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
@@ -2626,44 +3063,20 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
     pass
 
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[str, TableAttributeValueTypeDef],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
 
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
@@ -2679,44 +3092,20 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
-    {
-        "Item": Mapping[str, TableAttributeValueTypeDef],
-    },
-)
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
 
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
@@ -2734,55 +3123,59 @@
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
+
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
+
+TransactGetItemTypeDef = TypedDict(
+    "TransactGetItemTypeDef",
     {
-        "Key": Mapping[str, TableAttributeValueTypeDef],
+        "Get": GetTypeDef,
     },
 )
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
+
+_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputRequestTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesTypeDef],
+    },
+)
+_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputRequestTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": ConditionBaseImportTypeDef,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
-TransactGetItemTypeDef = TypedDict(
-    "TransactGetItemTypeDef",
+
+BatchGetItemOutputTypeDef = TypedDict(
+    "BatchGetItemOutputTypeDef",
     {
-        "Get": GetTypeDef,
+        "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KeysAndAttributesUnionTypeDef = Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
 _RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteTransactionInputRequestTypeDef",
     {
         "TransactStatements": Sequence[ParameterizedStatementTypeDef],
     },
 )
 _OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
@@ -2790,19 +3183,21 @@
     {
         "ClientRequestToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class ExecuteTransactionInputRequestTypeDef(
     _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+
 WriteRequestTypeDef = TypedDict(
     "WriteRequestTypeDef",
     {
         "PutRequest": PutRequestTypeDef,
         "DeleteRequest": DeleteRequestTypeDef,
     },
     total=False,
@@ -2815,14 +3210,47 @@
         "Put": PutTypeDef,
         "Delete": DeleteTypeDef,
         "Update": UpdateTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
+
+BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchWriteItemOutputServiceResourceTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -2844,20 +3272,22 @@
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
 ):
     pass
 
+
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -2874,20 +3304,22 @@
     {
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalGlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
+
 ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -2904,28 +3336,46 @@
     {
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettingsUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
+
+ImportTableDescriptionTypeDef = TypedDict(
+    "ImportTableDescriptionTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ImportArn": str,
+        "ImportStatus": ImportStatusType,
+        "TableArn": str,
+        "TableId": str,
+        "ClientToken": str,
+        "S3BucketSource": S3BucketSourceTypeDef,
+        "ErrorCount": int,
+        "CloudWatchLogGroupArn": str,
+        "InputFormat": InputFormatType,
+        "InputFormatOptions": InputFormatOptionsTypeDef,
+        "InputCompressionType": InputCompressionTypeType,
+        "TableCreationParameters": TableCreationParametersTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ProcessedSizeBytes": int,
+        "ProcessedItemCount": int,
+        "ImportedItemCount": int,
+        "FailureCode": str,
+        "FailureMessage": str,
     },
+    total=False,
 )
 
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
@@ -2938,31 +3388,73 @@
         "ClientToken": str,
         "InputFormatOptions": InputFormatOptionsTypeDef,
         "InputCompressionType": InputCompressionTypeType,
     },
     total=False,
 )
 
+
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
+
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
+    {
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+    },
+    total=False,
+)
+
 GlobalTableDescriptionTypeDef = TypedDict(
     "GlobalTableDescriptionTypeDef",
     {
         "ReplicationGroup": List[ReplicaDescriptionTypeDef],
         "GlobalTableArn": str,
         "CreationDateTime": datetime,
         "GlobalTableStatus": GlobalTableStatusType,
         "GlobalTableName": str,
     },
     total=False,
 )
 
+TableDescriptionTableTypeDef = TypedDict(
+    "TableDescriptionTableTypeDef",
+    {
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTypeDef],
+        "RestoreSummary": RestoreSummaryTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+        "ArchivalSummary": ArchivalSummaryTypeDef,
+        "TableClassSummary": TableClassSummaryTypeDef,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
 TableDescriptionTypeDef = TypedDict(
     "TableDescriptionTypeDef",
     {
         "AttributeDefinitions": List[AttributeDefinitionTypeDef],
         "TableName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "TableStatus": TableStatusType,
@@ -2995,224 +3487,67 @@
         "Create": CreateReplicationGroupMemberActionTypeDef,
         "Update": UpdateReplicationGroupMemberActionTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateTableInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTableInputRequestTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-class CreateTableInputRequestTypeDef(
-    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
-):
-    pass
-
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
-):
-    pass
-
-_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-        "BackupArn": str,
-    },
-)
-_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreTableFromBackupInputRequestTypeDef(
-    _RequiredRestoreTableFromBackupInputRequestTypeDef,
-    _OptionalRestoreTableFromBackupInputRequestTypeDef,
-):
-    pass
-
-_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-    },
-)
-_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "SourceTableArn": str,
-        "SourceTableName": str,
-        "UseLatestRestorableTime": bool,
-        "RestoreDateTime": TimestampTypeDef,
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreTableToPointInTimeInputRequestTypeDef(
-    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
-    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-ImportTableDescriptionTypeDef = TypedDict(
-    "ImportTableDescriptionTypeDef",
-    {
-        "ImportArn": str,
-        "ImportStatus": ImportStatusType,
-        "TableArn": str,
-        "TableId": str,
-        "ClientToken": str,
-        "S3BucketSource": S3BucketSourceTypeDef,
-        "ErrorCount": int,
-        "CloudWatchLogGroupArn": str,
-        "InputFormat": InputFormatType,
-        "InputFormatOptions": InputFormatOptionsOutputTypeDef,
-        "InputCompressionType": InputCompressionTypeType,
-        "TableCreationParameters": TableCreationParametersOutputTypeDef,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ProcessedSizeBytes": int,
-        "ProcessedItemCount": int,
-        "ImportedItemCount": int,
-        "FailureCode": str,
-        "FailureMessage": str,
-    },
-    total=False,
-)
-
-TableCreationParametersUnionTypeDef = Union[
-    TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
-]
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
     },
 )
 _OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
     "_OptionalTransactGetItemsInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
+
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
-_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputRequestTypeDef",
+
+_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputRequestTypeDef",
     {
-        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+        "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
     },
 )
-_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputRequestTypeDef",
+_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputRequestTypeDef",
     {
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
     total=False,
 )
 
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
+
+class BatchWriteItemInputRequestTypeDef(
+    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
 ):
     pass
 
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
-    },
-)
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
-    pass
-
-WriteRequestUnionTypeDef = Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
 _OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
@@ -3221,19 +3556,21 @@
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class TransactWriteItemsInputRequestTypeDef(
     _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
 ):
     pass
 
+
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
@@ -3261,19 +3598,21 @@
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaSettingsDescriptionTypeDef(
     _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
 ):
     pass
 
+
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -3283,19 +3622,21 @@
             ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef
         ],
         "ReplicaProvisionedReadCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
 )
 
+
 class ReplicaAutoScalingUpdateTypeDef(
     _RequiredReplicaAutoScalingUpdateTypeDef, _OptionalReplicaAutoScalingUpdateTypeDef
 ):
     pass
 
+
 _RequiredReplicaSettingsUpdateTypeDef = TypedDict(
     "_RequiredReplicaSettingsUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaSettingsUpdateTypeDef = TypedDict(
@@ -3307,19 +3648,53 @@
             ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaTableClass": TableClassType,
     },
     total=False,
 )
 
+
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
+
+DescribeImportOutputTypeDef = TypedDict(
+    "DescribeImportOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportTableOutputTypeDef = TypedDict(
+    "ImportTableOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupOutputTypeDef = TypedDict(
+    "DeleteBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupOutputTypeDef = TypedDict(
+    "DescribeBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3336,14 +3711,22 @@
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteTableOutputTableTypeDef = TypedDict(
+    "DeleteTableOutputTableTypeDef",
+    {
+        "TableDescription": TableDescriptionTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3406,108 +3789,37 @@
         "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
+
 class UpdateTableInputRequestTypeDef(
     _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
 ):
     pass
 
+
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "BillingMode": BillingModeType,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
         "StreamSpecification": StreamSpecificationTypeDef,
         "SSESpecification": SSESpecificationTypeDef,
         "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
         "TableClass": TableClassType,
         "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
-DescribeImportOutputTypeDef = TypedDict(
-    "DescribeImportOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportTableOutputTypeDef = TypedDict(
-    "ImportTableOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupOutputTypeDef = TypedDict(
-    "DeleteBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupOutputTypeDef = TypedDict(
-    "DescribeBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputRequestTypeDef",
-    {
-        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
-    },
-)
-_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputRequestTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-    },
-    total=False,
-)
-
-class BatchWriteItemInputRequestTypeDef(
-    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
-):
-    pass
-
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
-    },
-)
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-    },
-    total=False,
-)
-
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-):
-    pass
-
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
@@ -3544,20 +3856,22 @@
         "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef],
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
         "ReplicaUpdates": Sequence[ReplicaAutoScalingUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTableReplicaAutoScalingInputRequestTypeDef(
     _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef,
     _OptionalUpdateTableReplicaAutoScalingInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalTableSettingsInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
 )
 _OptionalUpdateGlobalTableSettingsInputRequestTypeDef = TypedDict(
@@ -3572,20 +3886,22 @@
             GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef
         ],
         "ReplicaSettingsUpdate": Sequence[ReplicaSettingsUpdateTypeDef],
     },
     total=False,
 )
 
+
 class UpdateGlobalTableSettingsInputRequestTypeDef(
     _RequiredUpdateGlobalTableSettingsInputRequestTypeDef,
     _OptionalUpdateGlobalTableSettingsInputRequestTypeDef,
 ):
     pass
 
+
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.2.post4/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

