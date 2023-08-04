# Comparing `tmp/mypy-boto3-dynamodb-1.28.16.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.16.tar", last modified: Tue Aug  1 11:36:39 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.19.tar", last modified: Fri Aug  4 11:19:14 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.16.tar` & `mypy-boto3-dynamodb-1.28.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.404906 mypy-boto3-dynamodb-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-08-01 11:36:39.400906 mypy-boto3-dynamodb-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.396906 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48027 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-08-01 11:15:32.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   105178 2023-08-01 11:15:36.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105039 2023-08-01 11:15:34.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-01 11:15:31.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.400906 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:39.000000 mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:39.404906 mypy-boto3-dynamodb-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:15:30.000000 mypy-boto3-dynamodb-1.28.16/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:19:14.696644 mypy-boto3-dynamodb-1.28.19/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16161 2023-08-04 11:19:14.696644 mypy-boto3-dynamodb-1.28.19/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14673 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:19:14.696644 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1858 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1856 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      911 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47967 2023-08-04 11:18:29.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47900 2023-08-04 11:18:29.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12961 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12959 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7505 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7498 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22466 2023-08-04 11:18:29.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22439 2023-08-04 11:18:29.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   110921 2023-08-04 11:18:33.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   110782 2023-08-04 11:18:32.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2258 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2256 2023-08-04 11:18:30.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:19:14.696644 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16161 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      841 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       20 2023-08-04 11:19:14.000000 mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 11:19:14.696644 mypy-boto3-dynamodb-1.28.19/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2000 2023-08-04 11:18:28.000000 mypy-boto3-dynamodb-1.28.19/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.16/LICENSE` & `mypy-boto3-dynamodb-1.28.19/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.28.19\nVersion:         1.28.19\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.19")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,20 @@
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
@@ -104,15 +104,15 @@
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
@@ -121,15 +121,15 @@
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
@@ -211,29 +211,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_execute_statement)
         """
 
     def batch_get_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_get_item)
         """
 
     def batch_write_item(
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
 
@@ -278,15 +278,15 @@
     def create_table(
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
@@ -564,17 +564,17 @@
         """
 
     def import_table(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#import_table)
@@ -712,15 +712,15 @@
 
     def restore_table_from_backup(
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

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,20 @@
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
@@ -104,15 +104,15 @@
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
@@ -121,15 +121,15 @@
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
@@ -205,28 +205,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_execute_statement)
         """
     def batch_get_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#batch_get_item)
         """
     def batch_write_item(
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
 
@@ -266,15 +266,15 @@
     def create_table(
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
@@ -528,17 +528,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#get_item)
         """
     def import_table(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#import_table)
@@ -666,15 +666,15 @@
         """
     def restore_table_from_backup(
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

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,15 @@
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

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,15 @@
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

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,21 +34,21 @@
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
@@ -129,26 +129,26 @@
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
-    ) -> _PageIterator[QueryOutputTypeDef]:
+    ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 
 class ScanPaginator(Paginator):
@@ -160,23 +160,23 @@
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
-    ) -> _PageIterator[ScanOutputTypeDef]:
+    ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,21 @@
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
@@ -123,26 +123,26 @@
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
-    ) -> _PageIterator[QueryOutputTypeDef]:
+    ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(Paginator):
     """
@@ -153,23 +153,23 @@
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
-    ) -> _PageIterator[ScanOutputTypeDef]:
+    ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -35,110 +35,103 @@
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
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
-
 class ServiceResourceTablesCollection(ResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
     """
 
     def all(self) -> "ServiceResourceTablesCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
-
     def filter(  # type: ignore
         self, *, ExclusiveStartTableName: str = ..., Limit: int = ...
     ) -> "ServiceResourceTablesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
-
     def limit(self, count: int) -> "ServiceResourceTablesCollection":
         """
         Return at most this many Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
-
     def page_size(self, count: int) -> "ServiceResourceTablesCollection":
         """
         Fetch at most this many Tables per service request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
-
     def pages(self) -> Iterator[List["Table"]]:
         """
         A generator which yields pages of Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
-
     def __iter__(self) -> Iterator["Table"]:
         """
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
-
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
     attribute_definitions: List[AttributeDefinitionTypeDef]
@@ -148,16 +141,16 @@
     creation_date_time: datetime
     provisioned_throughput: ProvisionedThroughputDescriptionResponseTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
     billing_mode_summary: BillingModeSummaryResponseTypeDef
-    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTypeDef]
-    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTypeDef]
+    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
+    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
     stream_specification: StreamSpecificationResponseTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
     replicas: List[ReplicaDescriptionTypeDef]
     restore_summary: RestoreSummaryResponseTypeDef
     sse_description: SSEDescriptionResponseTypeDef
@@ -169,233 +162,217 @@
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablebatch_writer-method)
         """
-
-    def delete(self) -> DeleteTableOutputTypeDef:
+    def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete-method)
         """
-
     def delete_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> DeleteItemOutputTypeDef:
+    ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
-
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_available_subresources-method)
         """
-
     def get_item(
         self,
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_item-method)
         """
-
     def load(self) -> None:
         """
         Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
         Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableload-method)
         """
-
     def put_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> PutItemOutputTypeDef:
+    ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
-
     def query(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablequery-method)
         """
-
     def reload(self) -> None:
         """
         Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
         Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablereload-method)
         """
-
     def scan(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablescan-method)
         """
-
     def update(
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
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate-method)
         """
-
     def update_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> UpdateItemOutputTypeDef:
+    ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
         """
-
     def wait_until_exists(self) -> None:
         """
         Waits until this Table is exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_exists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablewait_until_exists-method)
         """
-
     def wait_until_not_exists(self) -> None:
         """
         Waits until this Table is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_not_exists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablewait_until_not_exists-method)
         """
 
-
 _Table = Table
 
-
 class DynamoDBResourceMeta(ResourceMeta):
     client: DynamoDBClient
 
-
 class DynamoDBServiceResource(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/)
     """
 
     meta: "DynamoDBResourceMeta"
