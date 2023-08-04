# Comparing `tmp/types-aiobotocore-finspace-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-finspace-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-finspace-2.5.2.post1.tar` & `types-aiobotocore-finspace-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26537 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-08-02 14:38:43.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36840 2023-08-02 14:38:42.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:41.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.281585 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:18.000000 types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.588185 types-aiobotocore-finspace-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-04 12:00:53.584185 types-aiobotocore-finspace-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:53.588185 types-aiobotocore-finspace-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.584185 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-04 11:46:12.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-08-04 11:46:12.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-08-04 11:46:12.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:11.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.584185 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:53.000000 types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-2.5.2.post1/LICENSE` & `types-aiobotocore-finspace-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/setup.py` & `types-aiobotocore-finspace-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__init__.pyi` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/__main__.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.finspace 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.finspace 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersUnionTypeDef,
+    FederationParametersTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationUnionTypeDef,
+    KxDatabaseConfigurationTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,15 +57,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -132,15 +132,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersUnionTypeDef = ...,
+        federationParameters: FederationParametersTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -168,19 +168,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
+        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -466,29 +466,29 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersUnionTypeDef = ...
+        federationParameters: FederationParametersTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
 
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
+        databases: Sequence[KxDatabaseConfigurationTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/client.pyi` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersUnionTypeDef,
+    FederationParametersTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationUnionTypeDef,
+    KxDatabaseConfigurationTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,15 +57,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -125,15 +125,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersUnionTypeDef = ...,
+        federationParameters: FederationParametersTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -159,19 +159,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
+        databases: Sequence[KxDatabaseConfigurationTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        vpcConfiguration: VpcConfigurationTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -430,28 +430,28 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersUnionTypeDef = ...
+        federationParameters: FederationParametersTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
+        databases: Sequence[KxDatabaseConfigurationTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/literals.pyi` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/paginator.pyi` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.py` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_finspace.type_defs import AutoScalingConfigurationTypeDef
 
     data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -47,36 +47,33 @@
     "SuperuserParametersTypeDef",
     "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
     "CreateKxUserRequestRequestTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
-    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
-    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
@@ -88,52 +85,48 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
+    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserResponseTypeDef",
     "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseResponseTypeDef",
     "GetKxUserResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "EnvironmentTypeDef",
-    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
-    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
     "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
-    "KxDatabaseConfigurationUnionTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
@@ -259,25 +252,14 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "vpcId": str,
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "ipAddressType": Literal["IP_V4"],
-    },
-    total=False,
-)
-
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -404,27 +386,14 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-FederationParametersOutputTypeDef = TypedDict(
-    "FederationParametersOutputTypeDef",
-    {
-        "samlMetadataDocument": str,
-        "samlMetadataURL": str,
-        "applicationCallBackURL": str,
-        "federationURN": str,
-        "federationProviderName": str,
-        "attributeMap": Dict[str, str],
-    },
-    total=False,
-)
-
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -512,22 +481,14 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
-KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
-    "KxDatabaseCacheConfigurationOutputTypeDef",
-    {
-        "cacheType": str,
-        "dbPaths": List[str],
-    },
-)
-
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -805,14 +766,33 @@
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -1001,37 +981,14 @@
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-FederationParametersUnionTypeDef = Union[
-    FederationParametersTypeDef, FederationParametersOutputTypeDef
-]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1160,36 +1117,14 @@
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKxDatabaseConfigurationOutputTypeDef",
-    {
-        "databaseName": str,
-    },
-)
-_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKxDatabaseConfigurationOutputTypeDef",
-    {
-        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
-        "changesetId": str,
-    },
-    total=False,
-)
-
-
-class KxDatabaseConfigurationOutputTypeDef(
-    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1273,116 +1208,113 @@
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
-        "status": KxClusterStatusType,
-        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
+
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
+        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "databases": List[KxDatabaseConfigurationTypeDef],
         "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KxDatabaseConfigurationUnionTypeDef = Union[
-    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
-]
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
+        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace/type_defs.pyi` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_finspace.type_defs import AutoScalingConfigurationTypeDef
 
     data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChangesetStatusType,
     ChangeTypeType,
     EnvironmentStatusType,
     ErrorDetailsType,
     FederationModeType,
@@ -46,36 +46,33 @@
     "SuperuserParametersTypeDef",
     "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
     "CreateKxUserRequestRequestTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
-    "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
-    "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
@@ -87,52 +84,48 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
+    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserResponseTypeDef",
     "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseResponseTypeDef",
     "GetKxUserResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
-    "VpcConfigurationUnionTypeDef",
-    "EnvironmentTypeDef",
-    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
-    "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
     "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
+    "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
-    "KxDatabaseConfigurationUnionTypeDef",
-    "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
@@ -256,25 +249,14 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "vpcId": str,
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "ipAddressType": Literal["IP_V4"],
-    },
-    total=False,
-)
-
 _RequiredCreateKxDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -393,27 +375,14 @@
     "DeleteKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-FederationParametersOutputTypeDef = TypedDict(
-    "FederationParametersOutputTypeDef",
-    {
-        "samlMetadataDocument": str,
-        "samlMetadataURL": str,
-        "applicationCallBackURL": str,
-        "federationURN": str,
-        "federationProviderName": str,
-        "attributeMap": Dict[str, str],
-    },
-    total=False,
-)
-
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -501,22 +470,14 @@
         "availabilityZoneId": str,
         "lastModifiedTimestamp": datetime,
         "createdTimestamp": datetime,
     },
     total=False,
 )
 
-KxDatabaseCacheConfigurationOutputTypeDef = TypedDict(
-    "KxDatabaseCacheConfigurationOutputTypeDef",
-    {
-        "cacheType": str,
-        "dbPaths": List[str],
-    },
-)
-
 KxDatabaseCacheConfigurationTypeDef = TypedDict(
     "KxDatabaseCacheConfigurationTypeDef",
     {
         "cacheType": str,
         "dbPaths": Sequence[str],
     },
 )
@@ -778,14 +739,33 @@
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
     },
 )
 
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "name": str,
+        "environmentId": str,
+        "awsAccountId": str,
+        "status": EnvironmentStatusType,
+        "environmentUrl": str,
+        "description": str,
+        "environmentArn": str,
+        "sageMakerStudioDomainUrl": str,
+        "kmsKeyId": str,
+        "dedicatedServiceAccountId": str,
+        "federationMode": FederationModeType,
+        "federationParameters": FederationParametersTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -970,37 +950,14 @@
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "name": str,
-        "environmentId": str,
-        "awsAccountId": str,
-        "status": EnvironmentStatusType,
-        "environmentUrl": str,
-        "description": str,
-        "environmentArn": str,
-        "sageMakerStudioDomainUrl": str,
-        "kmsKeyId": str,
-        "dedicatedServiceAccountId": str,
-        "federationMode": FederationModeType,
-        "federationParameters": FederationParametersOutputTypeDef,
-    },
-    total=False,
-)
-
-FederationParametersUnionTypeDef = Union[
-    FederationParametersTypeDef, FederationParametersOutputTypeDef
-]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1127,34 +1084,14 @@
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKxDatabaseConfigurationOutputTypeDef",
-    {
-        "databaseName": str,
-    },
-)
-_OptionalKxDatabaseConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKxDatabaseConfigurationOutputTypeDef",
-    {
-        "cacheConfigurations": List[KxDatabaseCacheConfigurationOutputTypeDef],
-        "changesetId": str,
-    },
-    total=False,
-)
-
-class KxDatabaseConfigurationOutputTypeDef(
-    _RequiredKxDatabaseConfigurationOutputTypeDef, _OptionalKxDatabaseConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
     },
 )
 _OptionalKxDatabaseConfigurationTypeDef = TypedDict(
@@ -1236,114 +1173,111 @@
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateKxClusterResponseTypeDef = TypedDict(
-    "CreateKxClusterResponseTypeDef",
+_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
-        "status": KxClusterStatusType,
-        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "azMode": KxAzModeType,
+    },
+)
+_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKxClusterRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
+        "clusterDescription": str,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
-        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
-        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetKxClusterResponseTypeDef = TypedDict(
-    "GetKxClusterResponseTypeDef",
+class CreateKxClusterRequestRequestTypeDef(
+    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
+):
+    pass
+
+CreateKxClusterResponseTypeDef = TypedDict(
+    "CreateKxClusterResponseTypeDef",
     {
+        "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "databases": List[KxDatabaseConfigurationOutputTypeDef],
+        "databases": List[KxDatabaseConfigurationTypeDef],
         "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KxDatabaseConfigurationUnionTypeDef = Union[
-    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
-]
-_RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKxClusterRequestRequestTypeDef",
+GetKxClusterResponseTypeDef = TypedDict(
+    "GetKxClusterResponseTypeDef",
     {
-        "environmentId": str,
+        "status": KxClusterStatusType,
+        "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
-        "capacityConfiguration": CapacityConfigurationTypeDef,
-        "releaseLabel": str,
-        "azMode": KxAzModeType,
-    },
-)
-_OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKxClusterRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
-        "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
+        "databases": List[KxDatabaseConfigurationTypeDef],
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
+        "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
-        "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
+        "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
+        "azMode": KxAzModeType,
         "availabilityZoneId": str,
-        "tags": Mapping[str, str],
+        "createdTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateKxClusterRequestRequestTypeDef(
-    _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
+        "databases": Sequence[KxDatabaseConfigurationTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `types-aiobotocore-finspace-2.5.2.post1/types_aiobotocore_finspace.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-2.5.2.post2/types_aiobotocore_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

