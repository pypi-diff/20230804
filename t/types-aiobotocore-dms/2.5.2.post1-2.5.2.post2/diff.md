# Comparing `tmp/types-aiobotocore-dms-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dms-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-dms-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-dms-2.5.2.post1.tar` & `types-aiobotocore-dms-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.821601 types-aiobotocore-dms-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.821601 types-aiobotocore-dms-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69116 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69017 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94720 2023-08-02 14:36:35.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94669 2023-08-02 14:36:33.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.131942 types-aiobotocore-dms-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17015 2023-08-04 12:00:47.123942 types-aiobotocore-dms-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.131942 types-aiobotocore-dms-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-04 11:43:51.000000 types-aiobotocore-dms-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.123942 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69101 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69002 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-08-04 11:43:54.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-08-04 11:43:54.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    92903 2023-08-04 11:43:56.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92852 2023-08-04 11:43:55.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:52.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-04 11:43:53.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.123942 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17015 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:46.000000 types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dms-2.5.2.post1/LICENSE` & `types-aiobotocore-dms-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/setup.py` & `types-aiobotocore-dms-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dms",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__main__.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
-    OracleSettingsUnionTypeDef,
+    OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
     ReloadTablesResponseTypeDef,
@@ -292,15 +292,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsUnionTypeDef = ...,
+        OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -912,15 +912,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsUnionTypeDef = ...,
+        OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
```

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
-    OracleSettingsUnionTypeDef,
+    OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
     ReloadTablesResponseTypeDef,
@@ -281,15 +281,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsUnionTypeDef = ...,
+        OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -853,15 +853,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsUnionTypeDef = ...,
+        OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
```

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,14 @@
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
     "TableStatisticsTypeDef",
-    "OracleSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
@@ -178,14 +177,15 @@
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
+    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
@@ -242,31 +242,29 @@
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     "DescribeTableStatisticsResponseTypeDef",
-    "EndpointTypeDef",
-    "OracleSettingsUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
@@ -1311,63 +1309,14 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
     total=False,
 )
 