@@ -404,67 +381,63 @@
     def Table(self, name: str) -> _Table:
         """
         Creates a Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
-
     def batch_get_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
-
     def batch_write_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
-
     def create_table(
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
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
-
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourceget_available_subresources-method)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/service_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,103 +35,110 @@
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
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
+
 class ServiceResourceTablesCollection(ResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
     """
 
     def all(self) -> "ServiceResourceTablesCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
+
     def filter(  # type: ignore
         self, *, ExclusiveStartTableName: str = ..., Limit: int = ...
     ) -> "ServiceResourceTablesCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
+
     def limit(self, count: int) -> "ServiceResourceTablesCollection":
         """
         Return at most this many Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
+
     def page_size(self, count: int) -> "ServiceResourceTablesCollection":
         """
         Fetch at most this many Tables per service request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
+
     def pages(self) -> Iterator[List["Table"]]:
         """
         A generator which yields pages of Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
+
     def __iter__(self) -> Iterator["Table"]:
         """
         A generator which yields Tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#serviceresourcetablescollection)
         """
 
+
 class Table(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#table)
     """
 
     attribute_definitions: List[AttributeDefinitionTypeDef]
@@ -141,16 +148,16 @@
     creation_date_time: datetime
     provisioned_throughput: ProvisionedThroughputDescriptionResponseTypeDef
     table_size_bytes: int
     item_count: int
     table_arn: str
     table_id: str
     billing_mode_summary: BillingModeSummaryResponseTypeDef
-    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTypeDef]
-    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTypeDef]
+    local_secondary_indexes: List[LocalSecondaryIndexDescriptionTableTypeDef]
+    global_secondary_indexes: List[GlobalSecondaryIndexDescriptionTableTypeDef]
     stream_specification: StreamSpecificationResponseTypeDef
     latest_stream_label: str
     latest_stream_arn: str
     global_table_version: str
     replicas: List[ReplicaDescriptionTypeDef]
     restore_summary: RestoreSummaryResponseTypeDef
     sse_description: SSEDescriptionResponseTypeDef
@@ -162,217 +169,233 @@
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablebatch_writer-method)
         """
-    def delete(self) -> DeleteTableOutputTypeDef:
+
+    def delete(self) -> DeleteTableOutputTableTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete-method)
         """
+
     def delete_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> DeleteItemOutputTypeDef:
+    ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
+
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_available_subresources-method)
         """
+
     def get_item(
         self,
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableget_item-method)
         """
+
     def load(self) -> None:
         """
         Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
         Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableload-method)
         """
+
     def put_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> PutItemOutputTypeDef:
+    ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
+
     def query(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablequery-method)
         """
+
     def reload(self) -> None:
         """
         Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
         Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablereload-method)
         """
+
     def scan(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablescan-method)
         """
+
     def update(
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
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate-method)
         """
+
     def update_item(
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
         ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
-    ) -> UpdateItemOutputTypeDef:
+    ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
         """
+
     def wait_until_exists(self) -> None:
         """
         Waits until this Table is exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_exists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablewait_until_exists-method)
         """
+
     def wait_until_not_exists(self) -> None:
         """
         Waits until this Table is not exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_not_exists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tablewait_until_not_exists-method)
         """
 
+
 _Table = Table
 
+
 class DynamoDBResourceMeta(ResourceMeta):
     client: DynamoDBClient
 
+
 class DynamoDBServiceResource(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/)
     """
 
     meta: "DynamoDBResourceMeta"
@@ -381,63 +404,67 @@
     def Table(self, name: str) -> _Table:
         """
         Creates a Table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
