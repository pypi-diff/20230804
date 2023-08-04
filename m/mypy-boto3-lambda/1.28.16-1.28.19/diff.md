# Comparing `tmp/mypy-boto3-lambda-1.28.16.tar.gz` & `tmp/mypy-boto3-lambda-1.28.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.28.19.tar", last modified: Fri Aug  4 11:22:32 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.28.16.tar` & `mypy-boto3-lambda-1.28.19.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.356844 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59621 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59531 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80686 2023-08-01 11:22:03.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80579 2023-08-01 11:22:02.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-08-01 11:22:01.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25237 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:10.000000 mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.364844 mypy-boto3-lambda-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:22:00.000000 mypy-boto3-lambda-1.28.16/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-lambda-1.28.19/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16002 2023-08-04 11:22:32.346644 mypy-boto3-lambda-1.28.19/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14522 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4163 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4162 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      903 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59536 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59446 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14393 2023-08-04 11:22:01.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14391 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13695 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13681 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    78456 2023-08-04 11:22:02.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    78349 2023-08-04 11:22:01.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6159 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6153 2023-08-04 11:22:00.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16002 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      718 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       18 2023-08-04 11:22:32.000000 mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 11:22:32.346644 mypy-boto3-lambda-1.28.19/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1975 2023-08-04 11:21:59.000000 mypy-boto3-lambda-1.28.19/setup.py
```

### Comparing `mypy-boto3-lambda-1.28.16/LICENSE` & `mypy-boto3-lambda-1.28.19/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.Lambda 1.28.19\nVersion:         1.28.19\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,47 +43,47 @@
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
@@ -97,15 +97,15 @@
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
@@ -257,28 +257,28 @@
     def create_alias(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
 
     def create_code_signing_config(
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
@@ -288,28 +288,28 @@
     def create_event_source_mapping(
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
@@ -336,15 +336,15 @@
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
@@ -355,15 +355,15 @@
 
     def create_function_url_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -993,15 +993,15 @@
     def update_alias(
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
 
@@ -1010,15 +1010,15 @@
         """
 
     def update_code_signing_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -1027,15 +1027,15 @@
     def update_event_source_mapping(
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
@@ -1086,15 +1086,15 @@
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
@@ -1120,15 +1120,15 @@
 
     def update_function_url_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -43,47 +43,47 @@
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
@@ -97,15 +97,15 @@
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
@@ -248,27 +248,27 @@
     def create_alias(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
     def create_code_signing_config(
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
@@ -277,28 +277,28 @@
     def create_event_source_mapping(
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
@@ -324,15 +324,15 @@
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
@@ -342,15 +342,15 @@
         """
     def create_function_url_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -926,15 +926,15 @@
     def update_alias(
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
 
@@ -942,15 +942,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_alias)
         """
     def update_code_signing_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -958,15 +958,15 @@
     def update_event_source_mapping(
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
@@ -1015,15 +1015,15 @@
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
@@ -1047,15 +1047,15 @@
         """
     def update_function_url_config(
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,14 +606,15 @@
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

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -604,14 +604,15 @@
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

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/type_defs.py`

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

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/type_defs.pyi`

 * *Files 4% similar despite different names*

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

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.28.19/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.16/setup.py` & `mypy-boto3-lambda-1.28.19/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.28.16",
+    version="1.28.19",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.28.16 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.Lambda 1.28.19 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

