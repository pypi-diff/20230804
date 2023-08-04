# Comparing `tmp/types-aiobotocore-lambda-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lambda-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lambda-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lambda-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lambda-2.5.2.post1.tar` & `types-aiobotocore-lambda-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.517543 types-aiobotocore-lambda-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-08-02 14:52:33.517543 types-aiobotocore-lambda-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.517543 types-aiobotocore-lambda-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.517543 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62548 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    62456 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80718 2023-08-02 14:41:50.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80611 2023-08-02 14:41:47.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:45.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-08-02 14:41:46.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.517543 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25122 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:33.000000 types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.176643 types-aiobotocore-lambda-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15913 2023-08-04 13:59:15.176643 types-aiobotocore-lambda-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14399 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.176643 types-aiobotocore-lambda-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:42:24.000000 types-aiobotocore-lambda-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.176643 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4232 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4231 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    62463 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    62371 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14413 2023-08-04 13:42:26.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14411 2023-08-04 13:42:26.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14310 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14296 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    78488 2023-08-04 13:42:28.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    78381 2023-08-04 13:42:27.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6547 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6541 2023-08-04 13:42:25.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.176643 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15913 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:15.000000 types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lambda-2.5.2.post1/LICENSE` & `types-aiobotocore-lambda-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/setup.py` & `types-aiobotocore-lambda-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lambda",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Lambda 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__init__.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__init__.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/__main__.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Lambda 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Lambda 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/client.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,47 +45,47 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
-    AliasRoutingConfigurationUnionTypeDef,
-    AllowedPublishersUnionTypeDef,
+    AliasRoutingConfigurationTypeDef,
+    AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
-    CorsUnionTypeDef,
+    CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
-    ImageConfigUnionTypeDef,
+    ImageConfigTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
@@ -99,15 +99,15 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
-    SelfManagedEventSourceUnionTypeDef,
+    SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
     TimestampTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
@@ -259,28 +259,28 @@
     async def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_alias)
         """
 
     async def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: AllowedPublishersUnionTypeDef,
+        AllowedPublishers: AllowedPublishersTypeDef,
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -290,28 +290,28 @@
     async def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
+        FilterCriteria: FilterCriteriaTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
         StartingPositionTimestamp: TimestampTypeDef = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: SelfManagedEventSourceUnionTypeDef = ...,
+        SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -338,15 +338,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigUnionTypeDef = ...,
+        ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -357,15 +357,15 @@
 
     async def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: CorsUnionTypeDef = ...,
+        Cors: CorsTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function_url_config)
@@ -999,15 +999,15 @@
     async def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...,
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -1016,15 +1016,15 @@
         """
 
     async def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: AllowedPublishersUnionTypeDef = ...,
+        AllowedPublishers: AllowedPublishersTypeDef = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_code_signing_config)
@@ -1033,15 +1033,15 @@
     async def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
+        FilterCriteria: FilterCriteriaTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -1092,15 +1092,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigUnionTypeDef = ...,
+        ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1126,15 +1126,15 @@
 
     async def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: CorsUnionTypeDef = ...,
