# Comparing `tmp/types-aiobotocore-greengrass-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-greengrass-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrass-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrass-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-greengrass-2.5.2.post1.tar` & `types-aiobotocore-greengrass-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.661576 types-aiobotocore-greengrass-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-08-02 14:52:21.661576 types-aiobotocore-greengrass-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27597 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.661576 types-aiobotocore-greengrass-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.661576 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72484 2023-08-02 14:39:41.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72364 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-02 14:39:42.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-02 14:39:41.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-08-02 14:39:41.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-08-02 14:39:41.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94831 2023-08-02 14:39:43.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94711 2023-08-02 14:39:42.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:39.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.661576 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:21.000000 types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.496366 types-aiobotocore-greengrass-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-08-04 12:00:58.488365 types-aiobotocore-greengrass-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.496366 types-aiobotocore-greengrass-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.488365 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72384 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72264 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 11:47:12.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-04 11:47:12.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88853 2023-08-04 11:47:13.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88736 2023-08-04 11:47:13.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:47:11.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.488365 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:58.000000 types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/LICENSE` & `types-aiobotocore-greengrass-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/setup.py` & `types-aiobotocore-greengrass-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrass",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Greengrass 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__init__.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__init__.pyi` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/__main__.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Greengrass 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Greengrass 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/client.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
-    ConnectorDefinitionVersionUnionTypeDef,
-    ConnectorUnionTypeDef,
-    CoreDefinitionVersionUnionTypeDef,
+    ConnectorDefinitionVersionTypeDef,
+    ConnectorTypeDef,
+    CoreDefinitionVersionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDeviceDefinitionResponseTypeDef,
@@ -71,22 +71,22 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DeviceDefinitionVersionUnionTypeDef,
+    DeviceDefinitionVersionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
-    FunctionDefinitionVersionUnionTypeDef,
-    FunctionUnionTypeDef,
+    FunctionDefinitionVersionTypeDef,
+    FunctionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
@@ -125,21 +125,21 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggerDefinitionVersionUnionTypeDef,
+    LoggerDefinitionVersionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
-    ResourceDefinitionVersionUnionTypeDef,
-    ResourceUnionTypeDef,
+    ResourceDefinitionVersionTypeDef,
+    ResourceTypeDef,
     StartBulkDeploymentResponseTypeDef,
-    SubscriptionDefinitionVersionUnionTypeDef,
+    SubscriptionDefinitionVersionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -218,15 +218,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#close)
         """
 
     async def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ConnectorDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
@@ -234,28 +234,28 @@
         """
 
     async def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorUnionTypeDef] = ...
+        Connectors: Sequence[ConnectorTypeDef] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition_version)
         """
 
     async def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: CoreDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: CoreDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -292,15 +292,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_deployment)
         """
 
     async def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: DeviceDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: DeviceDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -321,15 +321,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition_version)
         """
 
     async def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: FunctionDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: FunctionDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -339,15 +339,15 @@
 
     async def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionUnionTypeDef] = ...
+        Functions: Sequence[FunctionTypeDef] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_function_definition_version)
         """
@@ -397,15 +397,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group_version)
         """
 
     async def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: LoggerDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: LoggerDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -426,15 +426,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition_version)
         """
 
     async def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ResourceDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: ResourceDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -443,15 +443,15 @@
         """
 
     async def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceUnionTypeDef] = ...
+        Resources: Sequence[ResourceTypeDef] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_resource_definition_version)
         """
@@ -476,15 +476,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_software_update_job)
         """
 
     async def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: SubscriptionDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/client.pyi` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
-    ConnectorDefinitionVersionUnionTypeDef,
-    ConnectorUnionTypeDef,
-    CoreDefinitionVersionUnionTypeDef,
+    ConnectorDefinitionVersionTypeDef,
+    ConnectorTypeDef,
+    CoreDefinitionVersionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDeviceDefinitionResponseTypeDef,
@@ -71,22 +71,22 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DeviceDefinitionVersionUnionTypeDef,
+    DeviceDefinitionVersionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
-    FunctionDefinitionVersionUnionTypeDef,
-    FunctionUnionTypeDef,
+    FunctionDefinitionVersionTypeDef,
+    FunctionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
@@ -125,21 +125,21 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggerDefinitionVersionUnionTypeDef,
+    LoggerDefinitionVersionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
-    ResourceDefinitionVersionUnionTypeDef,
-    ResourceUnionTypeDef,
+    ResourceDefinitionVersionTypeDef,
+    ResourceTypeDef,
     StartBulkDeploymentResponseTypeDef,
-    SubscriptionDefinitionVersionUnionTypeDef,
+    SubscriptionDefinitionVersionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -209,42 +209,42 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#close)
         """
     async def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ConnectorDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: ConnectorDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition)
         """
     async def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[ConnectorUnionTypeDef] = ...
+        Connectors: Sequence[ConnectorTypeDef] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_connector_definition_version)
         """
     async def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: CoreDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: CoreDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -278,15 +278,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_deployment)
         """
     async def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: DeviceDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: DeviceDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -305,15 +305,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_device_definition_version)
         """
     async def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: FunctionDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: FunctionDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -322,15 +322,15 @@
         """
     async def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[FunctionUnionTypeDef] = ...
+        Functions: Sequence[FunctionTypeDef] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_function_definition_version)
         """
