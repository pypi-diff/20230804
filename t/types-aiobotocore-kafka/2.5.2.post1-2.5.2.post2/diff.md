# Comparing `tmp/types-aiobotocore-kafka-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kafka-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kafka-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-kafka-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-kafka-2.5.2.post1.tar` & `types-aiobotocore-kafka-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.085555 types-aiobotocore-kafka-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21018 2023-08-02 14:52:29.081555 types-aiobotocore-kafka-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:29.085555 types-aiobotocore-kafka-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.081555 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36955 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56914 2023-08-02 14:41:16.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56841 2023-08-02 14:41:15.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:12.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.081555 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21018 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:28.000000 types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.396643 types-aiobotocore-kafka-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14420 2023-08-04 13:59:13.396643 types-aiobotocore-kafka-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12910 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.406643 types-aiobotocore-kafka-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.396643 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2839 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2838 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38775 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38708 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10851 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10849 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13197 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13184 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59047 2023-08-04 13:41:41.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58974 2023-08-04 13:41:40.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:38.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.396643 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14420 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:13.000000 types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/LICENSE` & `types-aiobotocore-kafka-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kafka-2.5.2.post1/setup.py` & `types-aiobotocore-kafka-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kafka",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Kafka 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__init__.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_kafka import (
         Client,
         KafkaClient,
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -24,28 +25,30 @@
     async with session.create_client("kafka") as client:
         client: KafkaClient
         ...
 
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
     list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -56,14 +59,15 @@
 
 
 __all__ = (
     "Client",
     "KafkaClient",
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__init__.pyi` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_kafka import (
         Client,
         KafkaClient,
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -24,28 +25,30 @@
     async with session.create_client("kafka") as client:
         client: KafkaClient
         ...
 
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
     list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -55,14 +58,15 @@
 Client = KafkaClient
 
 __all__ = (
     "Client",
     "KafkaClient",
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/__main__.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Kafka 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Kafka 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
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

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/client.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,52 +20,55 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoUnionTypeDef,
-    ClientAuthenticationUnionTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
@@ -171,19 +174,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#close)
         """
 
     async def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -293,14 +296,24 @@
         """
         Returns a description of the cluster operation specified by the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_operation)
         """
 
+    async def describe_cluster_operation_v2(
+        self, *, ClusterOperationArn: str
+    ) -> DescribeClusterOperationV2ResponseTypeDef:
+        """
+        Returns a description of the cluster operation specified by the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation_v2)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_operation_v2)
+        """
+
     async def describe_cluster_v2(self, *, ClusterArn: str) -> DescribeClusterV2ResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_v2)
@@ -390,14 +403,25 @@
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_cluster_operations)
         """
 
+    async def list_cluster_operations_v2(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClusterOperationsV2ResponseTypeDef:
+        """
+        Returns a list of all the operations that have been performed on the specified
+        MSK cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations_v2)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_cluster_operations_v2)
+        """
+
     async def list_clusters(
         self, *, ClusterNameFilter: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters)
@@ -637,15 +661,15 @@
         """
 
     async def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_security)
@@ -682,14 +706,23 @@
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cluster_operations_v2"]
+    ) -> ListClusterOperationsV2Paginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
         """
 
     @overload
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/client.pyi` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,52 +20,55 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoUnionTypeDef,
-    ClientAuthenticationUnionTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
@@ -162,19 +165,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#close)
         """
     async def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -274,14 +277,23 @@
     ) -> DescribeClusterOperationResponseTypeDef:
         """
         Returns a description of the cluster operation specified by the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_operation)
         """
+    async def describe_cluster_operation_v2(
+        self, *, ClusterOperationArn: str
+    ) -> DescribeClusterOperationV2ResponseTypeDef:
+        """
+        Returns a description of the cluster operation specified by the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation_v2)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_operation_v2)
+        """
     async def describe_cluster_v2(self, *, ClusterArn: str) -> DescribeClusterV2ResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#describe_cluster_v2)
@@ -361,14 +373,24 @@
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_cluster_operations)
         """