+        Cors: CorsTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_url_config)
```

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/client.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,47 +45,47 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
-    AliasRoutingConfigurationUnionTypeDef,
-    AllowedPublishersUnionTypeDef,
+    AliasRoutingConfigurationTypeDef,
+    AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     BlobTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
-    CorsUnionTypeDef,
+    CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
-    ImageConfigUnionTypeDef,
+    ImageConfigTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
@@ -99,15 +99,15 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
-    SelfManagedEventSourceUnionTypeDef,
+    SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
     TimestampTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
@@ -250,27 +250,27 @@
     async def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_alias)
         """
     async def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: AllowedPublishersUnionTypeDef,
+        AllowedPublishers: AllowedPublishersTypeDef,
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -279,28 +279,28 @@
     async def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
+        FilterCriteria: FilterCriteriaTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
         StartingPositionTimestamp: TimestampTypeDef = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: SelfManagedEventSourceUnionTypeDef = ...,
+        SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -326,15 +326,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigUnionTypeDef = ...,
+        ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -344,15 +344,15 @@
         """
     async def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: CorsUnionTypeDef = ...,
+        Cors: CorsTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function_url_config)
@@ -932,15 +932,15 @@
     async def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationUnionTypeDef = ...,
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -948,15 +948,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_alias)
         """
     async def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: AllowedPublishersUnionTypeDef = ...,
+        AllowedPublishers: AllowedPublishersTypeDef = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_code_signing_config)
@@ -964,15 +964,15 @@
     async def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaUnionTypeDef = ...,
+        FilterCriteria: FilterCriteriaTypeDef = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -1021,15 +1021,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigUnionTypeDef = ...,
+        ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1053,15 +1053,15 @@
         """
     async def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: CorsUnionTypeDef = ...,
+        Cors: CorsTypeDef = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_url_config)
```

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/literals.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     "nodejs4.3-edge",
     "nodejs6.10",
     "nodejs8.10",
     "provided",
     "provided.al2",
     "python2.7",
     "python3.10",
+    "python3.11",
     "python3.6",
     "python3.7",
     "python3.8",
     "python3.9",
     "ruby2.5",
     "ruby2.7",
     "ruby3.2",
@@ -211,14 +212,15 @@
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
@@ -314,14 +316,15 @@
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
@@ -400,26 +403,28 @@
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
@@ -601,14 +606,15 @@
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

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/literals.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
     "nodejs4.3-edge",
     "nodejs6.10",
     "nodejs8.10",
     "provided",
     "provided.al2",
     "python2.7",
     "python3.10",
+    "python3.11",
     "python3.6",
     "python3.7",
     "python3.8",
     "python3.9",
     "ruby2.5",
     "ruby2.7",
     "ruby3.2",
@@ -209,14 +210,15 @@
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
@@ -312,14 +314,15 @@
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
@@ -398,26 +401,28 @@
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
@@ -599,14 +604,15 @@
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

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/paginator.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/paginator.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/type_defs.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,20 @@
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
-    "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
-    "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "BlobTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
-    "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
     "TimestampTypeDef",
@@ -91,15 +88,14 @@
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteFunctionUrlConfigRequestRequestTypeDef",
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
     "EnvironmentErrorTypeDef",
-    "SelfManagedEventSourceOutputTypeDef",
     "FilterTypeDef",
     "FunctionCodeLocationTypeDef",
     "LayerTypeDef",
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
@@ -116,15 +112,14 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
     "ImageConfigErrorTypeDef",
-    "ImageConfigOutputTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "LayerVersionsListItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
@@ -164,50 +159,44 @@
     "ListFunctionsByCodeSigningConfigResponseTypeDef",
     "ListTagsResponseTypeDef",
     "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
-    "AliasRoutingConfigurationUnionTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
-    "AllowedPublishersUnionTypeDef",
     "FunctionCodeTypeDef",
     "InvocationRequestRequestTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
+    "CreateFunctionUrlConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
-    "UpdateFunctionUrlConfigResponseTypeDef",
-    "CorsUnionTypeDef",
-    "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
+    "UpdateFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
-    "SelfManagedEventSourceUnionTypeDef",
-    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
     "GetFunctionRequestFunctionActiveV2WaitTypeDef",
     "GetFunctionRequestFunctionExistsWaitTypeDef",
     "GetFunctionRequestFunctionUpdatedV2WaitTypeDef",
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
-    "ImageConfigUnionTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
@@ -228,18 +217,17 @@
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
     "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
+    "CreateEventSourceMappingRequestRequestTypeDef",
     "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
-    "CreateEventSourceMappingRequestRequestTypeDef",
-    "FilterCriteriaUnionTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
     "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
@@ -333,37 +321,22 @@
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
 
-AliasRoutingConfigurationOutputTypeDef = TypedDict(
-    "AliasRoutingConfigurationOutputTypeDef",
-    {
-        "AdditionalVersionWeights": Dict[str, float],
-    },
-    total=False,
-)
-
 AliasRoutingConfigurationTypeDef = TypedDict(
     "AliasRoutingConfigurationTypeDef",
     {
         "AdditionalVersionWeights": Mapping[str, float],
     },
     total=False,
 )
 