@@ -376,15 +376,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_group_version)
         """
     async def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: LoggerDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: LoggerDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -403,15 +403,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_logger_definition_version)
         """
     async def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: ResourceDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: ResourceDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -419,15 +419,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_resource_definition)
         """
     async def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[ResourceUnionTypeDef] = ...
+        Resources: Sequence[ResourceTypeDef] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_resource_definition_version)
         """
@@ -450,15 +450,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_software_update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/client/#create_software_update_job)
         """
     async def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: SubscriptionDefinitionVersionUnionTypeDef = ...,
+        InitialVersion: SubscriptionDefinitionVersionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/literals.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/literals.pyi` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/paginator.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/paginator.pyi` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/type_defs.py` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
     data: AssociateRoleToGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BulkDeploymentStatusType,
     ConfigurationSyncStatusType,
     DeploymentTypeType,
     EncodingTypeType,
     FunctionIsolationModeType,
@@ -32,24 +32,22 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
     "ConnectivityInfoTypeDef",
-    "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
     "CoreTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeviceTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
     "GroupVersionTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
@@ -115,15 +113,14 @@
     "ListLoggerDefinitionsRequestRequestTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
-    "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
@@ -180,30 +177,25 @@
     "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
-    "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
-    "ConnectorUnionTypeDef",
-    "CoreDefinitionVersionOutputTypeDef",
+    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
-    "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
-    "LoggerDefinitionVersionOutputTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
-    "SubscriptionDefinitionVersionOutputTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
@@ -243,56 +235,39 @@
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
-    "GetConnectorDefinitionVersionResponseTypeDef",
-    "ConnectorDefinitionVersionUnionTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
-    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
-    "GetCoreDefinitionVersionResponseTypeDef",
-    "CoreDefinitionVersionUnionTypeDef",
+    "GetConnectorDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
+    "GetCoreDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
-    "DeviceDefinitionVersionUnionTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
-    "LoggerDefinitionVersionUnionTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "SubscriptionDefinitionVersionUnionTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "FunctionDefaultConfigTypeDef",
-    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
-    "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
-    "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "FunctionOutputTypeDef",
     "FunctionTypeDef",
-    "ResourceDefinitionVersionOutputTypeDef",
+    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
-    "ResourceUnionTypeDef",
-    "FunctionDefinitionVersionOutputTypeDef",
+    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
-    "FunctionUnionTypeDef",
-    "GetResourceDefinitionVersionResponseTypeDef",
     "CreateResourceDefinitionRequestRequestTypeDef",
-    "ResourceDefinitionVersionUnionTypeDef",
-    "CreateResourceDefinitionVersionRequestRequestTypeDef",
-    "GetFunctionDefinitionVersionResponseTypeDef",
+    "GetResourceDefinitionVersionResponseTypeDef",
     "CreateFunctionDefinitionRequestRequestTypeDef",
-    "FunctionDefinitionVersionUnionTypeDef",
-    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
+    "GetFunctionDefinitionVersionResponseTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -353,34 +328,14 @@
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
     },
     total=False,
 )
 
-_RequiredConnectorOutputTypeDef = TypedDict(
-    "_RequiredConnectorOutputTypeDef",
-    {
-        "ConnectorArn": str,
-        "Id": str,
-    },
-)
-_OptionalConnectorOutputTypeDef = TypedDict(
-    "_OptionalConnectorOutputTypeDef",
-    {
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
-    pass
-
-
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -388,19 +343,17 @@
     "_OptionalConnectorTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
-
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -409,19 +362,17 @@
     "_OptionalCoreTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
-
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
 )
@@ -431,21 +382,19 @@
         "AmznClientToken": str,
         "DeploymentId": str,
         "GroupVersionId": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -454,41 +403,37 @@
     "_OptionalDeviceTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
-
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "AmznClientToken": str,
     },
     total=False,
 )
 
-
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
         "FunctionDefinitionVersionArn": str,
@@ -516,22 +461,20 @@
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
-
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
         "Type": LoggerTypeType,
@@ -541,19 +484,17 @@
     "_OptionalLoggerTypeDef",
     {
         "Space": int,
     },
     total=False,
 )
 
-
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
-
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
         "UpdateTargetsArchitecture": UpdateTargetsArchitectureType,
@@ -565,22 +506,20 @@
     {
         "AmznClientToken": str,
         "UpdateAgentLogLevel": UpdateAgentLogLevelType,
     },
     total=False,
 )
 
-
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
-
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
@@ -687,21 +626,19 @@
     "_OptionalResourceAccessPolicyTypeDef",
     {
         "Permission": PermissionType,
     },
     total=False,
 )
 
-
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
-
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
     total=False,
@@ -746,22 +683,20 @@
     "_OptionalGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalGetConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
@@ -799,22 +734,20 @@
     "_OptionalGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalGetDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
@@ -829,22 +762,20 @@
     "_OptionalGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
@@ -889,22 +820,20 @@
     "_OptionalGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalGetLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
@@ -934,22 +863,20 @@
     "_OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 
@@ -1006,22 +933,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
-
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1038,22 +963,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListConnectorDefinitionVersionsRequestRequestTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 VersionInformationTypeDef = TypedDict(
     "VersionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
@@ -1081,22 +1004,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1113,21 +1034,19 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1135,22 +1054,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1167,22 +1084,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1206,21 +1121,19 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1237,22 +1150,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1269,22 +1180,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1301,22 +1210,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1340,30 +1247,19 @@
     {
         "AmznClientToken": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
-SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
-    "SecretsManagerSecretResourceDataOutputTypeDef",
-    {
-        "ARN": str,
-        "AdditionalStagingLabelsToDownload": List[str],
-    },
-    total=False,
-)
-
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
@@ -1387,21 +1283,19 @@
     "_OptionalTelemetryConfigurationTypeDef",
     {
         "ConfigurationSyncStatus": ConfigurationSyncStatusType,
     },
     total=False,
 )
 
-
 class TelemetryConfigurationTypeDef(
     _RequiredTelemetryConfigurationTypeDef, _OptionalTelemetryConfigurationTypeDef
 ):
     pass
 
-
 _RequiredStartBulkDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDeploymentRequestRequestTypeDef",
     {
         "ExecutionRoleArn": str,
         "InputFileUri": str,
     },
 )
@@ -1410,22 +1304,20 @@
     {
         "AmznClientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1439,21 +1331,19 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 TelemetryConfigurationUpdateTypeDef = TypedDict(
     "TelemetryConfigurationUpdateTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 
@@ -1475,197 +1365,179 @@
     "_OptionalUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorDefinitionRequestRequestTypeDef(
     _RequiredUpdateConnectorDefinitionRequestRequestTypeDef,
     _OptionalUpdateConnectorDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateCoreDefinitionRequestRequestTypeDef(
     _RequiredUpdateCoreDefinitionRequestRequestTypeDef,
     _OptionalUpdateCoreDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateDeviceDefinitionRequestRequestTypeDef(
     _RequiredUpdateDeviceDefinitionRequestRequestTypeDef,
     _OptionalUpdateDeviceDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateFunctionDefinitionRequestRequestTypeDef(
     _RequiredUpdateFunctionDefinitionRequestRequestTypeDef,
     _OptionalUpdateFunctionDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "CertificateExpiryInMilliseconds": str,
     },
     total=False,
 )
 
-
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateLoggerDefinitionRequestRequestTypeDef(
     _RequiredUpdateLoggerDefinitionRequestRequestTypeDef,
     _OptionalUpdateLoggerDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateResourceDefinitionRequestRequestTypeDef(
     _RequiredUpdateResourceDefinitionRequestRequestTypeDef,
     _OptionalUpdateResourceDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateRoleToGroupResponseTypeDef = TypedDict(
     "AssociateRoleToGroupResponseTypeDef",
     {
         "AssociatedAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2199,47 +2071,49 @@
     "_OptionalUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ConnectivityInfo": Sequence[ConnectivityInfoTypeDef],
     },
     total=False,
 )
 
-
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
-
-ConnectorDefinitionVersionOutputTypeDef = TypedDict(
-    "ConnectorDefinitionVersionOutputTypeDef",
-    {
-        "Connectors": List[ConnectorOutputTypeDef],
-    },
-    total=False,
-)
-
 ConnectorDefinitionVersionTypeDef = TypedDict(
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
-ConnectorUnionTypeDef = Union[ConnectorTypeDef, ConnectorOutputTypeDef]
-CoreDefinitionVersionOutputTypeDef = TypedDict(
-    "CoreDefinitionVersionOutputTypeDef",
+_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
     {
-        "Cores": List[CoreTypeDef],
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
+class CreateConnectorDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
@@ -2255,22 +2129,20 @@
     {
         "AmznClientToken": str,
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
 
-
 class CreateCoreDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateCoreDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateCoreDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2278,30 +2150,20 @@
     {
         "AmznClientToken": str,
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-DeviceDefinitionVersionOutputTypeDef = TypedDict(
-    "DeviceDefinitionVersionOutputTypeDef",
-    {
-        "Devices": List[DeviceTypeDef],
-    },
-    total=False,
-)
-
 DeviceDefinitionVersionTypeDef = TypedDict(
     "DeviceDefinitionVersionTypeDef",
     {
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
@@ -2318,21 +2180,19 @@
         "AmznClientToken": str,
         "InitialVersion": GroupVersionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 GetGroupVersionResponseTypeDef = TypedDict(
     "GetGroupVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": GroupVersionTypeDef,
         "Id": str,
@@ -2352,30 +2212,20 @@
     {
         "AmznClientToken": str,
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
 
-
 class CreateLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-LoggerDefinitionVersionOutputTypeDef = TypedDict(
-    "LoggerDefinitionVersionOutputTypeDef",
-    {
-        "Loggers": List[LoggerTypeDef],
-    },
-    total=False,
-)
-
 LoggerDefinitionVersionTypeDef = TypedDict(
     "LoggerDefinitionVersionTypeDef",
     {
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
@@ -2391,30 +2241,20 @@
     {
         "AmznClientToken": str,
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
-
 class CreateSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
-    "SubscriptionDefinitionVersionOutputTypeDef",
-    {
-        "Subscriptions": List[SubscriptionTypeDef],
-    },
-    total=False,
-)
-
 SubscriptionDefinitionVersionTypeDef = TypedDict(
     "SubscriptionDefinitionVersionTypeDef",
     {
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
@@ -2555,22 +2395,20 @@
     "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
 ):
     pass
 
-
 ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
     "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2585,22 +2423,20 @@
     "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2615,22 +2451,20 @@
     "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
     _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
     "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2645,44 +2479,40 @@
     "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
     _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
     _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
     "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2697,22 +2527,20 @@
     "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2727,22 +2555,20 @@
     "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
     _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "ListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2757,22 +2583,20 @@
     "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2787,22 +2611,20 @@
     "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
     _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
     "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2817,22 +2639,20 @@
     "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2947,114 +2767,70 @@
     "_OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationUpdateTypeDef,
     },
     total=False,
 )
 
-
 class UpdateThingRuntimeConfigurationRequestRequestTypeDef(
     _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef,
     _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": ConnectorDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConnectorDefinitionVersionUnionTypeDef = Union[
-    ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
-]
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Connectors": Sequence[ConnectorUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateConnectorDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-
-GetCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionVersionResponseTypeDef",
+GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": CoreDefinitionVersionOutputTypeDef,
+        "Definition": ConnectorDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoreDefinitionVersionUnionTypeDef = Union[
-    CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
-]
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+GetCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Definition": CoreDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3065,24 +2841,22 @@
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-DeviceDefinitionVersionUnionTypeDef = Union[
-    DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
-]
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Definition": DeviceDefinitionVersionTypeDef,
         "Id": str,
+        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
@@ -3091,25 +2865,21 @@
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-LoggerDefinitionVersionUnionTypeDef = Union[
-    LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
-]
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
+        "Definition": LoggerDefinitionVersionTypeDef,
         "Id": str,
-        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
@@ -3118,32 +2888,31 @@
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-SubscriptionDefinitionVersionUnionTypeDef = Union[
-    SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
-]
-FunctionDefaultConfigTypeDef = TypedDict(
-    "FunctionDefaultConfigTypeDef",
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigTypeDef,
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": SubscriptionDefinitionVersionTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
-    "FunctionConfigurationEnvironmentOutputTypeDef",
+FunctionDefaultConfigTypeDef = TypedDict(
+    "FunctionDefaultConfigTypeDef",
     {
-        "AccessSysfs": bool,
-        "Execution": FunctionExecutionConfigTypeDef,
-        "ResourceAccessPolicies": List[ResourceAccessPolicyTypeDef],
-        "Variables": Dict[str, str],
+        "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
 
 FunctionConfigurationEnvironmentTypeDef = TypedDict(
     "FunctionConfigurationEnvironmentTypeDef",
     {
@@ -3151,28 +2920,14 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
-ResourceDataContainerOutputTypeDef = TypedDict(
-    "ResourceDataContainerOutputTypeDef",
-    {
-        "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
-        "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
-        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
-        "SageMakerMachineLearningModelResourceData": (
-            SageMakerMachineLearningModelResourceDataTypeDef
-        ),
-        "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
@@ -3187,29 +2942,14 @@
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionConfigurationOutputTypeDef = TypedDict(
-    "FunctionConfigurationOutputTypeDef",
-    {
-        "EncodingType": EncodingTypeType,
-        "Environment": FunctionConfigurationEnvironmentOutputTypeDef,
-        "ExecArgs": str,
-        "Executable": str,
-        "MemorySize": int,
-        "Pinned": bool,
-        "Timeout": int,
-        "FunctionRuntimeOverride": str,
-    },
-    total=False,
-)
-
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
         "Environment": FunctionConfigurationEnvironmentTypeDef,
         "ExecArgs": str,
         "Executable": str,
@@ -3217,52 +2957,23 @@
         "Pinned": bool,
         "Timeout": int,
         "FunctionRuntimeOverride": str,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "ResourceDataContainer": ResourceDataContainerOutputTypeDef,
-    },
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceDataContainer": ResourceDataContainerTypeDef,
     },
 )
 
-_RequiredFunctionOutputTypeDef = TypedDict(
-    "_RequiredFunctionOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalFunctionOutputTypeDef = TypedDict(
-    "_OptionalFunctionOutputTypeDef",
-    {
-        "FunctionArn": str,
-        "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
-    pass
-
-
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -3270,112 +2981,95 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
-
-ResourceDefinitionVersionOutputTypeDef = TypedDict(
-    "ResourceDefinitionVersionOutputTypeDef",
+_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
-        "Resources": List[ResourceOutputTypeDef],
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+class CreateResourceDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
-FunctionDefinitionVersionOutputTypeDef = TypedDict(
-    "FunctionDefinitionVersionOutputTypeDef",
+_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": List[FunctionOutputTypeDef],
+        "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
+class CreateFunctionDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
-FunctionUnionTypeDef = Union[FunctionTypeDef, FunctionOutputTypeDef]
-GetResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": ResourceDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResourceDefinitionVersionUnionTypeDef = Union[
-    ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
-]
-_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateResourceDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-
-GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionVersionResponseTypeDef",
+GetResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": FunctionDefinitionVersionOutputTypeDef,
+        "Definition": ResourceDefinitionVersionTypeDef,
         "Id": str,
-        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
@@ -3384,32 +3078,19 @@
         "InitialVersion": FunctionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-FunctionDefinitionVersionUnionTypeDef = Union[
-    FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
-]
-_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
+GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionVersionResponseTypeDef",
     {
-        "AmznClientToken": str,
-        "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[FunctionUnionTypeDef],
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": FunctionDefinitionVersionTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-
-class CreateFunctionDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass/type_defs.pyi` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
     data: AssociateRoleToGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BulkDeploymentStatusType,
     ConfigurationSyncStatusType,
     DeploymentTypeType,
     EncodingTypeType,
     FunctionIsolationModeType,
@@ -32,23 +32,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
     "ConnectivityInfoTypeDef",
-    "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
     "CoreTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "DeviceTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
     "GroupVersionTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
@@ -114,15 +114,14 @@
     "ListLoggerDefinitionsRequestRequestTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
-    "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
@@ -179,30 +178,25 @@
     "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
-    "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
-    "ConnectorUnionTypeDef",
-    "CoreDefinitionVersionOutputTypeDef",
+    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
-    "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
-    "LoggerDefinitionVersionOutputTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
-    "SubscriptionDefinitionVersionOutputTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
@@ -242,56 +236,39 @@
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
-    "GetConnectorDefinitionVersionResponseTypeDef",
-    "ConnectorDefinitionVersionUnionTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
-    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
-    "GetCoreDefinitionVersionResponseTypeDef",
-    "CoreDefinitionVersionUnionTypeDef",
+    "GetConnectorDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
+    "GetCoreDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
-    "DeviceDefinitionVersionUnionTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
-    "LoggerDefinitionVersionUnionTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "SubscriptionDefinitionVersionUnionTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     "FunctionDefaultConfigTypeDef",
-    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
-    "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
-    "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "FunctionOutputTypeDef",
     "FunctionTypeDef",
-    "ResourceDefinitionVersionOutputTypeDef",
+    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
-    "ResourceUnionTypeDef",
-    "FunctionDefinitionVersionOutputTypeDef",
+    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
-    "FunctionUnionTypeDef",
-    "GetResourceDefinitionVersionResponseTypeDef",
     "CreateResourceDefinitionRequestRequestTypeDef",
-    "ResourceDefinitionVersionUnionTypeDef",
-    "CreateResourceDefinitionVersionRequestRequestTypeDef",
-    "GetFunctionDefinitionVersionResponseTypeDef",
+    "GetResourceDefinitionVersionResponseTypeDef",
     "CreateFunctionDefinitionRequestRequestTypeDef",
-    "FunctionDefinitionVersionUnionTypeDef",
-    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
+    "GetFunctionDefinitionVersionResponseTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -352,32 +329,14 @@
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
     },
     total=False,
 )
 
-_RequiredConnectorOutputTypeDef = TypedDict(
-    "_RequiredConnectorOutputTypeDef",
-    {
-        "ConnectorArn": str,
-        "Id": str,
-    },
-)
-_OptionalConnectorOutputTypeDef = TypedDict(
-    "_OptionalConnectorOutputTypeDef",
-    {
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
-    pass
-
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -385,17 +344,19 @@
     "_OptionalConnectorTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
+
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -404,17 +365,19 @@
     "_OptionalCoreTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
+
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
 )
@@ -424,19 +387,21 @@
         "AmznClientToken": str,
         "DeploymentId": str,
         "GroupVersionId": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -445,37 +410,41 @@
     "_OptionalDeviceTypeDef",
     {
         "SyncShadow": bool,
     },
     total=False,
 )
 
+
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "AmznClientToken": str,
     },
     total=False,
 )
 
+
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
         "FunctionDefinitionVersionArn": str,
@@ -503,20 +472,22 @@
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
+
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
         "Type": LoggerTypeType,
@@ -526,17 +497,19 @@
     "_OptionalLoggerTypeDef",
     {
         "Space": int,
     },
     total=False,
 )
 
+
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
+
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
         "UpdateTargetsArchitecture": UpdateTargetsArchitectureType,
@@ -548,20 +521,22 @@
     {
         "AmznClientToken": str,
         "UpdateAgentLogLevel": UpdateAgentLogLevelType,
     },
     total=False,
 )
 
+
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
+
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
@@ -668,19 +643,21 @@
     "_OptionalResourceAccessPolicyTypeDef",
     {
         "Permission": PermissionType,
     },
     total=False,
 )
 
+
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
+
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
     total=False,
@@ -725,20 +702,22 @@
     "_OptionalGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalGetConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
@@ -776,20 +755,22 @@
     "_OptionalGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalGetDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
@@ -804,20 +785,22 @@
     "_OptionalGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFunctionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetFunctionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
@@ -862,20 +845,22 @@
     "_OptionalGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalGetLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
@@ -905,20 +890,22 @@
     "_OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalGetSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 
@@ -975,20 +962,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
+
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1005,20 +994,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListConnectorDefinitionVersionsRequestRequestTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 VersionInformationTypeDef = TypedDict(
     "VersionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
@@ -1046,20 +1037,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1076,19 +1069,21 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1096,20 +1091,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1126,20 +1123,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1163,19 +1162,21 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
+
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1192,20 +1193,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1222,20 +1225,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1252,20 +1257,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1289,27 +1296,20 @@
     {
         "AmznClientToken": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
-SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
-    "SecretsManagerSecretResourceDataOutputTypeDef",
-    {
-        "ARN": str,
-        "AdditionalStagingLabelsToDownload": List[str],
-    },
-    total=False,
-)
 
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
@@ -1334,19 +1334,21 @@
     "_OptionalTelemetryConfigurationTypeDef",
     {
         "ConfigurationSyncStatus": ConfigurationSyncStatusType,
     },
     total=False,
 )
 
+
 class TelemetryConfigurationTypeDef(
     _RequiredTelemetryConfigurationTypeDef, _OptionalTelemetryConfigurationTypeDef
 ):
     pass
 
+
 _RequiredStartBulkDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDeploymentRequestRequestTypeDef",
     {
         "ExecutionRoleArn": str,
         "InputFileUri": str,
     },
 )
@@ -1355,20 +1357,22 @@
     {
         "AmznClientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1382,19 +1386,21 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 TelemetryConfigurationUpdateTypeDef = TypedDict(
     "TelemetryConfigurationUpdateTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 
@@ -1416,179 +1422,197 @@
     "_OptionalUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorDefinitionRequestRequestTypeDef(
     _RequiredUpdateConnectorDefinitionRequestRequestTypeDef,
     _OptionalUpdateConnectorDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalUpdateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateCoreDefinitionRequestRequestTypeDef(
     _RequiredUpdateCoreDefinitionRequestRequestTypeDef,
     _OptionalUpdateCoreDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalUpdateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDeviceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateDeviceDefinitionRequestRequestTypeDef(
     _RequiredUpdateDeviceDefinitionRequestRequestTypeDef,
     _OptionalUpdateDeviceDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalUpdateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFunctionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateFunctionDefinitionRequestRequestTypeDef(
     _RequiredUpdateFunctionDefinitionRequestRequestTypeDef,
     _OptionalUpdateFunctionDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "CertificateExpiryInMilliseconds": str,
     },
     total=False,
 )
 
+
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalUpdateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggerDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateLoggerDefinitionRequestRequestTypeDef(
     _RequiredUpdateLoggerDefinitionRequestRequestTypeDef,
     _OptionalUpdateLoggerDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalUpdateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateResourceDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateResourceDefinitionRequestRequestTypeDef(
     _RequiredUpdateResourceDefinitionRequestRequestTypeDef,
     _OptionalUpdateResourceDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateRoleToGroupResponseTypeDef = TypedDict(
     "AssociateRoleToGroupResponseTypeDef",
     {
         "AssociatedAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2122,45 +2146,53 @@
     "_OptionalUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ConnectivityInfo": Sequence[ConnectivityInfoTypeDef],
     },
     total=False,
 )
 
+
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
-ConnectorDefinitionVersionOutputTypeDef = TypedDict(
-    "ConnectorDefinitionVersionOutputTypeDef",
-    {
-        "Connectors": List[ConnectorOutputTypeDef],
-    },
-    total=False,
-)
 
 ConnectorDefinitionVersionTypeDef = TypedDict(
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
-ConnectorUnionTypeDef = Union[ConnectorTypeDef, ConnectorOutputTypeDef]
-CoreDefinitionVersionOutputTypeDef = TypedDict(
-    "CoreDefinitionVersionOutputTypeDef",
+_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
     {
-        "Cores": List[CoreTypeDef],
+        "AmznClientToken": str,
+        "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
+
+class CreateConnectorDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
+
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
@@ -2176,20 +2208,22 @@
     {
         "AmznClientToken": str,
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
 
+
 class CreateCoreDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateCoreDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateCoreDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2197,27 +2231,21 @@
     {
         "AmznClientToken": str,
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeviceDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateDeviceDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateDeviceDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-DeviceDefinitionVersionOutputTypeDef = TypedDict(
-    "DeviceDefinitionVersionOutputTypeDef",
-    {
-        "Devices": List[DeviceTypeDef],
-    },
-    total=False,
-)
 
 DeviceDefinitionVersionTypeDef = TypedDict(
     "DeviceDefinitionVersionTypeDef",
     {
         "Devices": Sequence[DeviceTypeDef],
     },
     total=False,
@@ -2235,19 +2263,21 @@
         "AmznClientToken": str,
         "InitialVersion": GroupVersionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 GetGroupVersionResponseTypeDef = TypedDict(
     "GetGroupVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": GroupVersionTypeDef,
         "Id": str,
@@ -2267,27 +2297,21 @@
     {
         "AmznClientToken": str,
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
 )
 
+
 class CreateLoggerDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-LoggerDefinitionVersionOutputTypeDef = TypedDict(
-    "LoggerDefinitionVersionOutputTypeDef",
-    {
-        "Loggers": List[LoggerTypeDef],
-    },
-    total=False,
-)
 
 LoggerDefinitionVersionTypeDef = TypedDict(
     "LoggerDefinitionVersionTypeDef",
     {
         "Loggers": Sequence[LoggerTypeDef],
     },
     total=False,
@@ -2304,27 +2328,21 @@
     {
         "AmznClientToken": str,
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
 )
 
+
 class CreateSubscriptionDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateSubscriptionDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
-SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
-    "SubscriptionDefinitionVersionOutputTypeDef",
-    {
-        "Subscriptions": List[SubscriptionTypeDef],
-    },
-    total=False,
-)
 
 SubscriptionDefinitionVersionTypeDef = TypedDict(
     "SubscriptionDefinitionVersionTypeDef",
     {
         "Subscriptions": Sequence[SubscriptionTypeDef],
     },
     total=False,
@@ -2466,20 +2484,22 @@
     "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
 ):
     pass
 
+
 ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
     "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2494,20 +2514,22 @@
     "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
     _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2522,20 +2544,22 @@
     "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
     _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
     "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2550,40 +2574,44 @@
     "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
     _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
     _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
     "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2598,20 +2626,22 @@
     "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2626,20 +2656,22 @@
     "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
     _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "ListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2654,20 +2686,22 @@
     "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2682,20 +2716,22 @@
     "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
     _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
     "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2710,20 +2746,22 @@
     "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2838,110 +2876,72 @@
     "_OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationUpdateTypeDef,
     },
     total=False,
 )
 
+
 class UpdateThingRuntimeConfigurationRequestRequestTypeDef(
     _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef,
     _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": ConnectorDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConnectorDefinitionVersionUnionTypeDef = Union[
-    ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
-]
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Connectors": Sequence[ConnectorUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateConnectorDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-GetCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionVersionResponseTypeDef",
+GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": CoreDefinitionVersionOutputTypeDef,
+        "Definition": ConnectorDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoreDefinitionVersionUnionTypeDef = Union[
-    CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
-]
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+GetCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionOutputTypeDef,
+        "Definition": CoreDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2952,24 +2952,22 @@
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-DeviceDefinitionVersionUnionTypeDef = Union[
-    DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
-]
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Definition": DeviceDefinitionVersionTypeDef,
         "Id": str,
+        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
@@ -2978,25 +2976,21 @@
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-LoggerDefinitionVersionUnionTypeDef = Union[
-    LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
-]
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
+        "Definition": LoggerDefinitionVersionTypeDef,
         "Id": str,
-        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
@@ -3005,32 +2999,31 @@
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-SubscriptionDefinitionVersionUnionTypeDef = Union[
-    SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
-]
-FunctionDefaultConfigTypeDef = TypedDict(
-    "FunctionDefaultConfigTypeDef",
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
-        "Execution": FunctionDefaultExecutionConfigTypeDef,
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": SubscriptionDefinitionVersionTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
-    "FunctionConfigurationEnvironmentOutputTypeDef",
+FunctionDefaultConfigTypeDef = TypedDict(
+    "FunctionDefaultConfigTypeDef",
     {
-        "AccessSysfs": bool,
-        "Execution": FunctionExecutionConfigTypeDef,
-        "ResourceAccessPolicies": List[ResourceAccessPolicyTypeDef],
-        "Variables": Dict[str, str],
+        "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
 
 FunctionConfigurationEnvironmentTypeDef = TypedDict(
     "FunctionConfigurationEnvironmentTypeDef",
     {
@@ -3038,28 +3031,14 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
-ResourceDataContainerOutputTypeDef = TypedDict(
-    "ResourceDataContainerOutputTypeDef",
-    {
-        "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
-        "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
-        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
-        "SageMakerMachineLearningModelResourceData": (
-            SageMakerMachineLearningModelResourceDataTypeDef
-        ),
-        "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
-    },
-    total=False,
-)
-
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
@@ -3074,29 +3053,14 @@
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionConfigurationOutputTypeDef = TypedDict(
-    "FunctionConfigurationOutputTypeDef",
-    {
-        "EncodingType": EncodingTypeType,
-        "Environment": FunctionConfigurationEnvironmentOutputTypeDef,
-        "ExecArgs": str,
-        "Executable": str,
-        "MemorySize": int,
-        "Pinned": bool,
-        "Timeout": int,
-        "FunctionRuntimeOverride": str,
-    },
-    total=False,
-)
-
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
         "Environment": FunctionConfigurationEnvironmentTypeDef,
         "ExecArgs": str,
         "Executable": str,
@@ -3104,50 +3068,23 @@
         "Pinned": bool,
         "Timeout": int,
         "FunctionRuntimeOverride": str,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "ResourceDataContainer": ResourceDataContainerOutputTypeDef,
-    },
-)
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceDataContainer": ResourceDataContainerTypeDef,
     },
 )
 
-_RequiredFunctionOutputTypeDef = TypedDict(
-    "_RequiredFunctionOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalFunctionOutputTypeDef = TypedDict(
-    "_OptionalFunctionOutputTypeDef",
-    {
-        "FunctionArn": str,
-        "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
-    pass
-
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -3155,108 +3092,101 @@
     {
         "FunctionArn": str,
         "FunctionConfiguration": FunctionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
-ResourceDefinitionVersionOutputTypeDef = TypedDict(
-    "ResourceDefinitionVersionOutputTypeDef",
+
+_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
-        "Resources": List[ResourceOutputTypeDef],
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+
+class CreateResourceDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
-FunctionDefinitionVersionOutputTypeDef = TypedDict(
-    "FunctionDefinitionVersionOutputTypeDef",
+_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
+        "AmznClientToken": str,
         "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": List[FunctionOutputTypeDef],
+        "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
+
+class CreateFunctionDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
+
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
-FunctionUnionTypeDef = Union[FunctionTypeDef, FunctionOutputTypeDef]
-GetResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": ResourceDefinitionVersionOutputTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResourceDefinitionVersionUnionTypeDef = Union[
-    ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
-]
-_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateResourceDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionVersionResponseTypeDef",
+GetResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": FunctionDefinitionVersionOutputTypeDef,
+        "Definition": ResourceDefinitionVersionTypeDef,
         "Id": str,
-        "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
@@ -3265,31 +3195,19 @@
         "InitialVersion": FunctionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-FunctionDefinitionVersionUnionTypeDef = Union[
-    FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
-]
-_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
+GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionVersionResponseTypeDef",
     {
-        "AmznClientToken": str,
-        "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[FunctionUnionTypeDef],
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": FunctionDefinitionVersionTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-class CreateFunctionDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post1/types_aiobotocore_greengrass.egg-info/SOURCES.txt` & `types-aiobotocore-greengrass-2.5.2.post2/types_aiobotocore_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