+    async def list_cluster_operations_v2(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClusterOperationsV2ResponseTypeDef:
+        """
+        Returns a list of all the operations that have been performed on the specified
+        MSK cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations_v2)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#list_cluster_operations_v2)
+        """
     async def list_clusters(
         self, *, ClusterNameFilter: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters)
@@ -586,15 +608,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_monitoring)
         """
     async def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#update_security)
@@ -627,14 +649,22 @@
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cluster_operations_v2"]
+    ) -> ListClusterOperationsV2Paginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_clusters_v2"]) -> ListClustersV2Paginator:
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/literals.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
     "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
+    "ListClusterOperationsV2PaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
@@ -65,14 +66,15 @@
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
 ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
+ListClusterOperationsV2PaginatorName = Literal["list_cluster_operations_v2"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
@@ -102,14 +104,15 @@
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
@@ -205,14 +208,15 @@
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
@@ -291,26 +295,28 @@
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
@@ -453,14 +459,15 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_client_vpc_connections",
     "list_cluster_operations",
+    "list_cluster_operations_v2",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/literals.pyi` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
     "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
+    "ListClusterOperationsV2PaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
@@ -63,14 +64,15 @@
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
 ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
+ListClusterOperationsV2PaginatorName = Literal["list_cluster_operations_v2"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
@@ -100,14 +102,15 @@
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
@@ -203,14 +206,15 @@
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
@@ -289,26 +293,28 @@
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
@@ -451,14 +457,15 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_client_vpc_connections",
     "list_cluster_operations",
+    "list_cluster_operations_v2",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/paginator.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_kafka.client import KafkaClient
     from types_aiobotocore_kafka.paginator import (
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -24,14 +25,15 @@
 
     session = get_session()
     with session.create_client("kafka") as client:
         client: KafkaClient
 
         list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
         list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+        list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
         list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
         list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
         list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
         list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
         list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
         list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
         list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
@@ -42,28 +44,30 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
@@ -107,14 +111,29 @@
     ) -> AsyncIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationspaginator)
         """
 
 
+class ListClusterOperationsV2Paginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationsv2paginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListClusterOperationsV2ResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationsv2paginator)
+        """
+
+
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/paginator.pyi` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_kafka.client import KafkaClient
     from types_aiobotocore_kafka.paginator import (
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -24,14 +25,15 @@
 
     session = get_session()
     with session.create_client("kafka") as client:
         client: KafkaClient
 
         list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
         list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+        list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
         list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
         list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
         list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
         list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
         list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
         list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
         list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
@@ -42,28 +44,30 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
@@ -102,14 +106,28 @@
         self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationspaginator)
         """
 