+
     def batch_get_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
+
     def batch_write_item(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
+
     def create_table(
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
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
+
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourceget_available_subresources-method)
         """
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,35 +64,35 @@
 
 
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
@@ -110,15 +110,14 @@
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
@@ -141,66 +140,73 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "BatchStatementErrorTypeDef",
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
-    "BatchStatementErrorTypeDef",
-    "DeleteRequestOutputTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "ItemCollectionMetricsTypeDef",
-    "ItemResponseTypeDef",
-    "KeysAndAttributesOutputTypeDef",
-    "PutRequestOutputTypeDef",
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
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
@@ -208,106 +214,110 @@
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
-    "BatchStatementResponseTypeDef",
-    "WriteRequestOutputTypeDef",
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
+    "BatchExecuteStatementOutputTypeDef",
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
-    "BatchExecuteStatementOutputTypeDef",
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
@@ -355,14 +365,30 @@
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
@@ -444,30 +470,14 @@
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
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -516,31 +526,40 @@
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
@@ -595,28 +614,19 @@
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
@@ -821,23 +831,14 @@
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
@@ -1163,14 +1164,41 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
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
@@ -1180,82 +1208,60 @@
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
+class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
 
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
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
+ExpectedAttributeValueTableTypeDef = TypedDict(
+    "ExpectedAttributeValueTableTypeDef",
     {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Value": TableAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-DeleteRequestOutputTypeDef = TypedDict(
-    "DeleteRequestOutputTypeDef",
-    {
-        "Key": Dict[str, TableAttributeValueTypeDef],
-    },
-)
-
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
 _OptionalGetItemInputTableGetItemTypeDef = TypedDict(
@@ -1273,59 +1279,112 @@
 
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
 
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
 
 
-class KeysAndAttributesOutputTypeDef(
-    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+class KeysAndAttributesServiceResourceTypeDef(
+    _RequiredKeysAndAttributesServiceResourceTypeDef,
+    _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
 
-PutRequestOutputTypeDef = TypedDict(
-    "PutRequestOutputTypeDef",
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
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
@@ -1365,20 +1424,84 @@
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
@@ -1398,14 +1521,25 @@
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
+
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -1421,47 +1555,43 @@
 
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
 
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
@@ -1521,22 +1651,14 @@
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
@@ -1695,77 +1817,36 @@
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
@@ -1849,14 +1930,24 @@
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Action": AttributeActionType,
     },
     total=False,
@@ -2137,14 +2228,248 @@
 )
 
 
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
@@ -2161,111 +2486,145 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
+BatchGetItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
+        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchGetItemOutputTypeDef = TypedDict(
-    "BatchGetItemOutputTypeDef",
+DeleteItemOutputTableTypeDef = TypedDict(
+    "DeleteItemOutputTableTypeDef",
     {
-        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
@@ -2281,18 +2640,28 @@
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
@@ -2307,50 +2676,192 @@
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
 
 
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
 
-GlobalSecondaryIndexUpdateTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTypeDef",
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
@@ -2418,73 +2929,40 @@
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
 
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
 )
 
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2499,49 +2977,14 @@
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
@@ -2570,37 +3013,14 @@
 
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
-
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -2626,70 +3046,14 @@
 )
 
 
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
 
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
@@ -2712,43 +3076,14 @@
 
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
@@ -2771,43 +3106,14 @@
 
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
@@ -2832,53 +3138,52 @@
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
 
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
@@ -2913,14 +3218,47 @@
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
@@ -3014,31 +3352,38 @@
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
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
@@ -3058,26 +3403,66 @@
 
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
@@ -3110,173 +3495,14 @@
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
@@ -3290,58 +3516,46 @@
 
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
 
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
 
 
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
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
@@ -3449,14 +3663,46 @@
 
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
+
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3473,14 +3719,22 @@
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
@@ -3556,101 +3810,24 @@
 
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
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -63,35 +63,35 @@
     from typing_extensions import TypedDict
 
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
@@ -109,15 +109,14 @@
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
@@ -140,66 +139,73 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "BatchStatementErrorTypeDef",
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
-    "BatchStatementErrorTypeDef",
-    "DeleteRequestOutputTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "ItemCollectionMetricsTypeDef",
-    "ItemResponseTypeDef",
-    "KeysAndAttributesOutputTypeDef",
-    "PutRequestOutputTypeDef",
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
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
@@ -207,106 +213,110 @@
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
-    "BatchStatementResponseTypeDef",
-    "WriteRequestOutputTypeDef",
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
+    "BatchExecuteStatementOutputTypeDef",
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
-    "BatchExecuteStatementOutputTypeDef",
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
@@ -354,14 +364,30 @@
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
@@ -437,30 +463,14 @@
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
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -509,31 +519,40 @@
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
@@ -586,28 +605,19 @@
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
@@ -810,23 +820,14 @@
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
@@ -1144,14 +1145,41 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
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
@@ -1161,80 +1189,58 @@
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
+class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
     pass
 
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
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
+ExpectedAttributeValueTableTypeDef = TypedDict(
+    "ExpectedAttributeValueTableTypeDef",
     {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
+        "Value": TableAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-DeleteRequestOutputTypeDef = TypedDict(
-    "DeleteRequestOutputTypeDef",
-    {
-        "Key": Dict[str, TableAttributeValueTypeDef],
-    },
-)
-
 _RequiredGetItemInputTableGetItemTypeDef = TypedDict(
     "_RequiredGetItemInputTableGetItemTypeDef",
     {
         "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
 _OptionalGetItemInputTableGetItemTypeDef = TypedDict(
@@ -1250,57 +1256,108 @@
 )
 
 class GetItemInputTableGetItemTypeDef(
     _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
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
 
-class KeysAndAttributesOutputTypeDef(
-    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
+class KeysAndAttributesServiceResourceTypeDef(
+    _RequiredKeysAndAttributesServiceResourceTypeDef,
+    _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-PutRequestOutputTypeDef = TypedDict(
-    "PutRequestOutputTypeDef",
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
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
+):
+    pass
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
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
@@ -1338,20 +1395,80 @@
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
@@ -1369,14 +1486,25 @@
 
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
+
 _RequiredGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -1390,45 +1518,43 @@
 )
 
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
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
@@ -1486,22 +1612,14 @@
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
@@ -1654,75 +1772,36 @@
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
@@ -1804,14 +1883,24 @@
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Action": AttributeActionType,
     },
     total=False,
@@ -2070,14 +2159,236 @@
     },
     total=False,
 )
 
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
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
+
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
@@ -2094,111 +2405,145 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
+BatchGetItemOutputServiceResourceTypeDef = TypedDict(
+    "BatchGetItemOutputServiceResourceTypeDef",
     {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, TableAttributeValueTypeDef],
-    },
-    total=False,
-)
-
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
+        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
+        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchGetItemOutputTypeDef = TypedDict(
-    "BatchGetItemOutputTypeDef",
+DeleteItemOutputTableTypeDef = TypedDict(
+    "DeleteItemOutputTableTypeDef",
     {
-        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
+        "ConsumedCapacity": ConsumedCapacityTypeDef,
+        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
@@ -2214,18 +2559,28 @@
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
@@ -2240,48 +2595,182 @@
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
 
 class TableCreationParametersTypeDef(
     _RequiredTableCreationParametersTypeDef, _OptionalTableCreationParametersTypeDef
 ):
     pass
 
-GlobalSecondaryIndexUpdateTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTypeDef",
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
     },
     total=False,
 )
 
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
+    },
+    total=False,
+)
+
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
@@ -2345,71 +2834,40 @@
 
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
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
 )
 
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2422,47 +2880,14 @@
 
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
-
 _RequiredQueryInputRequestTypeDef = TypedDict(
     "_RequiredQueryInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalQueryInputRequestTypeDef = TypedDict(
@@ -2489,37 +2914,14 @@
 )
 
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
-
 _RequiredScanInputRequestTypeDef = TypedDict(
     "_RequiredScanInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalScanInputRequestTypeDef = TypedDict(
@@ -2543,68 +2945,14 @@
     },
     total=False,
 )
 
 class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
     pass
 
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
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
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
@@ -2625,41 +2973,14 @@
 )
 
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
 _RequiredPutItemInputRequestTypeDef = TypedDict(
     "_RequiredPutItemInputRequestTypeDef",
     {
         "TableName": str,
         "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
@@ -2680,41 +3001,14 @@
 )
 
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
-
 _RequiredUpdateItemInputRequestTypeDef = TypedDict(
     "_RequiredUpdateItemInputRequestTypeDef",
     {
         "TableName": str,
         "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
@@ -2737,51 +3031,50 @@
 )
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
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
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
 ):
     pass
 
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
@@ -2814,14 +3107,45 @@
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
@@ -2909,31 +3233,38 @@
 
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
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
@@ -2951,26 +3282,66 @@
 )
 
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
@@ -3003,165 +3374,14 @@
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
@@ -3173,54 +3393,44 @@
 )
 
 class TransactGetItemsInputRequestTypeDef(
     _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
 ):
     pass
 
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
 
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
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
@@ -3320,14 +3530,46 @@
 )
 
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
+
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3344,14 +3586,22 @@
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
@@ -3425,97 +3675,24 @@
 
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
```

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.19/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.16/setup.py` & `mypy-boto3-dynamodb-1.28.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.16",
+    version="1.28.19",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.DynamoDB 1.28.19 service generated with mypy-boto3-builder"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