-OracleSettingsOutputTypeDef = TypedDict(
-    "OracleSettingsOutputTypeDef",
-    {
-        "AddSupplementalLogging": bool,
-        "ArchivedLogDestId": int,
-        "AdditionalArchivedLogDestId": int,
-        "ExtraArchivedLogDestIds": List[int],
-        "AllowSelectNestedTables": bool,
-        "ParallelAsmReadThreads": int,
-        "ReadAheadBlocks": int,
-        "AccessAlternateDirectly": bool,
-        "UseAlternateFolderForOnline": bool,
-        "OraclePathPrefix": str,
-        "UsePathPrefix": str,
-        "ReplacePathPrefix": bool,
-        "EnableHomogenousTablespace": bool,
-        "DirectPathNoLog": bool,
-        "ArchivedLogsOnly": bool,
-        "AsmPassword": str,
-        "AsmServer": str,
-        "AsmUser": str,
-        "CharLengthSemantics": CharLengthSemanticsType,
-        "DatabaseName": str,
-        "DirectPathParallelLoad": bool,
-        "FailTasksOnLobTruncation": bool,
-        "NumberDatatypeScale": int,
-        "Password": str,
-        "Port": int,
-        "ReadTableSpaceName": bool,
-        "RetryInterval": int,
-        "SecurityDbEncryption": str,
-        "SecurityDbEncryptionName": str,
-        "ServerName": str,
-        "SpatialDataOptionToGeoJsonFunctionName": str,
-        "StandbyDelayTime": int,
-        "Username": str,
-        "UseBFile": bool,
-        "UseDirectPathFullLoad": bool,
-        "UseLogminerReader": bool,
-        "SecretsManagerAccessRoleArn": str,
-        "SecretsManagerSecretId": str,
-        "SecretsManagerOracleAsmAccessRoleArn": str,
-        "SecretsManagerOracleAsmSecretId": str,
-        "TrimSpaceInChar": bool,
-        "ConvertTimestampWithZoneToUTC": bool,
-    },
-    total=False,
-)
-
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -2018,14 +1967,56 @@
 
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
 
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsTypeDef,
+        "S3Settings": S3SettingsTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsTypeDef,
+        "MongoDbSettings": MongoDbSettingsTypeDef,
+        "KinesisSettings": KinesisSettingsTypeDef,
+        "KafkaSettings": KafkaSettingsTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
+        "NeptuneSettings": NeptuneSettingsTypeDef,
+        "RedshiftSettings": RedshiftSettingsTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
+        "MySQLSettings": MySQLSettingsTypeDef,
+        "OracleSettings": OracleSettingsTypeDef,
+        "SybaseSettings": SybaseSettingsTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsTypeDef,
+        "DocDbSettings": DocDbSettingsTypeDef,
+        "RedisSettings": RedisSettingsTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalModifyEndpointMessageRequestTypeDef = TypedDict(
@@ -2795,57 +2786,14 @@
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsOutputTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-    },
-    total=False,
-)
-
-OracleSettingsUnionTypeDef = Union[OracleSettingsTypeDef, OracleSettingsOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2977,23 +2925,14 @@
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3019,14 +2958,23 @@
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "Databases": List[DatabaseResponseTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
     "TableStatisticsTypeDef",
-    "OracleSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
@@ -177,14 +176,15 @@
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
+    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
@@ -241,31 +241,29 @@
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     "DescribeTableStatisticsResponseTypeDef",
-    "EndpointTypeDef",
-    "OracleSettingsUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
@@ -1296,63 +1294,14 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
     total=False,
 )
 
-OracleSettingsOutputTypeDef = TypedDict(
-    "OracleSettingsOutputTypeDef",
-    {
-        "AddSupplementalLogging": bool,
-        "ArchivedLogDestId": int,
-        "AdditionalArchivedLogDestId": int,
-        "ExtraArchivedLogDestIds": List[int],
-        "AllowSelectNestedTables": bool,
-        "ParallelAsmReadThreads": int,
-        "ReadAheadBlocks": int,
-        "AccessAlternateDirectly": bool,
-        "UseAlternateFolderForOnline": bool,
-        "OraclePathPrefix": str,
-        "UsePathPrefix": str,
-        "ReplacePathPrefix": bool,
-        "EnableHomogenousTablespace": bool,
-        "DirectPathNoLog": bool,
-        "ArchivedLogsOnly": bool,
-        "AsmPassword": str,
-        "AsmServer": str,
-        "AsmUser": str,
-        "CharLengthSemantics": CharLengthSemanticsType,
-        "DatabaseName": str,
-        "DirectPathParallelLoad": bool,
-        "FailTasksOnLobTruncation": bool,
-        "NumberDatatypeScale": int,
-        "Password": str,
-        "Port": int,
-        "ReadTableSpaceName": bool,
-        "RetryInterval": int,
-        "SecurityDbEncryption": str,
-        "SecurityDbEncryptionName": str,
-        "ServerName": str,
-        "SpatialDataOptionToGeoJsonFunctionName": str,
-        "StandbyDelayTime": int,
-        "Username": str,
-        "UseBFile": bool,
-        "UseDirectPathFullLoad": bool,
-        "UseLogminerReader": bool,
-        "SecretsManagerAccessRoleArn": str,
-        "SecretsManagerSecretId": str,
-        "SecretsManagerOracleAsmAccessRoleArn": str,
-        "SecretsManagerOracleAsmSecretId": str,
-        "TrimSpaceInChar": bool,
-        "ConvertTimestampWithZoneToUTC": bool,
-    },
-    total=False,
-)
-
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1983,14 +1932,56 @@
 )
 
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsTypeDef,
+        "S3Settings": S3SettingsTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsTypeDef,
+        "MongoDbSettings": MongoDbSettingsTypeDef,
+        "KinesisSettings": KinesisSettingsTypeDef,
+        "KafkaSettings": KafkaSettingsTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
+        "NeptuneSettings": NeptuneSettingsTypeDef,
+        "RedshiftSettings": RedshiftSettingsTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
+        "MySQLSettings": MySQLSettingsTypeDef,
+        "OracleSettings": OracleSettingsTypeDef,
+        "SybaseSettings": SybaseSettingsTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsTypeDef,
+        "DocDbSettings": DocDbSettingsTypeDef,
+        "RedisSettings": RedisSettingsTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalModifyEndpointMessageRequestTypeDef = TypedDict(
@@ -2746,57 +2737,14 @@
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsOutputTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-    },
-    total=False,
-)
-
-OracleSettingsUnionTypeDef = Union[OracleSettingsTypeDef, OracleSettingsOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2926,23 +2874,14 @@
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2968,14 +2907,23 @@
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "Databases": List[DatabaseResponseTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.py` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.pyi` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/SOURCES.txt` & `types-aiobotocore-dms-2.5.2.post2/types_aiobotocore_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