-AllowedPublishersOutputTypeDef = TypedDict(
-    "AllowedPublishersOutputTypeDef",
-    {
-        "SigningProfileVersionArns": List[str],
-    },
-)
-
 AllowedPublishersTypeDef = TypedDict(
     "AllowedPublishersTypeDef",
     {
         "SigningProfileVersionArns": Sequence[str],
     },
 )
 
@@ -388,27 +361,14 @@
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
     total=False,
 )
 
-CorsOutputTypeDef = TypedDict(
-    "CorsOutputTypeDef",
-    {
-        "AllowCredentials": bool,
-        "AllowHeaders": List[str],
-        "AllowMethods": List[str],
-        "AllowOrigins": List[str],
-        "ExposeHeaders": List[str],
-        "MaxAge": int,
-    },
-    total=False,
-)
-
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
@@ -666,22 +626,14 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-SelfManagedEventSourceOutputTypeDef = TypedDict(
-    "SelfManagedEventSourceOutputTypeDef",
-    {
-        "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -958,24 +910,14 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-ImageConfigOutputTypeDef = TypedDict(
-    "ImageConfigOutputTypeDef",
-    {
-        "EntryPoint": List[str],
-        "Command": List[str],
-        "WorkingDirectory": str,
-    },
-    total=False,
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -1554,36 +1496,33 @@
 AliasConfigurationResponseTypeDef = TypedDict(
     "AliasConfigurationResponseTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
-        "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
+        "RoutingConfig": AliasRoutingConfigurationTypeDef,
         "RevisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
-        "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
+        "RoutingConfig": AliasRoutingConfigurationTypeDef,
         "RevisionId": str,
     },
     total=False,
 )
 
-AliasRoutingConfigurationUnionTypeDef = Union[
-    AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-]
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
         "FunctionVersion": str,
     },
@@ -1625,15 +1564,14 @@
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
 
-AllowedPublishersUnionTypeDef = Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef]
 FunctionCodeTypeDef = TypedDict(
     "FunctionCodeTypeDef",
     {
         "ZipFile": BlobTypeDef,
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
@@ -1743,15 +1681,15 @@
 
 
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
-        "AllowedPublishers": AllowedPublishersOutputTypeDef,
+        "AllowedPublishers": AllowedPublishersTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
         "LastModified": str,
     },
 )
 _OptionalCodeSigningConfigTypeDef = TypedDict(
     "_OptionalCodeSigningConfigTypeDef",
     {
@@ -1810,21 +1748,46 @@
 class UpdateCodeSigningConfigRequestRequestTypeDef(
     _RequiredUpdateCodeSigningConfigRequestRequestTypeDef,
     _OptionalUpdateCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "AuthType": FunctionUrlAuthTypeType,
+    },
+)
+_OptionalCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionUrlConfigRequestRequestTypeDef",
+    {
+        "Qualifier": str,
+        "Cors": CorsTypeDef,
+        "InvokeMode": InvokeModeType,
+    },
+    total=False,
+)
+
+
+class CreateFunctionUrlConfigRequestRequestTypeDef(
+    _RequiredCreateFunctionUrlConfigRequestRequestTypeDef,
+    _OptionalCreateFunctionUrlConfigRequestRequestTypeDef,
+):
+    pass
+
+
 CreateFunctionUrlConfigResponseTypeDef = TypedDict(
     "CreateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionUrlConfigTypeDef = TypedDict(
@@ -1836,15 +1799,15 @@
         "LastModifiedTime": str,
         "AuthType": FunctionUrlAuthTypeType,
     },
 )
 _OptionalFunctionUrlConfigTypeDef = TypedDict(
     "_OptionalFunctionUrlConfigTypeDef",
     {
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "InvokeMode": InvokeModeType,
     },
     total=False,
 )
 
 
 class FunctionUrlConfigTypeDef(
@@ -1855,62 +1818,22 @@
 
 GetFunctionUrlConfigResponseTypeDef = TypedDict(
     "GetFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
-        "CreationTime": str,
-        "LastModifiedTime": str,
-        "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
-    "UpdateFunctionUrlConfigResponseTypeDef",
-    {
-        "FunctionUrl": str,
-        "FunctionArn": str,
-        "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
-_RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "AuthType": FunctionUrlAuthTypeType,
-    },
-)
-_OptionalCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionUrlConfigRequestRequestTypeDef",
-    {
-        "Qualifier": str,
-        "Cors": CorsTypeDef,
-        "InvokeMode": InvokeModeType,
-    },
-    total=False,
-)
-
-
-class CreateFunctionUrlConfigRequestRequestTypeDef(
-    _RequiredCreateFunctionUrlConfigRequestRequestTypeDef,
-    _OptionalCreateFunctionUrlConfigRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
@@ -1928,14 +1851,28 @@
 class UpdateFunctionUrlConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
+    "UpdateFunctionUrlConfigResponseTypeDef",
+    {
+        "FunctionUrl": str,
+        "FunctionArn": str,
+        "AuthType": FunctionUrlAuthTypeType,
+        "Cors": CorsTypeDef,
+        "CreationTime": str,
+        "LastModifiedTime": str,
+        "InvokeMode": InvokeModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionConfigurationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
@@ -1984,25 +1921,14 @@
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
     total=False,
 )
 
-SelfManagedEventSourceUnionTypeDef = Union[
-    SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
-]
-FilterCriteriaOutputTypeDef = TypedDict(
-    "FilterCriteriaOutputTypeDef",
-    {
-        "Filters": List[FilterTypeDef],
-    },
-    total=False,
-)
-
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
@@ -2176,21 +2102,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
-        "ImageConfig": ImageConfigOutputTypeDef,
+        "ImageConfig": ImageConfigTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
     total=False,
 )
 
