# Comparing `tmp/types-aiobotocore-appflow-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appflow-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appflow-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-appflow-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-appflow-2.5.2.post1.tar` & `types-aiobotocore-appflow-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86507 2023-08-02 14:33:11.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86375 2023-08-02 14:33:10.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:09.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:50.000000 types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.787006 types-aiobotocore-appflow-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-08-04 12:00:22.787006 types-aiobotocore-appflow-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.787006 types-aiobotocore-appflow-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.767005 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-08-04 11:40:17.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-08-04 11:40:17.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71159 2023-08-04 11:40:19.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71057 2023-08-04 11:40:18.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:16.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.787006 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:22.000000 types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appflow-2.5.2.post1/LICENSE` & `types-aiobotocore-appflow-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post1/setup.py` & `types-aiobotocore-appflow-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appflow",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/__main__.py` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.py` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigUnionTypeDef,
+    DestinationFlowConfigTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigUnionTypeDef,
+    SourceFlowConfigTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskUnionTypeDef,
-    TriggerConfigUnionTypeDef,
+    TaskTypeDef,
+    TriggerConfigTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -143,18 +143,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
         """
 
     async def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigUnionTypeDef,
-        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
-        tasks: Sequence[TaskUnionTypeDef],
+        triggerConfig: TriggerConfigTypeDef,
+        sourceFlowConfig: SourceFlowConfigTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
+        tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
@@ -428,18 +428,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
 
     async def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigUnionTypeDef,
-        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
-        tasks: Sequence[TaskUnionTypeDef],
+        triggerConfig: TriggerConfigTypeDef,
+        sourceFlowConfig: SourceFlowConfigTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
+        tasks: Sequence[TaskTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/client.pyi` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,26 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigUnionTypeDef,
+    DestinationFlowConfigTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigUnionTypeDef,
+    SourceFlowConfigTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskUnionTypeDef,
-    TriggerConfigUnionTypeDef,
+    TaskTypeDef,
+    TriggerConfigTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -134,18 +134,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
         """
     async def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigUnionTypeDef,
-        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
-        tasks: Sequence[TaskUnionTypeDef],
+        triggerConfig: TriggerConfigTypeDef,
+        sourceFlowConfig: SourceFlowConfigTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
+        tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
@@ -396,18 +396,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
     async def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: TriggerConfigUnionTypeDef,