+class ListClusterOperationsV2Paginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationsv2paginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListClusterOperationsV2ResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusteroperationsv2paginator)
+        """
+
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/type_defs.py` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,31 +46,32 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "BlobTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
-    "TlsOutputTypeDef",
-    "UnauthenticatedTypeDef",
     "TlsTypeDef",
+    "UnauthenticatedTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
+    "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
@@ -80,14 +81,15 @@
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
+    "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersV2RequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
     "ListNodesRequestRequestTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
@@ -98,15 +100,14 @@
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
     "VpcConnectivityIamTypeDef",
@@ -142,78 +143,81 @@
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
+    "ListClusterOperationsV2ResponseTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    "ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
     "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
-    "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
+    "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoOutputTypeDef",
     "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
-    "ProvisionedTypeDef",
-    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
+    "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "ClusterTypeDef",
     "CreateClusterV2RequestRequestTypeDef",
+    "ClusterTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
+    "ClusterOperationV2TypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
+    "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
@@ -323,40 +327,31 @@
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
     total=False,
 )
 
-TlsOutputTypeDef = TypedDict(
-    "TlsOutputTypeDef",
+TlsTypeDef = TypedDict(
+    "TlsTypeDef",
     {
-        "CertificateAuthorityArnList": List[str],
+        "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
 UnauthenticatedTypeDef = TypedDict(
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-TlsTypeDef = TypedDict(
-    "TlsTypeDef",
-    {
-        "CertificateAuthorityArnList": Sequence[str],
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 _RequiredClientVpcConnectionTypeDef = TypedDict(
     "_RequiredClientVpcConnectionTypeDef",
     {
         "VpcConnectionArn": str,
     },
 )
 _OptionalClientVpcConnectionTypeDef = TypedDict(
@@ -399,14 +394,28 @@
     "ClusterOperationStepInfoTypeDef",
     {
         "StepStatus": str,
     },
     total=False,
 )
 
+ClusterOperationV2SummaryTypeDef = TypedDict(
+    "ClusterOperationV2SummaryTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+    },
+    total=False,
+)
+
 CompatibleKafkaVersionTypeDef = TypedDict(
     "CompatibleKafkaVersionTypeDef",
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
@@ -521,14 +530,21 @@
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
+DescribeClusterOperationV2RequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationV2RequestRequestTypeDef",
+    {
+        "ClusterOperationArn": str,
+    },
+)
+
 DescribeClusterRequestRequestTypeDef = TypedDict(
     "DescribeClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
@@ -682,14 +698,37 @@
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListClusterOperationsV2RequestRequestTypeDef(
+    _RequiredListClusterOperationsV2RequestRequestTypeDef,
+    _OptionalListClusterOperationsV2RequestRequestTypeDef,
+):
+    pass
+
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -918,33 +957,14 @@
 )
 
 
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
 
-_RequiredVpcConfigOutputTypeDef = TypedDict(
-    "_RequiredVpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-    },
-)
-_OptionalVpcConfigOutputTypeDef = TypedDict(
-    "_OptionalVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-
-class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1404,14 +1424,23 @@
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
+ListClusterOperationsV2ResponseTypeDef = TypedDict(
+    "ListClusterOperationsV2ResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1572,14 +1601,36 @@
 class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
     _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
+    _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+):
+    pass
+
+
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "ClusterNameFilter": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1717,14 +1768,25 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
+VpcConnectionInfoServerlessTypeDef = TypedDict(
+    "VpcConnectionInfoServerlessTypeDef",
+    {
+        "CreationTime": datetime,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "VpcConnectionArn": str,
+    },
+    total=False,
+)
+
 VpcConnectionInfoTypeDef = TypedDict(
     "VpcConnectionInfoTypeDef",
     {
         "VpcConnectionArn": str,
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
         "CreationTime": datetime,
@@ -1805,30 +1867,28 @@
 OpenMonitoringTypeDef = TypedDict(
     "OpenMonitoringTypeDef",
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 
-ClientAuthenticationOutputTypeDef = TypedDict(
-    "ClientAuthenticationOutputTypeDef",
+ClientAuthenticationTypeDef = TypedDict(
+    "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
-        "Tls": TlsOutputTypeDef,
+        "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-ClientAuthenticationTypeDef = TypedDict(
-    "ClientAuthenticationTypeDef",
+ClusterOperationV2ServerlessTypeDef = TypedDict(
+    "ClusterOperationV2ServerlessTypeDef",
     {
-        "Sasl": SaslTypeDef,
-        "Tls": TlsTypeDef,
-        "Unauthenticated": UnauthenticatedTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoServerlessTypeDef,
     },
     total=False,
 )
 
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
@@ -1867,15 +1927,15 @@
 ):
     pass
 
 
 _RequiredServerlessTypeDef = TypedDict(
     "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": List[VpcConfigTypeDef],
     },
 )
 _OptionalServerlessTypeDef = TypedDict(
     "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
@@ -1907,17 +1967,14 @@
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
 
-ClientAuthenticationUnionTypeDef = Union[
-    ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-]
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -1950,40 +2007,14 @@
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoOutputTypeDef",
-    {
-        "ClientSubnets": List[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoOutputTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": List[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": List[str],
-    },
-    total=False,
-)
-
-
-class BrokerNodeGroupInfoOutputTypeDef(
-    _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
-):
-    pass
-
-
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
 )
@@ -2013,15 +2044,15 @@
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
         "KafkaVersion": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
@@ -2034,16 +2065,16 @@
     },
 )
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -2056,102 +2087,99 @@
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-_RequiredProvisionedTypeDef = TypedDict(
-    "_RequiredProvisionedTypeDef",
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
     {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "ClusterName": str,
+        "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
 )
-_OptionalProvisionedTypeDef = TypedDict(
-    "_OptionalProvisionedTypeDef",
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
     {
-        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "ConfigurationInfo": ConfigurationInfoTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
-        "ZookeeperConnectString": str,
-        "ZookeeperConnectStringTls": str,
+        "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
 
-class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
     pass
 
 
-BrokerNodeGroupInfoUnionTypeDef = Union[
-    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef
-]
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
+_RequiredProvisionedRequestTypeDef = TypedDict(
+    "_RequiredProvisionedRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
 )
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
+_OptionalProvisionedRequestTypeDef = TypedDict(
+    "_OptionalProvisionedRequestTypeDef",
     {
         "ClientAuthentication": ClientAuthenticationTypeDef,
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
-        "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
 
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+class ProvisionedRequestTypeDef(
+    _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
 
-_RequiredProvisionedRequestTypeDef = TypedDict(
-    "_RequiredProvisionedRequestTypeDef",
+_RequiredProvisionedTypeDef = TypedDict(
+    "_RequiredProvisionedTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
 )
-_OptionalProvisionedRequestTypeDef = TypedDict(
-    "_OptionalProvisionedRequestTypeDef",
+_OptionalProvisionedTypeDef = TypedDict(
+    "_OptionalProvisionedTypeDef",
     {
+        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationTypeDef,
-        "ConfigurationInfo": ConfigurationInfoTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
+        "ZookeeperConnectString": str,
+        "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
 
-class ProvisionedRequestTypeDef(
-    _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
-):
+class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
     pass
 
 
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": str,
@@ -2166,14 +2194,25 @@
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
         "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
+ClusterOperationV2ProvisionedTypeDef = TypedDict(
+    "ClusterOperationV2ProvisionedTypeDef",
+    {
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2183,32 +2222,14 @@
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "ActiveOperationArn": str,
-        "ClusterType": ClusterTypeType,
-        "ClusterArn": str,
-        "ClusterName": str,
-        "CreationTime": datetime,
-        "CurrentVersion": str,
-        "State": ClusterStateType,
-        "StateInfo": StateInfoTypeDef,
-        "Tags": Dict[str, str],
-        "Provisioned": ProvisionedTypeDef,
-        "Serverless": ServerlessTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 _OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
@@ -2224,14 +2245,32 @@
 
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
 
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "ActiveOperationArn": str,
+        "ClusterType": ClusterTypeType,
+        "ClusterArn": str,
+        "ClusterName": str,
+        "CreationTime": datetime,
+        "CurrentVersion": str,
+        "State": ClusterStateType,
+        "StateInfo": StateInfoTypeDef,
+        "Tags": Dict[str, str],
+        "Provisioned": ProvisionedTypeDef,
+        "Serverless": ServerlessTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2241,14 +2280,31 @@
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClusterOperationV2TypeDef = TypedDict(
+    "ClusterOperationV2TypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+        "Provisioned": ClusterOperationV2ProvisionedTypeDef,
+        "Serverless": ClusterOperationV2ServerlessTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2257,7 +2313,15 @@
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DescribeClusterOperationV2ResponseTypeDef = TypedDict(
+    "DescribeClusterOperationV2ResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationV2TypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka/type_defs.pyi` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -45,31 +45,32 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "BlobTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
-    "TlsOutputTypeDef",
-    "UnauthenticatedTypeDef",
     "TlsTypeDef",
+    "UnauthenticatedTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
+    "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
@@ -79,14 +80,15 @@
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
+    "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersV2RequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
     "ListNodesRequestRequestTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
@@ -97,15 +99,14 @@
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
     "VpcConnectivityIamTypeDef",
@@ -141,78 +142,81 @@
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
+    "ListClusterOperationsV2ResponseTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    "ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
     "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
-    "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
+    "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoOutputTypeDef",
     "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
-    "ProvisionedTypeDef",
-    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
+    "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "ClusterTypeDef",
     "CreateClusterV2RequestRequestTypeDef",
+    "ClusterTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
+    "ClusterOperationV2TypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
+    "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
@@ -316,40 +320,31 @@
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
     total=False,
 )
 
-TlsOutputTypeDef = TypedDict(
-    "TlsOutputTypeDef",
+TlsTypeDef = TypedDict(
+    "TlsTypeDef",
     {
-        "CertificateAuthorityArnList": List[str],
+        "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
 UnauthenticatedTypeDef = TypedDict(
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-TlsTypeDef = TypedDict(
-    "TlsTypeDef",
-    {
-        "CertificateAuthorityArnList": Sequence[str],
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 _RequiredClientVpcConnectionTypeDef = TypedDict(
     "_RequiredClientVpcConnectionTypeDef",
     {
         "VpcConnectionArn": str,
     },
 )
 _OptionalClientVpcConnectionTypeDef = TypedDict(
@@ -390,14 +385,28 @@
     "ClusterOperationStepInfoTypeDef",
     {
         "StepStatus": str,
     },
     total=False,
 )
 
+ClusterOperationV2SummaryTypeDef = TypedDict(
+    "ClusterOperationV2SummaryTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+    },
+    total=False,
+)
+
 CompatibleKafkaVersionTypeDef = TypedDict(
     "CompatibleKafkaVersionTypeDef",
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
@@ -506,14 +515,21 @@
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
+DescribeClusterOperationV2RequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationV2RequestRequestTypeDef",
+    {
+        "ClusterOperationArn": str,
+    },
+)
+
 DescribeClusterRequestRequestTypeDef = TypedDict(
     "DescribeClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
@@ -663,14 +679,35 @@
 
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListClusterOperationsV2RequestRequestTypeDef(
+    _RequiredListClusterOperationsV2RequestRequestTypeDef,
+    _OptionalListClusterOperationsV2RequestRequestTypeDef,
+):
+    pass
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -887,31 +924,14 @@
     },
     total=False,
 )
 
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
-_RequiredVpcConfigOutputTypeDef = TypedDict(
-    "_RequiredVpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-    },
-)
-_OptionalVpcConfigOutputTypeDef = TypedDict(
-    "_OptionalVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
-    pass
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1363,14 +1383,23 @@
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
+ListClusterOperationsV2ResponseTypeDef = TypedDict(
+    "ListClusterOperationsV2ResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1525,14 +1554,34 @@
 
 class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
     _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
 ):
     pass
 
+_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
+    _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+):
+    pass
+
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "ClusterNameFilter": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1664,14 +1713,25 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
+VpcConnectionInfoServerlessTypeDef = TypedDict(
+    "VpcConnectionInfoServerlessTypeDef",
+    {
+        "CreationTime": datetime,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "VpcConnectionArn": str,
+    },
+    total=False,
+)
+
 VpcConnectionInfoTypeDef = TypedDict(
     "VpcConnectionInfoTypeDef",
     {
         "VpcConnectionArn": str,
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
         "CreationTime": datetime,
@@ -1752,30 +1812,28 @@
 OpenMonitoringTypeDef = TypedDict(
     "OpenMonitoringTypeDef",
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 
-ClientAuthenticationOutputTypeDef = TypedDict(
-    "ClientAuthenticationOutputTypeDef",
+ClientAuthenticationTypeDef = TypedDict(
+    "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
-        "Tls": TlsOutputTypeDef,
+        "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-ClientAuthenticationTypeDef = TypedDict(
-    "ClientAuthenticationTypeDef",
+ClusterOperationV2ServerlessTypeDef = TypedDict(
+    "ClusterOperationV2ServerlessTypeDef",
     {
-        "Sasl": SaslTypeDef,
-        "Tls": TlsTypeDef,
-        "Unauthenticated": UnauthenticatedTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoServerlessTypeDef,
     },
     total=False,
 )
 
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
@@ -1812,15 +1870,15 @@
     _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
 ):
     pass
 
 _RequiredServerlessTypeDef = TypedDict(
     "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": List[VpcConfigTypeDef],
     },
 )
 _OptionalServerlessTypeDef = TypedDict(
     "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
@@ -1848,17 +1906,14 @@
 )
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
-ClientAuthenticationUnionTypeDef = Union[
-    ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-]
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -1889,38 +1944,14 @@
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoOutputTypeDef",
-    {
-        "ClientSubnets": List[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoOutputTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": List[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": List[str],
-    },
-    total=False,
-)
-
-class BrokerNodeGroupInfoOutputTypeDef(
-    _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
-):
-    pass
-
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
 )
@@ -1948,15 +1979,15 @@
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
         "KafkaVersion": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
@@ -1969,16 +2000,16 @@
     },
 )
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
         "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -1991,43 +2022,14 @@
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-_RequiredProvisionedTypeDef = TypedDict(
-    "_RequiredProvisionedTypeDef",
-    {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
-        "NumberOfBrokerNodes": int,
-    },
-)
-_OptionalProvisionedTypeDef = TypedDict(
-    "_OptionalProvisionedTypeDef",
-    {
-        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-        "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringInfoTypeDef,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "ZookeeperConnectString": str,
-        "ZookeeperConnectStringTls": str,
-        "StorageMode": StorageModeType,
-    },
-    total=False,
-)
-
-class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
-    pass
-
-BrokerNodeGroupInfoUnionTypeDef = Union[
-    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef
-]
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -2076,14 +2078,40 @@
 )
 
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
+_RequiredProvisionedTypeDef = TypedDict(
+    "_RequiredProvisionedTypeDef",
+    {
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "NumberOfBrokerNodes": int,
+    },
+)
+_OptionalProvisionedTypeDef = TypedDict(
+    "_OptionalProvisionedTypeDef",
+    {
+        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+        "EnhancedMonitoring": EnhancedMonitoringType,
+        "OpenMonitoring": OpenMonitoringInfoTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "ZookeeperConnectString": str,
+        "ZookeeperConnectStringTls": str,
+        "StorageMode": StorageModeType,
+    },
+    total=False,
+)
+
+class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
+    pass
+
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": str,
         "ClusterArn": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2095,14 +2123,25 @@
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
         "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
+ClusterOperationV2ProvisionedTypeDef = TypedDict(
+    "ClusterOperationV2ProvisionedTypeDef",
+    {
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2112,32 +2151,14 @@
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "ActiveOperationArn": str,
-        "ClusterType": ClusterTypeType,
-        "ClusterArn": str,
-        "ClusterName": str,
-        "CreationTime": datetime,
-        "CurrentVersion": str,
-        "State": ClusterStateType,
-        "StateInfo": StateInfoTypeDef,
-        "Tags": Dict[str, str],
-        "Provisioned": ProvisionedTypeDef,
-        "Serverless": ServerlessTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 _OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
@@ -2151,14 +2172,32 @@
 )
 
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "ActiveOperationArn": str,
+        "ClusterType": ClusterTypeType,
+        "ClusterArn": str,
+        "ClusterName": str,
+        "CreationTime": datetime,
+        "CurrentVersion": str,
+        "State": ClusterStateType,
+        "StateInfo": StateInfoTypeDef,
+        "Tags": Dict[str, str],
+        "Provisioned": ProvisionedTypeDef,
+        "Serverless": ServerlessTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2168,14 +2207,31 @@
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClusterOperationV2TypeDef = TypedDict(
+    "ClusterOperationV2TypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+        "Provisioned": ClusterOperationV2ProvisionedTypeDef,
+        "Serverless": ClusterOperationV2ServerlessTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2184,7 +2240,15 @@
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DescribeClusterOperationV2ResponseTypeDef = TypedDict(
+    "DescribeClusterOperationV2ResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationV2TypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-kafka-2.5.2.post1/types_aiobotocore_kafka.egg-info/SOURCES.txt` & `types-aiobotocore-kafka-2.5.2.post2/types_aiobotocore_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