-ImageConfigUnionTypeDef = Union[ImageConfigTypeDef, ImageConfigOutputTypeDef]
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
     total=False,
@@ -2617,35 +2542,78 @@
 class UpdateFunctionEventInvokeConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventSourceMappingRequestRequestTypeDef",
+    {
+        "EventSourceArn": str,
+        "Enabled": bool,
+        "BatchSize": int,
+        "FilterCriteria": FilterCriteriaTypeDef,
+        "MaximumBatchingWindowInSeconds": int,
+        "ParallelizationFactor": int,
+        "StartingPosition": EventSourcePositionType,
+        "StartingPositionTimestamp": TimestampTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
+        "MaximumRecordAgeInSeconds": int,
+        "BisectBatchOnFunctionError": bool,
+        "MaximumRetryAttempts": int,
+        "TumblingWindowInSeconds": int,
+        "Topics": Sequence[str],
+        "Queues": Sequence[str],
+        "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
+        "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateEventSourceMappingRequestRequestTypeDef(
+    _RequiredCreateEventSourceMappingRequestRequestTypeDef,
+    _OptionalCreateEventSourceMappingRequestRequestTypeDef,
+):
+    pass
+
+
 EventSourceMappingConfigurationResponseTypeDef = TypedDict(
     "EventSourceMappingConfigurationResponseTypeDef",
     {
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
-        "FilterCriteria": FilterCriteriaOutputTypeDef,
+        "FilterCriteria": FilterCriteriaTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
         "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
         "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
@@ -2661,82 +2629,38 @@
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
-        "FilterCriteria": FilterCriteriaOutputTypeDef,
+        "FilterCriteria": FilterCriteriaTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
         "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
         "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventSourceMappingRequestRequestTypeDef",
-    {
-        "EventSourceArn": str,
-        "Enabled": bool,
-        "BatchSize": int,
-        "FilterCriteria": FilterCriteriaTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "ParallelizationFactor": int,
-        "StartingPosition": EventSourcePositionType,
-        "StartingPositionTimestamp": TimestampTypeDef,
-        "DestinationConfig": DestinationConfigTypeDef,
-        "MaximumRecordAgeInSeconds": int,
-        "BisectBatchOnFunctionError": bool,
-        "MaximumRetryAttempts": int,
-        "TumblingWindowInSeconds": int,
-        "Topics": Sequence[str],
-        "Queues": Sequence[str],
-        "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
-        "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
-        "ScalingConfig": ScalingConfigTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateEventSourceMappingRequestRequestTypeDef(
-    _RequiredCreateEventSourceMappingRequestRequestTypeDef,
-    _OptionalCreateEventSourceMappingRequestRequestTypeDef,
-):
-    pass
-
-
-FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
         "UUID": str,
     },
 )
 _OptionalUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/type_defs.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -53,23 +53,20 @@
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
-    "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
-    "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "BlobTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
-    "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
     "TimestampTypeDef",
@@ -90,15 +87,14 @@
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteFunctionUrlConfigRequestRequestTypeDef",
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
     "EnvironmentErrorTypeDef",
-    "SelfManagedEventSourceOutputTypeDef",
     "FilterTypeDef",
     "FunctionCodeLocationTypeDef",
     "LayerTypeDef",
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
@@ -115,15 +111,14 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
     "ImageConfigErrorTypeDef",
-    "ImageConfigOutputTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "LayerVersionsListItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
@@ -163,50 +158,44 @@
     "ListFunctionsByCodeSigningConfigResponseTypeDef",
     "ListTagsResponseTypeDef",
     "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
-    "AliasRoutingConfigurationUnionTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
-    "AllowedPublishersUnionTypeDef",
     "FunctionCodeTypeDef",
     "InvocationRequestRequestTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
+    "CreateFunctionUrlConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
-    "UpdateFunctionUrlConfigResponseTypeDef",
-    "CorsUnionTypeDef",
-    "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
+    "UpdateFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
-    "SelfManagedEventSourceUnionTypeDef",
-    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
     "GetFunctionRequestFunctionActiveV2WaitTypeDef",
     "GetFunctionRequestFunctionExistsWaitTypeDef",
     "GetFunctionRequestFunctionUpdatedV2WaitTypeDef",
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
-    "ImageConfigUnionTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
@@ -227,18 +216,17 @@
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
     "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
+    "CreateEventSourceMappingRequestRequestTypeDef",
     "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
-    "CreateEventSourceMappingRequestRequestTypeDef",
-    "FilterCriteriaUnionTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
     "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
@@ -328,37 +316,22 @@
 )
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
-AliasRoutingConfigurationOutputTypeDef = TypedDict(
-    "AliasRoutingConfigurationOutputTypeDef",
-    {
-        "AdditionalVersionWeights": Dict[str, float],
-    },
-    total=False,
-)
-
 AliasRoutingConfigurationTypeDef = TypedDict(
     "AliasRoutingConfigurationTypeDef",
     {
         "AdditionalVersionWeights": Mapping[str, float],
     },
     total=False,
 )
 