-        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
-        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
-        tasks: Sequence[TaskUnionTypeDef],
+        triggerConfig: TriggerConfigTypeDef,
+        sourceFlowConfig: SourceFlowConfigTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
+        tasks: Sequence[TaskTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.py` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/literals.pyi` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.py` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,15 +113,14 @@
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
-    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
@@ -140,25 +139,22 @@
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
-    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
-    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesOutputTypeDef",
     "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
@@ -174,104 +170,81 @@
     "ListTagsForResourceResponseTypeDef",
     "RegisterConnectorResponseTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomConnectorSourcePropertiesOutputTypeDef",
     "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
-    "TaskOutputTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
-    "CustomConnectorDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
-    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
-    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
-    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
-    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
-    "S3OutputFormatConfigOutputTypeDef",
-    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
-    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
-    "TriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
-    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
-    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
-    "S3DestinationPropertiesOutputTypeDef",
-    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
-    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
-    "TriggerConfigOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
-    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
-    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
-    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
-    "SourceFlowConfigUnionTypeDef",
-    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "DescribeFlowResponseTypeDef",
-    "DestinationFlowConfigUnionTypeDef",
     "CreateFlowRequestRequestTypeDef",
+    "DescribeFlowResponseTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
@@ -786,36 +759,14 @@
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
-_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
-    "_RequiredOAuth2PropertiesOutputTypeDef",
-    {
-        "tokenUrl": str,
-        "oAuth2GrantType": OAuth2GrantTypeType,
-    },
-)
-_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
-    "_OptionalOAuth2PropertiesOutputTypeDef",
-    {
-        "tokenUrlCustomProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class OAuth2PropertiesOutputTypeDef(
-    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
-):
-    pass
-
-
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -1132,23 +1083,14 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
-OAuthPropertiesOutputTypeDef = TypedDict(
-    "OAuthPropertiesOutputTypeDef",
-    {
-        "tokenUrl": str,
-        "authCodeUrl": str,
-        "oAuthScopes": List[str],
-    },
-)
-
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
@@ -1157,24 +1099,14 @@
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-PrefixConfigOutputTypeDef = TypedDict(
-    "PrefixConfigOutputTypeDef",
-    {
-        "prefixType": PrefixTypeType,
-        "prefixFormat": PrefixFormatType,
-        "pathPrefixHierarchy": List[PathPrefixType],
-    },
-    total=False,
-)
-
 PrefixConfigTypeDef = TypedDict(
     "PrefixConfigTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
@@ -1237,42 +1169,14 @@
 
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
 
-_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
-    {
-        "scheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
-    {
-        "dataPullMode": DataPullModeType,
-        "scheduleStartTime": datetime,
-        "scheduleEndTime": datetime,
-        "timezone": str,
-        "scheduleOffset": int,
-        "firstExecutionFrom": datetime,
-        "flowErrorDeactivationThreshold": int,
-    },
-    total=False,
-)
-
-
-class ScheduledTriggerPropertiesOutputTypeDef(
-    _RequiredScheduledTriggerPropertiesOutputTypeDef,
-    _OptionalScheduledTriggerPropertiesOutputTypeDef,
-):
-    pass
-
-
 TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
@@ -1484,37 +1388,14 @@
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
-    {
-        "customProperties": Dict[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
-    },
-    total=False,
-)
-
-
-class CustomConnectorSourcePropertiesOutputTypeDef(
-    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
-    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
@@ -1741,36 +1622,14 @@
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
 
-_RequiredTaskOutputTypeDef = TypedDict(
-    "_RequiredTaskOutputTypeDef",
-    {
-        "sourceFields": List[str],
-        "taskType": TaskTypeType,
-    },
-)
-_OptionalTaskOutputTypeDef = TypedDict(
-    "_OptionalTaskOutputTypeDef",
-    {
-        "connectorOperator": ConnectorOperatorTypeDef,
-        "destinationField": str,
-        "taskProperties": Dict[OperatorPropertiesKeysType, str],
-    },
-    total=False,
-)
-
-
-class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
-    pass
-
-
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1793,39 +1652,14 @@
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "idFieldNames": List[str],
-        "customProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class CustomConnectorDestinationPropertiesOutputTypeDef(
-    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
-    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1930,39 +1764,14 @@
 
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
 
-_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-
-class SalesforceDestinationPropertiesOutputTypeDef(
-    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
-    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -2002,38 +1811,14 @@
 
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
 
-_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-
-class ZendeskDestinationPropertiesOutputTypeDef(
-    _RequiredZendeskDestinationPropertiesOutputTypeDef,
-    _OptionalZendeskDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -2049,23 +1834,14 @@
 
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
 
-CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "CustomConnectorProfilePropertiesOutputTypeDef",
-    {
-        "profileProperties": Dict[str, str],
-        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
@@ -2155,41 +1931,14 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
-    {
-        "applicationHostUrl": str,
-        "applicationServicePath": str,
-        "portNumber": int,
-        "clientNumber": str,
-    },
-)
-_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
-    {
-        "logonLanguage": str,
-        "privateLinkServiceName": str,
-        "oAuthProperties": OAuthPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SAPODataConnectorProfilePropertiesOutputTypeDef(
-    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
-    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -2209,48 +1958,14 @@
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
 
-S3OutputFormatConfigOutputTypeDef = TypedDict(
-    "S3OutputFormatConfigOutputTypeDef",
-    {
-        "fileType": FileTypeType,
-        "prefixConfig": PrefixConfigOutputTypeDef,
-        "aggregationConfig": AggregationConfigTypeDef,
-        "preserveSourceDataTyping": bool,
-    },
-    total=False,
-)
-
-_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
-    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
-    {
-        "prefixConfig": PrefixConfigOutputTypeDef,
-    },
-)
-_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
-    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
-    {
-        "fileType": FileTypeType,
-        "aggregationConfig": AggregationConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class UpsolverS3OutputFormatConfigOutputTypeDef(
-    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
-    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
-):
-    pass
-
-
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -2298,39 +2013,14 @@
 
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
 
-_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
-    {
-        "objectPath": str,
-    },
-)
-_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
-    {
-        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-
-class SAPODataDestinationPropertiesOutputTypeDef(
-    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
-    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -2347,22 +2037,14 @@
 
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
 
-TriggerPropertiesOutputTypeDef = TypedDict(
-    "TriggerPropertiesOutputTypeDef",
-    {
-        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
 _OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
@@ -2416,15 +2098,14 @@
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
-TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2497,40 +2178,14 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
-ConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ConnectorProfilePropertiesOutputTypeDef",
-    {
-        "Amplitude": Dict[str, Any],
-        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
-        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
-        "GoogleAnalytics": Dict[str, Any],
-        "Honeycode": Dict[str, Any],
-        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
-        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
-        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
-        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
-        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
-        "Singular": Dict[str, Any],
-        "Slack": SlackConnectorProfilePropertiesTypeDef,
-        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
-        "Trendmicro": Dict[str, Any],
-        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
-        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
-        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
-        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
-        "Pardot": PardotConnectorProfilePropertiesTypeDef,
-    },
-    total=False,
-)
-
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2549,59 +2204,14 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationPropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DestinationPropertiesOutputTypeDef(
-    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
-):
-    pass
-
-
-_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
-    },
-)
-_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-    },
-    total=False,
-)
-
-
-class UpsolverDestinationPropertiesOutputTypeDef(
-    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
-    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2638,38 +2248,14 @@
 
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
 
-SourceConnectorPropertiesOutputTypeDef = TypedDict(
-    "SourceConnectorPropertiesOutputTypeDef",
-    {
-        "Amplitude": AmplitudeSourcePropertiesTypeDef,
-        "Datadog": DatadogSourcePropertiesTypeDef,
-        "Dynatrace": DynatraceSourcePropertiesTypeDef,
-        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
-        "InforNexus": InforNexusSourcePropertiesTypeDef,
-        "Marketo": MarketoSourcePropertiesTypeDef,
-        "S3": S3SourcePropertiesTypeDef,
-        "Salesforce": SalesforceSourcePropertiesTypeDef,
-        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
-        "Singular": SingularSourcePropertiesTypeDef,
-        "Slack": SlackSourcePropertiesTypeDef,
-        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
-        "Veeva": VeevaSourcePropertiesTypeDef,
-        "Zendesk": ZendeskSourcePropertiesTypeDef,
-        "SAPOData": SAPODataSourcePropertiesTypeDef,
-        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
-        "Pardot": PardotSourcePropertiesTypeDef,
-    },
-    total=False,
-)
-
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2686,35 +2272,14 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredTriggerConfigOutputTypeDef = TypedDict(
-    "_RequiredTriggerConfigOutputTypeDef",
-    {
-        "triggerType": TriggerTypeType,
-    },
-)
-_OptionalTriggerConfigOutputTypeDef = TypedDict(
-    "_OptionalTriggerConfigOutputTypeDef",
-    {
-        "triggerProperties": TriggerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TriggerConfigOutputTypeDef(
-    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
-):
-    pass
-
-
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2824,42 +2389,22 @@
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
-DestinationConnectorPropertiesOutputTypeDef = TypedDict(
-    "DestinationConnectorPropertiesOutputTypeDef",
-    {
-        "Redshift": RedshiftDestinationPropertiesTypeDef,
-        "S3": S3DestinationPropertiesOutputTypeDef,
-        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
-        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
-        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
-        "LookoutMetrics": Dict[str, Any],
-        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
-        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
-        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
-        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
-        "Marketo": MarketoDestinationPropertiesTypeDef,
-        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
-        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2872,38 +2417,14 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
-    "_RequiredSourceFlowConfigOutputTypeDef",
-    {
-        "connectorType": ConnectorTypeType,
-        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
-    },
-)
-_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
-    "_OptionalSourceFlowConfigOutputTypeDef",
-    {
-        "apiVersion": str,
-        "connectorProfileName": str,
-        "incrementalPullConfig": IncrementalPullConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SourceFlowConfigOutputTypeDef(
-    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2993,37 +2514,14 @@
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
-    "_RequiredDestinationFlowConfigOutputTypeDef",
-    {
-        "connectorType": ConnectorTypeType,
-        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
-    },
-)
-_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
-    "_OptionalDestinationFlowConfigOutputTypeDef",
-    {
-        "apiVersion": str,
-        "connectorProfileName": str,
-    },
-    total=False,
-)
-
-
-class DestinationFlowConfigOutputTypeDef(
-    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -3039,16 +2537,14 @@
 
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
 
-SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
-TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -3092,51 +2588,22 @@
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigOutputTypeDef,
-        "tasks": List[TaskOutputTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DestinationFlowConfigUnionTypeDef = Union[
-    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
-]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
-        "tasks": Sequence[TaskUnionTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
+        "tasks": Sequence[TaskTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3150,22 +2617,48 @@
 
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
 
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigTypeDef,
+        "tasks": List[TaskTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
-        "tasks": Sequence[TaskUnionTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
+        "tasks": Sequence[TaskTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow/type_defs.pyi` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
-    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
@@ -139,25 +138,22 @@
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
-    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
-    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesOutputTypeDef",
     "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
@@ -173,104 +169,81 @@
     "ListTagsForResourceResponseTypeDef",
     "RegisterConnectorResponseTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowResponseTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
-    "CustomConnectorSourcePropertiesOutputTypeDef",
     "CustomConnectorSourcePropertiesTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
-    "TaskOutputTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
-    "CustomConnectorDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
-    "SalesforceDestinationPropertiesOutputTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
-    "ZendeskDestinationPropertiesOutputTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
-    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
-    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
-    "S3OutputFormatConfigOutputTypeDef",
-    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
-    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
-    "TriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
-    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
-    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
-    "S3DestinationPropertiesOutputTypeDef",
-    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
-    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
-    "TriggerConfigOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
-    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
-    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
-    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
-    "SourceFlowConfigUnionTypeDef",
-    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "DescribeFlowResponseTypeDef",
-    "DestinationFlowConfigUnionTypeDef",
     "CreateFlowRequestRequestTypeDef",
+    "DescribeFlowResponseTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
@@ -773,34 +746,14 @@
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
-_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
-    "_RequiredOAuth2PropertiesOutputTypeDef",
-    {
-        "tokenUrl": str,
-        "oAuth2GrantType": OAuth2GrantTypeType,
-    },
-)
-_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
-    "_OptionalOAuth2PropertiesOutputTypeDef",
-    {
-        "tokenUrlCustomProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-class OAuth2PropertiesOutputTypeDef(
-    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
-):
-    pass
-
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -1103,23 +1056,14 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
-OAuthPropertiesOutputTypeDef = TypedDict(
-    "OAuthPropertiesOutputTypeDef",
-    {
-        "tokenUrl": str,
-        "authCodeUrl": str,
-        "oAuthScopes": List[str],
-    },
-)
-
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
@@ -1128,24 +1072,14 @@
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-PrefixConfigOutputTypeDef = TypedDict(
-    "PrefixConfigOutputTypeDef",
-    {
-        "prefixType": PrefixTypeType,
-        "prefixFormat": PrefixFormatType,
-        "pathPrefixHierarchy": List[PathPrefixType],
-    },
-    total=False,
-)
-
 PrefixConfigTypeDef = TypedDict(
     "PrefixConfigTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
@@ -1206,40 +1140,14 @@
 )
 
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
-_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
-    {
-        "scheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
-    {
-        "dataPullMode": DataPullModeType,
-        "scheduleStartTime": datetime,
-        "scheduleEndTime": datetime,
-        "timezone": str,
-        "scheduleOffset": int,
-        "firstExecutionFrom": datetime,
-        "flowErrorDeactivationThreshold": int,
-    },
-    total=False,
-)
-
-class ScheduledTriggerPropertiesOutputTypeDef(
-    _RequiredScheduledTriggerPropertiesOutputTypeDef,
-    _OptionalScheduledTriggerPropertiesOutputTypeDef,
-):
-    pass
-
 TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
