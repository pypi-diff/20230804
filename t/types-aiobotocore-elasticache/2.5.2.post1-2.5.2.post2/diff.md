# Comparing `tmp/types-aiobotocore-elasticache-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elasticache-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticache-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticache-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-elasticache-2.5.2.post1.tar` & `types-aiobotocore-elasticache-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27950 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26416 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70967 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70872 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-08-02 14:38:09.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86837 2023-08-02 14:38:12.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86770 2023-08-02 14:38:11.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-02 14:38:09.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27950 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.308062 types-aiobotocore-elasticache-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-08-04 12:00:50.308062 types-aiobotocore-elasticache-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.308062 types-aiobotocore-elasticache-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.296062 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70957 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70862 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86250 2023-08-04 11:45:40.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86183 2023-08-04 11:45:39.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:36.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-04 11:45:38.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.308062 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:00:50.000000 types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/LICENSE` & `types-aiobotocore-elasticache-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/setup.py` & `types-aiobotocore-elasticache-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticache",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__main__.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElastiCache 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ElastiCache 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationUnionTypeDef,
+    NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -431,15 +431,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
```

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationUnionTypeDef,
+    NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -413,15 +413,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
```

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -117,16 +118,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -158,14 +157,15 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
@@ -189,16 +189,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
-    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -208,14 +206,15 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -223,32 +222,31 @@
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -558,14 +556,28 @@
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -1075,42 +1087,14 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1666,14 +1650,28 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -2058,31 +2056,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
-NodeGroupConfigurationUnionTypeDef = Union[
-    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
-]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2262,14 +2243,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
@@ -2428,49 +2444,14 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2543,14 +2524,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2611,15 +2625,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2772,47 +2786,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -116,16 +117,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -157,14 +156,15 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
@@ -188,16 +188,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
-    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -207,14 +205,15 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -222,32 +221,31 @@
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -547,14 +545,28 @@
 
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -1048,42 +1060,14 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1617,14 +1601,28 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -2001,31 +1999,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
-NodeGroupConfigurationUnionTypeDef = Union[
-    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
-]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2205,14 +2186,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
@@ -2369,49 +2385,14 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2484,14 +2465,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2550,15 +2564,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2705,47 +2719,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.py` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.pyi` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/SOURCES.txt` & `types-aiobotocore-elasticache-2.5.2.post2/types_aiobotocore_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