-AllowedPublishersOutputTypeDef = TypedDict(
-    "AllowedPublishersOutputTypeDef",
-    {
-        "SigningProfileVersionArns": List[str],
-    },
-)
-
 AllowedPublishersTypeDef = TypedDict(
     "AllowedPublishersTypeDef",
     {
         "SigningProfileVersionArns": Sequence[str],
     },
 )
 
@@ -383,27 +356,14 @@
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
     total=False,
 )
 
-CorsOutputTypeDef = TypedDict(
-    "CorsOutputTypeDef",
-    {
-        "AllowCredentials": bool,
-        "AllowHeaders": List[str],
-        "AllowMethods": List[str],
-        "AllowOrigins": List[str],
-        "ExposeHeaders": List[str],
-        "MaxAge": int,
-    },
-    total=False,
-)
-
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
@@ -655,22 +615,14 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-SelfManagedEventSourceOutputTypeDef = TypedDict(
-    "SelfManagedEventSourceOutputTypeDef",
-    {
-        "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -935,24 +887,14 @@
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-ImageConfigOutputTypeDef = TypedDict(
-    "ImageConfigOutputTypeDef",
-    {
-        "EntryPoint": List[str],
-        "Command": List[str],
-        "WorkingDirectory": str,
-    },
-    total=False,
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -1509,36 +1451,33 @@
 AliasConfigurationResponseTypeDef = TypedDict(
     "AliasConfigurationResponseTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
-        "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
+        "RoutingConfig": AliasRoutingConfigurationTypeDef,
         "RevisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
-        "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
+        "RoutingConfig": AliasRoutingConfigurationTypeDef,
         "RevisionId": str,
     },
     total=False,
 )
 
-AliasRoutingConfigurationUnionTypeDef = Union[
-    AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
-]
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
         "FunctionVersion": str,
     },
@@ -1576,15 +1515,14 @@
 )
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
-AllowedPublishersUnionTypeDef = Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef]
 FunctionCodeTypeDef = TypedDict(
     "FunctionCodeTypeDef",
     {
         "ZipFile": BlobTypeDef,
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
@@ -1688,15 +1626,15 @@
     pass
 
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
-        "AllowedPublishers": AllowedPublishersOutputTypeDef,
+        "AllowedPublishers": AllowedPublishersTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
         "LastModified": str,
     },
 )
 _OptionalCodeSigningConfigTypeDef = TypedDict(
     "_OptionalCodeSigningConfigTypeDef",
     {
@@ -1749,21 +1687,44 @@
 
 class UpdateCodeSigningConfigRequestRequestTypeDef(
     _RequiredUpdateCodeSigningConfigRequestRequestTypeDef,
     _OptionalUpdateCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+        "AuthType": FunctionUrlAuthTypeType,
+    },
+)
+_OptionalCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionUrlConfigRequestRequestTypeDef",
+    {
+        "Qualifier": str,
+        "Cors": CorsTypeDef,
+        "InvokeMode": InvokeModeType,
+    },
+    total=False,
+)
+
+class CreateFunctionUrlConfigRequestRequestTypeDef(
+    _RequiredCreateFunctionUrlConfigRequestRequestTypeDef,
+    _OptionalCreateFunctionUrlConfigRequestRequestTypeDef,
+):
+    pass
+
 CreateFunctionUrlConfigResponseTypeDef = TypedDict(
     "CreateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionUrlConfigTypeDef = TypedDict(
@@ -1775,15 +1736,15 @@
         "LastModifiedTime": str,
         "AuthType": FunctionUrlAuthTypeType,
     },
 )
 _OptionalFunctionUrlConfigTypeDef = TypedDict(
     "_OptionalFunctionUrlConfigTypeDef",
     {
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "InvokeMode": InvokeModeType,
     },
     total=False,
 )
 
 class FunctionUrlConfigTypeDef(
     _RequiredFunctionUrlConfigTypeDef, _OptionalFunctionUrlConfigTypeDef
@@ -1792,60 +1753,22 @@
 
 GetFunctionUrlConfigResponseTypeDef = TypedDict(
     "GetFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
-        "CreationTime": str,
-        "LastModifiedTime": str,
-        "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
-    "UpdateFunctionUrlConfigResponseTypeDef",
-    {
-        "FunctionUrl": str,
-        "FunctionArn": str,
-        "AuthType": FunctionUrlAuthTypeType,
-        "Cors": CorsOutputTypeDef,
+        "Cors": CorsTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
-_RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-        "AuthType": FunctionUrlAuthTypeType,
-    },
-)
-_OptionalCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionUrlConfigRequestRequestTypeDef",
-    {
-        "Qualifier": str,
-        "Cors": CorsTypeDef,
-        "InvokeMode": InvokeModeType,
-    },
-    total=False,
-)
-
-class CreateFunctionUrlConfigRequestRequestTypeDef(
-    _RequiredCreateFunctionUrlConfigRequestRequestTypeDef,
-    _OptionalCreateFunctionUrlConfigRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
@@ -1861,14 +1784,28 @@
 
 class UpdateFunctionUrlConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionUrlConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionUrlConfigRequestRequestTypeDef,
 ):
     pass
 
+UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
+    "UpdateFunctionUrlConfigResponseTypeDef",
+    {
+        "FunctionUrl": str,
+        "FunctionArn": str,
+        "AuthType": FunctionUrlAuthTypeType,
+        "Cors": CorsTypeDef,
+        "CreationTime": str,
+        "LastModifiedTime": str,
+        "InvokeMode": InvokeModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFunctionConfigurationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalUpdateFunctionConfigurationRequestRequestTypeDef = TypedDict(
@@ -1915,25 +1852,14 @@
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
     total=False,
 )
 
-SelfManagedEventSourceUnionTypeDef = Union[
-    SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
-]
-FilterCriteriaOutputTypeDef = TypedDict(
-    "FilterCriteriaOutputTypeDef",
-    {
-        "Filters": List[FilterTypeDef],
-    },
-    total=False,
-)
-
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
@@ -2095,21 +2021,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
-        "ImageConfig": ImageConfigOutputTypeDef,
+        "ImageConfig": ImageConfigTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
     total=False,
 )
 
-ImageConfigUnionTypeDef = Union[ImageConfigTypeDef, ImageConfigOutputTypeDef]
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
     total=False,
@@ -2514,35 +2439,76 @@
 
 class UpdateFunctionEventInvokeConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventSourceMappingRequestRequestTypeDef",
+    {
+        "EventSourceArn": str,
+        "Enabled": bool,
+        "BatchSize": int,
+        "FilterCriteria": FilterCriteriaTypeDef,
+        "MaximumBatchingWindowInSeconds": int,
+        "ParallelizationFactor": int,
+        "StartingPosition": EventSourcePositionType,
+        "StartingPositionTimestamp": TimestampTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
+        "MaximumRecordAgeInSeconds": int,
+        "BisectBatchOnFunctionError": bool,
+        "MaximumRetryAttempts": int,
+        "TumblingWindowInSeconds": int,
+        "Topics": Sequence[str],
+        "Queues": Sequence[str],
+        "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
+        "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateEventSourceMappingRequestRequestTypeDef(
+    _RequiredCreateEventSourceMappingRequestRequestTypeDef,
+    _OptionalCreateEventSourceMappingRequestRequestTypeDef,
+):
+    pass
+
 EventSourceMappingConfigurationResponseTypeDef = TypedDict(
     "EventSourceMappingConfigurationResponseTypeDef",
     {
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
-        "FilterCriteria": FilterCriteriaOutputTypeDef,
+        "FilterCriteria": FilterCriteriaTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
         "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
         "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
@@ -2558,80 +2524,38 @@
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
-        "FilterCriteria": FilterCriteriaOutputTypeDef,
+        "FilterCriteria": FilterCriteriaTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
         "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
         "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
+        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventSourceMappingRequestRequestTypeDef",
-    {
-        "EventSourceArn": str,
-        "Enabled": bool,
-        "BatchSize": int,
-        "FilterCriteria": FilterCriteriaTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "ParallelizationFactor": int,
-        "StartingPosition": EventSourcePositionType,
-        "StartingPositionTimestamp": TimestampTypeDef,
-        "DestinationConfig": DestinationConfigTypeDef,
-        "MaximumRecordAgeInSeconds": int,
-        "BisectBatchOnFunctionError": bool,
-        "MaximumRetryAttempts": int,
-        "TumblingWindowInSeconds": int,
-        "Topics": Sequence[str],
-        "Queues": Sequence[str],
-        "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
-        "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
-        "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
-        "ScalingConfig": ScalingConfigTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
-    },
-    total=False,
-)
-
-class CreateEventSourceMappingRequestRequestTypeDef(
-    _RequiredCreateEventSourceMappingRequestRequestTypeDef,
-    _OptionalCreateEventSourceMappingRequestRequestTypeDef,
-):
-    pass
-
-FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
         "UUID": str,
     },
 )
 _OptionalUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/waiter.py` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda/waiter.pyi` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.5.2.post1/types_aiobotocore_lambda.egg-info/SOURCES.txt` & `types-aiobotocore-lambda-2.5.2.post2/types_aiobotocore_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