@@ -1445,35 +1353,14 @@
     "UpdateFlowResponseTypeDef",
     {
         "flowStatus": FlowStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
-    {
-        "customProperties": Dict[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
-    },
-    total=False,
-)
-
-class CustomConnectorSourcePropertiesOutputTypeDef(
-    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
-    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorSourcePropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
@@ -1688,34 +1575,14 @@
 
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-_RequiredTaskOutputTypeDef = TypedDict(
-    "_RequiredTaskOutputTypeDef",
-    {
-        "sourceFields": List[str],
-        "taskType": TaskTypeType,
-    },
-)
-_OptionalTaskOutputTypeDef = TypedDict(
-    "_OptionalTaskOutputTypeDef",
-    {
-        "connectorOperator": ConnectorOperatorTypeDef,
-        "destinationField": str,
-        "taskProperties": Dict[OperatorPropertiesKeysType, str],
-    },
-    total=False,
-)
-
-class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
-    pass
-
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1736,37 +1603,14 @@
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
-    {
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "idFieldNames": List[str],
-        "customProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-class CustomConnectorDestinationPropertiesOutputTypeDef(
-    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
-    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1861,37 +1705,14 @@
 )
 
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
-_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-        "dataTransferApi": SalesforceDataTransferApiType,
-    },
-    total=False,
-)
-
-class SalesforceDestinationPropertiesOutputTypeDef(
-    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
-    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1927,36 +1748,14 @@
 )
 
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
-_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "object": str,
-    },
-)
-_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
-    {
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-class ZendeskDestinationPropertiesOutputTypeDef(
-    _RequiredZendeskDestinationPropertiesOutputTypeDef,
-    _OptionalZendeskDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1970,23 +1769,14 @@
 )
 
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
-CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "CustomConnectorProfilePropertiesOutputTypeDef",
-    {
-        "profileProperties": Dict[str, str],
-        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
@@ -2074,39 +1864,14 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
-    {
-        "applicationHostUrl": str,
-        "applicationServicePath": str,
-        "portNumber": int,
-        "clientNumber": str,
-    },
-)
-_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
-    {
-        "logonLanguage": str,
-        "privateLinkServiceName": str,
-        "oAuthProperties": OAuthPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-class SAPODataConnectorProfilePropertiesOutputTypeDef(
-    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
-    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -2124,46 +1889,14 @@
 
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-S3OutputFormatConfigOutputTypeDef = TypedDict(
-    "S3OutputFormatConfigOutputTypeDef",
-    {
-        "fileType": FileTypeType,
-        "prefixConfig": PrefixConfigOutputTypeDef,
-        "aggregationConfig": AggregationConfigTypeDef,
-        "preserveSourceDataTyping": bool,
-    },
-    total=False,
-)
-
-_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
-    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
-    {
-        "prefixConfig": PrefixConfigOutputTypeDef,
-    },
-)
-_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
-    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
-    {
-        "fileType": FileTypeType,
-        "aggregationConfig": AggregationConfigTypeDef,
-    },
-    total=False,
-)
-
-class UpsolverS3OutputFormatConfigOutputTypeDef(
-    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
-    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
-):
-    pass
-
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -2207,37 +1940,14 @@
 )
 
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
-_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
-    {
-        "objectPath": str,
-    },
-)
-_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
-    {
-        "successResponseHandlingConfig": SuccessResponseHandlingConfigTypeDef,
-        "idFieldNames": List[str],
-        "errorHandlingConfig": ErrorHandlingConfigTypeDef,
-        "writeOperationType": WriteOperationTypeType,
-    },
-    total=False,
-)
-
-class SAPODataDestinationPropertiesOutputTypeDef(
-    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
-    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -2252,22 +1962,14 @@
 )
 
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
-TriggerPropertiesOutputTypeDef = TypedDict(
-    "TriggerPropertiesOutputTypeDef",
-    {
-        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
 _OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
@@ -2317,15 +2019,14 @@
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
-TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2396,40 +2097,14 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
-ConnectorProfilePropertiesOutputTypeDef = TypedDict(
-    "ConnectorProfilePropertiesOutputTypeDef",
-    {
-        "Amplitude": Dict[str, Any],
-        "Datadog": DatadogConnectorProfilePropertiesTypeDef,
-        "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
-        "GoogleAnalytics": Dict[str, Any],
-        "Honeycode": Dict[str, Any],
-        "InforNexus": InforNexusConnectorProfilePropertiesTypeDef,
-        "Marketo": MarketoConnectorProfilePropertiesTypeDef,
-        "Redshift": RedshiftConnectorProfilePropertiesTypeDef,
-        "Salesforce": SalesforceConnectorProfilePropertiesTypeDef,
-        "ServiceNow": ServiceNowConnectorProfilePropertiesTypeDef,
-        "Singular": Dict[str, Any],
-        "Slack": SlackConnectorProfilePropertiesTypeDef,
-        "Snowflake": SnowflakeConnectorProfilePropertiesTypeDef,
-        "Trendmicro": Dict[str, Any],
-        "Veeva": VeevaConnectorProfilePropertiesTypeDef,
-        "Zendesk": ZendeskConnectorProfilePropertiesTypeDef,
-        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
-        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
-        "Pardot": PardotConnectorProfilePropertiesTypeDef,
-    },
-    total=False,
-)
-
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2448,55 +2123,14 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationPropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class S3DestinationPropertiesOutputTypeDef(
-    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
-):
-    pass
-
-_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
-    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
-    {
-        "bucketName": str,
-        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
-    },
-)
-_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
-    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
-    {
-        "bucketPrefix": str,
-    },
-    total=False,
-)
-
-class UpsolverDestinationPropertiesOutputTypeDef(
-    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
-    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2529,38 +2163,14 @@
 )
 
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
-SourceConnectorPropertiesOutputTypeDef = TypedDict(
-    "SourceConnectorPropertiesOutputTypeDef",
-    {
-        "Amplitude": AmplitudeSourcePropertiesTypeDef,
-        "Datadog": DatadogSourcePropertiesTypeDef,
-        "Dynatrace": DynatraceSourcePropertiesTypeDef,
-        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
-        "InforNexus": InforNexusSourcePropertiesTypeDef,
-        "Marketo": MarketoSourcePropertiesTypeDef,
-        "S3": S3SourcePropertiesTypeDef,
-        "Salesforce": SalesforceSourcePropertiesTypeDef,
-        "ServiceNow": ServiceNowSourcePropertiesTypeDef,
-        "Singular": SingularSourcePropertiesTypeDef,
-        "Slack": SlackSourcePropertiesTypeDef,
-        "Trendmicro": TrendmicroSourcePropertiesTypeDef,
-        "Veeva": VeevaSourcePropertiesTypeDef,
-        "Zendesk": ZendeskSourcePropertiesTypeDef,
-        "SAPOData": SAPODataSourcePropertiesTypeDef,
-        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
-        "Pardot": PardotSourcePropertiesTypeDef,
-    },
-    total=False,
-)
-
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2577,33 +2187,14 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredTriggerConfigOutputTypeDef = TypedDict(
-    "_RequiredTriggerConfigOutputTypeDef",
-    {
-        "triggerType": TriggerTypeType,
-    },
-)
-_OptionalTriggerConfigOutputTypeDef = TypedDict(
-    "_OptionalTriggerConfigOutputTypeDef",
-    {
-        "triggerProperties": TriggerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-class TriggerConfigOutputTypeDef(
-    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
-):
-    pass
-
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2711,42 +2302,22 @@
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
-DestinationConnectorPropertiesOutputTypeDef = TypedDict(
-    "DestinationConnectorPropertiesOutputTypeDef",
-    {
-        "Redshift": RedshiftDestinationPropertiesTypeDef,
-        "S3": S3DestinationPropertiesOutputTypeDef,
-        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
-        "Snowflake": SnowflakeDestinationPropertiesTypeDef,
-        "EventBridge": EventBridgeDestinationPropertiesTypeDef,
-        "LookoutMetrics": Dict[str, Any],
-        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
-        "Honeycode": HoneycodeDestinationPropertiesTypeDef,
-        "CustomerProfiles": CustomerProfilesDestinationPropertiesTypeDef,
-        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
-        "Marketo": MarketoDestinationPropertiesTypeDef,
-        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
-        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2759,36 +2330,14 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
-_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
-    "_RequiredSourceFlowConfigOutputTypeDef",
-    {
-        "connectorType": ConnectorTypeType,
-        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
-    },
-)
-_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
-    "_OptionalSourceFlowConfigOutputTypeDef",
-    {
-        "apiVersion": str,
-        "connectorProfileName": str,
-        "incrementalPullConfig": IncrementalPullConfigTypeDef,
-    },
-    total=False,
-)
-
-class SourceFlowConfigOutputTypeDef(
-    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
-):
-    pass
-
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2872,35 +2421,14 @@
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
-    "_RequiredDestinationFlowConfigOutputTypeDef",
-    {
-        "connectorType": ConnectorTypeType,
-        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
-    },
-)
-_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
-    "_OptionalDestinationFlowConfigOutputTypeDef",
-    {
-        "apiVersion": str,
-        "connectorProfileName": str,
-    },
-    total=False,
-)
-
-class DestinationFlowConfigOutputTypeDef(
-    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
-):
-    pass
-
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -2914,16 +2442,14 @@
 )
 
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
-SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
-TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2963,51 +2489,22 @@
 
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigOutputTypeDef,
-        "tasks": List[TaskOutputTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DestinationFlowConfigUnionTypeDef = Union[
-    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
-]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
-        "tasks": Sequence[TaskUnionTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
+        "tasks": Sequence[TaskTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3019,22 +2516,48 @@
 )
 
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigTypeDef,
+        "tasks": List[TaskTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
-        "tasks": Sequence[TaskUnionTypeDef],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
+        "tasks": Sequence[TaskTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `types-aiobotocore-appflow-2.5.2.post1/types_aiobotocore_appflow.egg-info/SOURCES.txt` & `types-aiobotocore-appflow-2.5.2.post2/types_aiobotocore_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

