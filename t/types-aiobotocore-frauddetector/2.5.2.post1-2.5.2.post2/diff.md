# Comparing `tmp/types-aiobotocore-frauddetector-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-frauddetector-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-frauddetector-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-frauddetector-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-frauddetector-2.5.2.post1.tar` & `types-aiobotocore-frauddetector-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.377582 types-aiobotocore-frauddetector-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19229 2023-08-02 14:52:19.373582 types-aiobotocore-frauddetector-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.377582 types-aiobotocore-frauddetector-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.369582 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49170 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-02 14:38:59.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61114 2023-08-02 14:39:01.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61043 2023-08-02 14:38:59.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:58.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.373582 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19229 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:19.000000 types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.800267 types-aiobotocore-frauddetector-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-08-04 12:00:55.796266 types-aiobotocore-frauddetector-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.800267 types-aiobotocore-frauddetector-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.796266 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49150 2023-08-04 11:46:29.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49068 2023-08-04 11:46:29.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-04 11:46:29.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-04 11:46:29.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59400 2023-08-04 11:46:31.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59333 2023-08-04 11:46:30.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:28.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.796266 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:55.000000 types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/LICENSE` & `types-aiobotocore-frauddetector-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/setup.py` & `types-aiobotocore-frauddetector-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-frauddetector",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FraudDetector 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/__main__.py` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.FraudDetector 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/client.py` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -66,53 +66,49 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationUnionTypeDef,
+    ModelOutputConfigurationTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
-    TrainingDataSchemaUnionTypeDef,
+    TrainingDataSchemaTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FraudDetectorClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class FraudDetectorClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
     """
 
     meta: ClientMeta
@@ -121,65 +117,58 @@
     def exceptions(self) -> Exceptions:
         """
         FraudDetectorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#exceptions)
         """
-
     async def batch_create_variable(
         self, *, variableEntries: Sequence[VariableEntryTypeDef], tags: Sequence[TagTypeDef] = ...
     ) -> BatchCreateVariableResultTypeDef:
         """
         Creates a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#batch_create_variable)
         """
-
     async def batch_get_variable(self, *, names: Sequence[str]) -> BatchGetVariableResultTypeDef:
         """
         Gets a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_get_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#batch_get_variable)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#can_paginate)
         """
-
     async def cancel_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels an in-progress batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#cancel_batch_import_job)
         """
-
     async def cancel_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels the specified batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#cancel_batch_prediction_job)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#close)
         """
-
     async def create_batch_import_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -188,15 +177,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_import_job)
         """
-
     async def create_batch_prediction_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -207,15 +195,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_prediction_job)
         """
-
     async def create_detector_version(
         self,
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
@@ -225,15 +212,14 @@
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_detector_version)
         """
-
     async def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
@@ -241,15 +227,14 @@
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_list)
         """
-
     async def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -257,33 +242,31 @@
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model)
         """
-
     async def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: TrainingDataSchemaUnionTypeDef,
+        trainingDataSchema: TrainingDataSchemaTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model_version)
         """
-
     async def create_rule(
         self,
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
@@ -293,15 +276,14 @@
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_rule)
         """
-
     async def create_variable(
         self,
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
@@ -311,161 +293,143 @@
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_variable)
         """
-
     async def delete_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes the specified batch import job ID record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_batch_import_job)
         """
-
     async def delete_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_batch_prediction_job)
         """
-
     async def delete_detector(self, *, detectorId: str) -> Dict[str, Any]:
         """
         Deletes the detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_detector)
         """
-
     async def delete_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> Dict[str, Any]:
         """
         Deletes the detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_detector_version)
         """
-
     async def delete_entity_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_entity_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_entity_type)
         """
-
     async def delete_event(
         self, *, eventId: str, eventTypeName: str, deleteAuditHistory: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_event)
         """
-
     async def delete_event_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_event_type)
         """
-
     async def delete_events_by_event_type(
         self, *, eventTypeName: str
     ) -> DeleteEventsByEventTypeResultTypeDef:
         """
         Deletes all events of a particular event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_events_by_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_events_by_event_type)
         """
-
     async def delete_external_model(self, *, modelEndpoint: str) -> Dict[str, Any]:
         """
         Removes a SageMaker model from Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_external_model)
         """
-
     async def delete_label(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_label)
         """
-
     async def delete_list(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes the list, provided it is not used in a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_list)
         """
-
     async def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_model)
         """
-
     async def delete_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> Dict[str, Any]:
         """
         Deletes a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_model_version)
         """
-
     async def delete_outcome(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_outcome)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_outcome)
         """
-
     async def delete_rule(self, *, rule: RuleTypeDef) -> Dict[str, Any]:
         """
         Deletes the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_rule)
         """
-
     async def delete_variable(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_variable)
         """
-
     async def describe_detector(
         self, *, detectorId: str, nextToken: str = ..., maxResults: int = ...
     ) -> DescribeDetectorResultTypeDef:
         """
         Gets all versions for a specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#describe_detector)
         """
-
     async def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
@@ -474,97 +438,88 @@
         """
         Gets all of the model versions for the specified model type or for the specified
         model type and model ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#describe_model_versions)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#generate_presigned_url)
         """
-
     async def get_batch_import_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchImportJobsResultTypeDef:
         """
         Gets all batch import jobs or a specific job of the specified ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_batch_import_jobs)
         """
-
     async def get_batch_prediction_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchPredictionJobsResultTypeDef:
         """
         Gets all batch prediction jobs or a specific job if you specify a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_prediction_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_batch_prediction_jobs)
         """
-
     async def get_delete_events_by_event_type_status(
         self, *, eventTypeName: str
     ) -> GetDeleteEventsByEventTypeStatusResultTypeDef:
         """
         Retrieves the status of a `DeleteEventsByEventType` action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_delete_events_by_event_type_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_delete_events_by_event_type_status)
         """
-
     async def get_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> GetDetectorVersionResultTypeDef:
         """
         Gets a particular detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_detector_version)
         """
-
     async def get_detectors(
         self, *, detectorId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorsResultTypeDef:
         """
         Gets all detectors or a single detector if a `detectorId` is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_detectors)
         """
-
     async def get_entity_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEntityTypesResultTypeDef:
         """
         Gets all entity types or a specific entity type if a name is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_entity_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_entity_types)
         """
-
     async def get_event(self, *, eventId: str, eventTypeName: str) -> GetEventResultTypeDef:
         """
         Retrieves details of events stored with Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event)
         """
-
     async def get_event_prediction(
         self,
         *,
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
@@ -575,15 +530,14 @@
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction)
         """
-
     async def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
@@ -593,111 +547,101 @@
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction_metadata)
         """
-
     async def get_event_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEventTypesResultTypeDef:
         """
         Gets all event types or a specific event type if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_types)
         """
-
     async def get_external_models(
         self, *, modelEndpoint: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetExternalModelsResultTypeDef:
         """
         Gets the details for one or more Amazon SageMaker models that have been imported
         into the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_external_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_external_models)
         """
-
     async def get_kms_encryption_key(self) -> GetKMSEncryptionKeyResultTypeDef:
         """
         Gets the encryption key if a KMS key has been specified to be used to encrypt
         content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_kms_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_kms_encryption_key)
         """
-
     async def get_labels(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetLabelsResultTypeDef:
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_labels)
         """
-
     async def get_list_elements(
         self, *, name: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetListElementsResultTypeDef:
         """
         Gets all the elements in the specified list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_list_elements)
         """
-
     async def get_lists_metadata(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetListsMetadataResultTypeDef:
         """
         Gets the metadata of either all the lists under the account or the specified
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_lists_metadata)
         """
-
     async def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_model_version)
         """
-
     async def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_models)
         """
-
     async def get_outcomes(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetOutcomesResultTypeDef:
         """
         Gets one or more outcomes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_outcomes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_outcomes)
         """
-
     async def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
@@ -706,25 +650,23 @@
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_rules)
         """
-
     async def get_variables(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetVariablesResultTypeDef:
         """
         Gets all of the variables or the specific variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_variables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_variables)
         """
-
     async def list_event_predictions(
         self,
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
@@ -734,50 +676,46 @@
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_event_predictions)
         """
-
     async def list_tags_for_resource(
         self, *, resourceARN: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListTagsForResourceResultTypeDef:
         """
         Lists all tags associated with the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_tags_for_resource)
         """
-
     async def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_detector)
         """
-
     async def put_entity_type(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_entity_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_entity_type)
         """
-
     async def put_event_type(
         self,
         *,
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
@@ -788,61 +726,56 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_event_type)
         """
-
     async def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: ModelOutputConfigurationUnionTypeDef,
+        outputConfiguration: ModelOutputConfigurationTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_external_model)
         """
-
     async def put_kms_encryption_key(self, *, kmsEncryptionKeyArn: str) -> Dict[str, Any]:
         """
         Specifies the KMS key to be used to encrypt content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_kms_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_kms_encryption_key)
         """
-
     async def put_label(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_label)
         """
-
     async def put_outcome(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_outcome)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_outcome)
         """
-
     async def send_event(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
@@ -853,31 +786,28 @@
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#send_event)
         """
-
     async def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#untag_resource)
         """
-
     async def update_detector_version(
         self,
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
@@ -887,45 +817,41 @@
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version)
         """
-
     async def update_detector_version_metadata(
         self, *, detectorId: str, detectorVersionId: str, description: str
     ) -> Dict[str, Any]:
         """
         Updates the detector version's description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version_metadata)
         """
-
     async def update_detector_version_status(
         self, *, detectorId: str, detectorVersionId: str, status: DetectorVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the detector version’s status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version_status)
         """
-
     async def update_event_label(
         self, *, eventId: str, eventTypeName: str, assignedLabel: str, labelTimestamp: str
     ) -> Dict[str, Any]:
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_event_label)
         """
-
     async def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
@@ -933,25 +859,23 @@
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_list)
         """
-
     async def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model)
         """
-
     async def update_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
@@ -960,38 +884,35 @@
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version)
         """
-
     async def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
         status: ModelVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version_status)
         """
-
     async def update_rule_metadata(self, *, rule: RuleTypeDef, description: str) -> Dict[str, Any]:
         """
         Updates a rule's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_metadata)
         """
-
     async def update_rule_version(
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
@@ -1000,29 +921,26 @@
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_version)
         """
-
     async def update_variable(
         self, *, name: str, defaultValue: str = ..., description: str = ..., variableType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_variable)
         """
-
     async def __aenter__(self) -> "FraudDetectorClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
         """
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/client.pyi` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,49 +66,53 @@
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     ModelEndpointDataBlobTypeDef,
     ModelInputConfigurationTypeDef,
-    ModelOutputConfigurationUnionTypeDef,
+    ModelOutputConfigurationTypeDef,
     ModelVersionTypeDef,
     PredictionTimeRangeTypeDef,
     RuleTypeDef,
     TagTypeDef,
-    TrainingDataSchemaUnionTypeDef,
+    TrainingDataSchemaTypeDef,
     UpdateModelVersionResultTypeDef,
     UpdateRuleVersionResultTypeDef,
     VariableEntryTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("FraudDetectorClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class FraudDetectorClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
     """
 
     meta: ClientMeta
@@ -117,58 +121,65 @@
     def exceptions(self) -> Exceptions:
         """
         FraudDetectorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#exceptions)
         """
+
     async def batch_create_variable(
         self, *, variableEntries: Sequence[VariableEntryTypeDef], tags: Sequence[TagTypeDef] = ...
     ) -> BatchCreateVariableResultTypeDef:
         """
         Creates a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#batch_create_variable)
         """
+
     async def batch_get_variable(self, *, names: Sequence[str]) -> BatchGetVariableResultTypeDef:
         """
         Gets a batch of variables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.batch_get_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#batch_get_variable)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#can_paginate)
         """
+
     async def cancel_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels an in-progress batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#cancel_batch_import_job)
         """
+
     async def cancel_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Cancels the specified batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.cancel_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#cancel_batch_prediction_job)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#close)
         """
+
     async def create_batch_import_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -177,14 +188,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_import_job)
         """
+
     async def create_batch_prediction_job(
         self,
         *,
         jobId: str,
         inputPath: str,
         outputPath: str,
         eventTypeName: str,
@@ -195,14 +207,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_batch_prediction_job)
         """
+
     async def create_detector_version(
         self,
         *,
         detectorId: str,
         rules: Sequence[RuleTypeDef],
         description: str = ...,
         externalModelEndpoints: Sequence[str] = ...,
@@ -212,14 +225,15 @@
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_detector_version)
         """
+
     async def create_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         variableType: str = ...,
         description: str = ...,
@@ -227,14 +241,15 @@
     ) -> Dict[str, Any]:
         """
         Creates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_list)
         """
+
     async def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -242,31 +257,33 @@
     ) -> Dict[str, Any]:
         """
         Creates a model using the specified model type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model)
         """
+
     async def create_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         trainingDataSource: TrainingDataSourceEnumType,
-        trainingDataSchema: TrainingDataSchemaUnionTypeDef,
+        trainingDataSchema: TrainingDataSchemaTypeDef,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
         ingestedEventsDetail: IngestedEventsDetailTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelVersionResultTypeDef:
         """
         Creates a version of the model using the specified model type and model id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_model_version)
         """
+
     async def create_rule(
         self,
         *,
         ruleId: str,
         detectorId: str,
         expression: str,
         language: Literal["DETECTORPL"],
@@ -276,14 +293,15 @@
     ) -> CreateRuleResultTypeDef:
         """
         Creates a rule for use with the specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_rule)
         """
+
     async def create_variable(
         self,
         *,
         name: str,
         dataType: DataTypeType,
         dataSource: DataSourceType,
         defaultValue: str,
@@ -293,143 +311,161 @@
     ) -> Dict[str, Any]:
         """
         Creates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#create_variable)
         """
+
     async def delete_batch_import_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes the specified batch import job ID record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_batch_import_job)
         """
+
     async def delete_batch_prediction_job(self, *, jobId: str) -> Dict[str, Any]:
         """
         Deletes a batch prediction job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_batch_prediction_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_batch_prediction_job)
         """
+
     async def delete_detector(self, *, detectorId: str) -> Dict[str, Any]:
         """
         Deletes the detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_detector)
         """
+
     async def delete_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> Dict[str, Any]:
         """
         Deletes the detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_detector_version)
         """
+
     async def delete_entity_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_entity_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_entity_type)
         """
+
     async def delete_event(
         self, *, eventId: str, eventTypeName: str, deleteAuditHistory: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_event)
         """
+
     async def delete_event_type(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_event_type)
         """
+
     async def delete_events_by_event_type(
         self, *, eventTypeName: str
     ) -> DeleteEventsByEventTypeResultTypeDef:
         """
         Deletes all events of a particular event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_events_by_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_events_by_event_type)
         """
+
     async def delete_external_model(self, *, modelEndpoint: str) -> Dict[str, Any]:
         """
         Removes a SageMaker model from Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_external_model)
         """
+
     async def delete_label(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_label)
         """
+
     async def delete_list(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes the list, provided it is not used in a rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_list)
         """
+
     async def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_model)
         """
+
     async def delete_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> Dict[str, Any]:
         """
         Deletes a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_model_version)
         """
+
     async def delete_outcome(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_outcome)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_outcome)
         """
+
     async def delete_rule(self, *, rule: RuleTypeDef) -> Dict[str, Any]:
         """
         Deletes the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_rule)
         """
+
     async def delete_variable(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#delete_variable)
         """
+
     async def describe_detector(
         self, *, detectorId: str, nextToken: str = ..., maxResults: int = ...
     ) -> DescribeDetectorResultTypeDef:
         """
         Gets all versions for a specified detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#describe_detector)
         """
+
     async def describe_model_versions(
         self,
         *,
         modelId: str = ...,
         modelVersionNumber: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
@@ -438,88 +474,97 @@
         """
         Gets all of the model versions for the specified model type or for the specified
         model type and model ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.describe_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#describe_model_versions)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#generate_presigned_url)
         """
+
     async def get_batch_import_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchImportJobsResultTypeDef:
         """
         Gets all batch import jobs or a specific job of the specified ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_batch_import_jobs)
         """
+
     async def get_batch_prediction_jobs(
         self, *, jobId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> GetBatchPredictionJobsResultTypeDef:
         """
         Gets all batch prediction jobs or a specific job if you specify a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_batch_prediction_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_batch_prediction_jobs)
         """
+
     async def get_delete_events_by_event_type_status(
         self, *, eventTypeName: str
     ) -> GetDeleteEventsByEventTypeStatusResultTypeDef:
         """
         Retrieves the status of a `DeleteEventsByEventType` action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_delete_events_by_event_type_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_delete_events_by_event_type_status)
         """
+
     async def get_detector_version(
         self, *, detectorId: str, detectorVersionId: str
     ) -> GetDetectorVersionResultTypeDef:
         """
         Gets a particular detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_detector_version)
         """
+
     async def get_detectors(
         self, *, detectorId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorsResultTypeDef:
         """
         Gets all detectors or a single detector if a `detectorId` is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_detectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_detectors)
         """
+
     async def get_entity_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEntityTypesResultTypeDef:
         """
         Gets all entity types or a specific entity type if a name is specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_entity_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_entity_types)
         """
+
     async def get_event(self, *, eventId: str, eventTypeName: str) -> GetEventResultTypeDef:
         """
         Retrieves details of events stored with Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event)
         """
+
     async def get_event_prediction(
         self,
         *,
         detectorId: str,
         eventId: str,
         eventTypeName: str,
         entities: Sequence[EntityTypeDef],
@@ -530,14 +575,15 @@
     ) -> GetEventPredictionResultTypeDef:
         """
         Evaluates an event against a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction)
         """
+
     async def get_event_prediction_metadata(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         detectorId: str,
         detectorVersionId: str,
@@ -547,101 +593,111 @@
         Gets details of the past fraud predictions for the specified event ID, event
         type, detector ID, and detector version ID that was generated in the specified
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_prediction_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_prediction_metadata)
         """
+
     async def get_event_types(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetEventTypesResultTypeDef:
         """
         Gets all event types or a specific event type if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_event_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_event_types)
         """
+
     async def get_external_models(
         self, *, modelEndpoint: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetExternalModelsResultTypeDef:
         """
         Gets the details for one or more Amazon SageMaker models that have been imported
         into the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_external_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_external_models)
         """
+
     async def get_kms_encryption_key(self) -> GetKMSEncryptionKeyResultTypeDef:
         """
         Gets the encryption key if a KMS key has been specified to be used to encrypt
         content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_kms_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_kms_encryption_key)
         """
+
     async def get_labels(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetLabelsResultTypeDef:
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_labels)
         """
+
     async def get_list_elements(
         self, *, name: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetListElementsResultTypeDef:
         """
         Gets all the elements in the specified list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_list_elements)
         """
+
     async def get_lists_metadata(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetListsMetadataResultTypeDef:
         """
         Gets the metadata of either all the lists under the account or the specified
         list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_lists_metadata)
         """
+
     async def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_model_version)
         """
+
     async def get_models(
         self,
         *,
         modelId: str = ...,
         modelType: ModelTypeEnumType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetModelsResultTypeDef:
         """
         Gets one or more models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_models)
         """
+
     async def get_outcomes(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetOutcomesResultTypeDef:
         """
         Gets one or more outcomes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_outcomes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_outcomes)
         """
+
     async def get_rules(
         self,
         *,
         detectorId: str,
         ruleId: str = ...,
         ruleVersion: str = ...,
         nextToken: str = ...,
@@ -650,23 +706,25 @@
         """
         Get all rules for a detector (paginated) if `ruleId` and `ruleVersion` are not
         specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_rules)
         """
+
     async def get_variables(
         self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetVariablesResultTypeDef:
         """
         Gets all of the variables or the specific variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_variables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#get_variables)
         """
+
     async def list_event_predictions(
         self,
         *,
         eventId: FilterConditionTypeDef = ...,
         eventType: FilterConditionTypeDef = ...,
         detectorId: FilterConditionTypeDef = ...,
         detectorVersionId: FilterConditionTypeDef = ...,
@@ -676,46 +734,50 @@
     ) -> ListEventPredictionsResultTypeDef:
         """
         Gets a list of past predictions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_event_predictions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_event_predictions)
         """
+
     async def list_tags_for_resource(
         self, *, resourceARN: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListTagsForResourceResultTypeDef:
         """
         Lists all tags associated with the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#list_tags_for_resource)
         """
+
     async def put_detector(
         self,
         *,
         detectorId: str,
         eventTypeName: str,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_detector)
         """
+
     async def put_entity_type(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an entity type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_entity_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_entity_type)
         """
+
     async def put_event_type(
         self,
         *,
         name: str,
         eventVariables: Sequence[str],
         entityTypes: Sequence[str],
         description: str = ...,
@@ -726,56 +788,61 @@
     ) -> Dict[str, Any]:
         """
         Creates or updates an event type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_event_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_event_type)
         """
+
     async def put_external_model(
         self,
         *,
         modelEndpoint: str,
         modelSource: Literal["SAGEMAKER"],
         invokeModelEndpointRoleArn: str,
         inputConfiguration: ModelInputConfigurationTypeDef,
-        outputConfiguration: ModelOutputConfigurationUnionTypeDef,
+        outputConfiguration: ModelOutputConfigurationTypeDef,
         modelEndpointStatus: ModelEndpointStatusType,
         tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon SageMaker model endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_external_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_external_model)
         """
+
     async def put_kms_encryption_key(self, *, kmsEncryptionKeyArn: str) -> Dict[str, Any]:
         """
         Specifies the KMS key to be used to encrypt content in Amazon Fraud Detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_kms_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_kms_encryption_key)
         """
+
     async def put_label(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_label)
         """
+
     async def put_outcome(
         self, *, name: str, description: str = ..., tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates an outcome.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.put_outcome)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#put_outcome)
         """
+
     async def send_event(
         self,
         *,
         eventId: str,
         eventTypeName: str,
         eventTimestamp: str,
         eventVariables: Mapping[str, str],
@@ -786,28 +853,31 @@
         """
         Stores events in Amazon Fraud Detector without generating fraud predictions for
         those events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.send_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#send_event)
         """
+
     async def tag_resource(self, *, resourceARN: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Assigns tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#untag_resource)
         """
+
     async def update_detector_version(
         self,
         *,
         detectorId: str,
         detectorVersionId: str,
         externalModelEndpoints: Sequence[str],
         rules: Sequence[RuleTypeDef],
@@ -817,41 +887,45 @@
     ) -> Dict[str, Any]:
         """
         Updates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version)
         """
+
     async def update_detector_version_metadata(
         self, *, detectorId: str, detectorVersionId: str, description: str
     ) -> Dict[str, Any]:
         """
         Updates the detector version's description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version_metadata)
         """
+
     async def update_detector_version_status(
         self, *, detectorId: str, detectorVersionId: str, status: DetectorVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the detector version’s status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_detector_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_detector_version_status)
         """
+
     async def update_event_label(
         self, *, eventId: str, eventTypeName: str, assignedLabel: str, labelTimestamp: str
     ) -> Dict[str, Any]:
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_event_label)
         """
+
     async def update_list(
         self,
         *,
         name: str,
         elements: Sequence[str] = ...,
         description: str = ...,
         updateMode: ListUpdateModeType = ...,
@@ -859,23 +933,25 @@
     ) -> Dict[str, Any]:
         """
         Updates a list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_list)
         """
+
     async def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model)
         """
+
     async def update_model_version(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         majorVersionNumber: str,
         externalEventsDetail: ExternalEventsDetailTypeDef = ...,
@@ -884,35 +960,38 @@
     ) -> UpdateModelVersionResultTypeDef:
         """
         Updates a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version)
         """
+
     async def update_model_version_status(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         modelVersionNumber: str,
         status: ModelVersionStatusType
     ) -> Dict[str, Any]:
         """
         Updates the status of a model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model_version_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_model_version_status)
         """
+
     async def update_rule_metadata(self, *, rule: RuleTypeDef, description: str) -> Dict[str, Any]:
         """
         Updates a rule's metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_metadata)
         """
+
     async def update_rule_version(
         self,
         *,
         rule: RuleTypeDef,
         expression: str,
         language: Literal["DETECTORPL"],
         outcomes: Sequence[str],
@@ -921,26 +1000,29 @@
     ) -> UpdateRuleVersionResultTypeDef:
         """
         Updates a rule version resulting in a new rule version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_rule_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_rule_version)
         """
+
     async def update_variable(
         self, *, name: str, defaultValue: str = ..., description: str = ..., variableType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a variable.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_variable)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/#update_variable)
         """
+
     async def __aenter__(self) -> "FraudDetectorClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/client/)
         """
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/literals.py` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/literals.pyi` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/type_defs.py` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     "EvaluatedRuleTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
     "ExternalModelSummaryTypeDef",
     "ModelInputConfigurationTypeDef",
-    "ModelOutputConfigurationOutputTypeDef",
+    "ModelOutputConfigurationTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
@@ -118,21 +118,19 @@
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
     "IngestedEventsTimeWindowTypeDef",
-    "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
-    "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
@@ -186,39 +184,36 @@
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
+    "PutExternalModelRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
     "IngestedEventsDetailTypeDef",
-    "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
-    "ModelOutputConfigurationUnionTypeDef",
-    "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
     "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
-    "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
-    "TrainingDataSchemaUnionTypeDef",
+    "GetModelVersionResultTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -777,32 +772,32 @@
 
 class ModelInputConfigurationTypeDef(
     _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
 
-_RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationOutputTypeDef",
+_RequiredModelOutputConfigurationTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
-_OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationOutputTypeDef",
+_OptionalModelOutputConfigurationTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationTypeDef",
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
 
-class ModelOutputConfigurationOutputTypeDef(
-    _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
+class ModelOutputConfigurationTypeDef(
+    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
 
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
@@ -1087,23 +1082,14 @@
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
 
-LabelSchemaOutputTypeDef = TypedDict(
-    "LabelSchemaOutputTypeDef",
-    {
-        "labelMapper": Dict[str, List[str]],
-        "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
-    },
-    total=False,
-)
-
 LabelSchemaTypeDef = TypedDict(
     "LabelSchemaTypeDef",
     {
         "labelMapper": Mapping[str, Sequence[str]],
         "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
     },
     total=False,
@@ -1156,36 +1142,14 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
-_RequiredModelOutputConfigurationTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationTypeDef",
-    {
-        "format": ModelOutputDataFormatType,
-    },
-)
-_OptionalModelOutputConfigurationTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationTypeDef",
-    {
-        "jsonKeyToVariableMap": Mapping[str, str],
-        "csvIndexToVariableMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class ModelOutputConfigurationTypeDef(
-    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
-):
-    pass
-
-
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -2045,23 +2009,49 @@
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
         "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_RequiredPutExternalModelRequestRequestTypeDef",
+    {
+        "modelEndpoint": str,
+        "modelSource": Literal["SAGEMAKER"],
+        "invokeModelEndpointRoleArn": str,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "modelEndpointStatus": ModelEndpointStatusType,
+    },
+)
+_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_OptionalPutExternalModelRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutExternalModelRequestRequestTypeDef(
+    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
+):
+    pass
+
+
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2105,35 +2095,14 @@
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
     },
 )
 
-_RequiredTrainingDataSchemaOutputTypeDef = TypedDict(
-    "_RequiredTrainingDataSchemaOutputTypeDef",
-    {
-        "modelVariables": List[str],
-    },
-)
-_OptionalTrainingDataSchemaOutputTypeDef = TypedDict(
-    "_OptionalTrainingDataSchemaOutputTypeDef",
-    {
-        "labelSchema": LabelSchemaOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TrainingDataSchemaOutputTypeDef(
-    _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
-):
-    pass
-
-
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
@@ -2178,43 +2147,14 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
-ModelOutputConfigurationUnionTypeDef = Union[
-    ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
-]
-_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_RequiredPutExternalModelRequestRequestTypeDef",
-    {
-        "modelEndpoint": str,
-        "modelSource": Literal["SAGEMAKER"],
-        "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
-        "modelEndpointStatus": ModelEndpointStatusType,
-    },
-)
-_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_OptionalPutExternalModelRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutExternalModelRequestRequestTypeDef(
-    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
-):
-    pass
-
-
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2324,30 +2264,14 @@
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
 
-GetModelVersionResultTypeDef = TypedDict(
-    "GetModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
-        "status": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2367,15 +2291,30 @@
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
 
-TrainingDataSchemaUnionTypeDef = Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef]
+GetModelVersionResultTypeDef = TypedDict(
+    "GetModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "trainingDataSource": TrainingDataSourceEnumType,
+        "trainingDataSchema": TrainingDataSchemaTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
+        "status": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2468,15 +2407,15 @@
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "trainingDataSchema": TrainingDataSchemaTypeDef,
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector/type_defs.pyi` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     "EvaluatedRuleTypeDef",
     "EventOrchestrationTypeDef",
     "EventPredictionSummaryTypeDef",
     "IngestedEventStatisticsTypeDef",
     "EventVariableSummaryTypeDef",
     "ExternalModelSummaryTypeDef",
     "ModelInputConfigurationTypeDef",
-    "ModelOutputConfigurationOutputTypeDef",
+    "ModelOutputConfigurationTypeDef",
     "FilterConditionTypeDef",
     "GetBatchImportJobsRequestRequestTypeDef",
     "GetBatchPredictionJobsRequestRequestTypeDef",
     "GetDeleteEventsByEventTypeStatusRequestRequestTypeDef",
     "GetDetectorVersionRequestRequestTypeDef",
     "GetDetectorsRequestRequestTypeDef",
     "GetEntityTypesRequestRequestTypeDef",
@@ -117,21 +117,19 @@
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
     "GetVariablesRequestRequestTypeDef",
     "IngestedEventsTimeWindowTypeDef",
-    "LabelSchemaOutputTypeDef",
     "LabelSchemaTypeDef",
     "PredictionTimeRangeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogOddsMetricTypeDef",
     "MetricDataPointTypeDef",
-    "ModelOutputConfigurationTypeDef",
     "OFIMetricDataPointTypeDef",
     "UncertaintyRangeTypeDef",
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
@@ -185,39 +183,36 @@
     "SendEventRequestRequestTypeDef",
     "GetEntityTypesResultTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "ListEventPredictionsResultTypeDef",
     "EventTypeTypeDef",
     "ExternalModelOutputsTypeDef",
     "ExternalModelTypeDef",
+    "PutExternalModelRequestRequestTypeDef",
     "GetKMSEncryptionKeyResultTypeDef",
     "GetLabelsResultTypeDef",
     "GetModelsResultTypeDef",
     "GetOutcomesResultTypeDef",
     "GetRulesResultTypeDef",
     "IngestedEventsDetailTypeDef",
-    "TrainingDataSchemaOutputTypeDef",
     "TrainingDataSchemaTypeDef",
     "ListEventPredictionsRequestRequestTypeDef",
     "VariableImportanceMetricsTypeDef",
     "TrainingMetricsTypeDef",
-    "ModelOutputConfigurationUnionTypeDef",
-    "PutExternalModelRequestRequestTypeDef",
     "OFIModelPerformanceTypeDef",
     "TFIModelPerformanceTypeDef",
     "PredictionExplanationsTypeDef",
     "GetEventPredictionRequestRequestTypeDef",
     "GetEventResultTypeDef",
     "GetEventTypesResultTypeDef",
     "GetEventPredictionResultTypeDef",
     "GetExternalModelsResultTypeDef",
     "UpdateModelVersionRequestRequestTypeDef",
-    "GetModelVersionResultTypeDef",
     "CreateModelVersionRequestRequestTypeDef",
-    "TrainingDataSchemaUnionTypeDef",
+    "GetModelVersionResultTypeDef",
     "TrainingResultTypeDef",
     "OFITrainingMetricsValueTypeDef",
     "TFITrainingMetricsValueTypeDef",
     "ModelVersionEvaluationTypeDef",
     "TrainingMetricsV2TypeDef",
     "EvaluatedModelVersionTypeDef",
     "TrainingResultV2TypeDef",
@@ -766,31 +761,31 @@
 )
 
 class ModelInputConfigurationTypeDef(
     _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
-_RequiredModelOutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationOutputTypeDef",
+_RequiredModelOutputConfigurationTypeDef = TypedDict(
+    "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
-_OptionalModelOutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationOutputTypeDef",
+_OptionalModelOutputConfigurationTypeDef = TypedDict(
+    "_OptionalModelOutputConfigurationTypeDef",
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
-class ModelOutputConfigurationOutputTypeDef(
-    _RequiredModelOutputConfigurationOutputTypeDef, _OptionalModelOutputConfigurationOutputTypeDef
+class ModelOutputConfigurationTypeDef(
+    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
@@ -1070,23 +1065,14 @@
     "IngestedEventsTimeWindowTypeDef",
     {
         "startTime": str,
         "endTime": str,
     },
 )
 
-LabelSchemaOutputTypeDef = TypedDict(
-    "LabelSchemaOutputTypeDef",
-    {
-        "labelMapper": Dict[str, List[str]],
-        "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
-    },
-    total=False,
-)
-
 LabelSchemaTypeDef = TypedDict(
     "LabelSchemaTypeDef",
     {
         "labelMapper": Mapping[str, Sequence[str]],
         "unlabeledEventsTreatment": UnlabeledEventsTreatmentType,
     },
     total=False,
@@ -1137,34 +1123,14 @@
         "precision": float,
         "tpr": float,
         "threshold": float,
     },
     total=False,
 )
 
-_RequiredModelOutputConfigurationTypeDef = TypedDict(
-    "_RequiredModelOutputConfigurationTypeDef",
-    {
-        "format": ModelOutputDataFormatType,
-    },
-)
-_OptionalModelOutputConfigurationTypeDef = TypedDict(
-    "_OptionalModelOutputConfigurationTypeDef",
-    {
-        "jsonKeyToVariableMap": Mapping[str, str],
-        "csvIndexToVariableMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-class ModelOutputConfigurationTypeDef(
-    _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
-):
-    pass
-
 OFIMetricDataPointTypeDef = TypedDict(
     "OFIMetricDataPointTypeDef",
     {
         "fpr": float,
         "precision": float,
         "tpr": float,
         "threshold": float,
@@ -1986,23 +1952,47 @@
 ExternalModelTypeDef = TypedDict(
     "ExternalModelTypeDef",
     {
         "modelEndpoint": str,
         "modelSource": Literal["SAGEMAKER"],
         "invokeModelEndpointRoleArn": str,
         "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationOutputTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
         "modelEndpointStatus": ModelEndpointStatusType,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_RequiredPutExternalModelRequestRequestTypeDef",
+    {
+        "modelEndpoint": str,
+        "modelSource": Literal["SAGEMAKER"],
+        "invokeModelEndpointRoleArn": str,
+        "inputConfiguration": ModelInputConfigurationTypeDef,
+        "outputConfiguration": ModelOutputConfigurationTypeDef,
+        "modelEndpointStatus": ModelEndpointStatusType,
+    },
+)
+_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
+    "_OptionalPutExternalModelRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutExternalModelRequestRequestTypeDef(
+    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
+):
+    pass
+
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2046,33 +2036,14 @@
 IngestedEventsDetailTypeDef = TypedDict(
     "IngestedEventsDetailTypeDef",
     {
         "ingestedEventsTimeWindow": IngestedEventsTimeWindowTypeDef,
     },
 )
 
-_RequiredTrainingDataSchemaOutputTypeDef = TypedDict(
-    "_RequiredTrainingDataSchemaOutputTypeDef",
-    {
-        "modelVariables": List[str],
-    },
-)
-_OptionalTrainingDataSchemaOutputTypeDef = TypedDict(
-    "_OptionalTrainingDataSchemaOutputTypeDef",
-    {
-        "labelSchema": LabelSchemaOutputTypeDef,
-    },
-    total=False,
-)
-
-class TrainingDataSchemaOutputTypeDef(
-    _RequiredTrainingDataSchemaOutputTypeDef, _OptionalTrainingDataSchemaOutputTypeDef
-):
-    pass
-
 _RequiredTrainingDataSchemaTypeDef = TypedDict(
     "_RequiredTrainingDataSchemaTypeDef",
     {
         "modelVariables": Sequence[str],
     },
 )
 _OptionalTrainingDataSchemaTypeDef = TypedDict(
@@ -2115,41 +2086,14 @@
     {
         "auc": float,
         "metricDataPoints": List[MetricDataPointTypeDef],
     },
     total=False,
 )
 
-ModelOutputConfigurationUnionTypeDef = Union[
-    ModelOutputConfigurationTypeDef, ModelOutputConfigurationOutputTypeDef
-]
-_RequiredPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_RequiredPutExternalModelRequestRequestTypeDef",
-    {
-        "modelEndpoint": str,
-        "modelSource": Literal["SAGEMAKER"],
-        "invokeModelEndpointRoleArn": str,
-        "inputConfiguration": ModelInputConfigurationTypeDef,
-        "outputConfiguration": ModelOutputConfigurationTypeDef,
-        "modelEndpointStatus": ModelEndpointStatusType,
-    },
-)
-_OptionalPutExternalModelRequestRequestTypeDef = TypedDict(
-    "_OptionalPutExternalModelRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutExternalModelRequestRequestTypeDef(
-    _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
-):
-    pass
-
 OFIModelPerformanceTypeDef = TypedDict(
     "OFIModelPerformanceTypeDef",
     {
         "auc": float,
         "uncertaintyRange": UncertaintyRangeTypeDef,
     },
     total=False,
@@ -2255,30 +2199,14 @@
 
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-GetModelVersionResultTypeDef = TypedDict(
-    "GetModelVersionResultTypeDef",
-    {
-        "modelId": str,
-        "modelType": ModelTypeEnumType,
-        "modelVersionNumber": str,
-        "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
-        "externalEventsDetail": ExternalEventsDetailTypeDef,
-        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
-        "status": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2296,15 +2224,30 @@
 
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-TrainingDataSchemaUnionTypeDef = Union[TrainingDataSchemaTypeDef, TrainingDataSchemaOutputTypeDef]
+GetModelVersionResultTypeDef = TypedDict(
+    "GetModelVersionResultTypeDef",
+    {
+        "modelId": str,
+        "modelType": ModelTypeEnumType,
+        "modelVersionNumber": str,
+        "trainingDataSource": TrainingDataSourceEnumType,
+        "trainingDataSchema": TrainingDataSchemaTypeDef,
+        "externalEventsDetail": ExternalEventsDetailTypeDef,
+        "ingestedEventsDetail": IngestedEventsDetailTypeDef,
+        "status": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TrainingResultTypeDef = TypedDict(
     "TrainingResultTypeDef",
     {
         "dataValidationMetrics": DataValidationMetricsTypeDef,
         "trainingMetrics": TrainingMetricsTypeDef,
         "variableImportanceMetrics": VariableImportanceMetricsTypeDef,
     },
@@ -2397,15 +2340,15 @@
     "ModelVersionDetailTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": str,
         "trainingDataSource": TrainingDataSourceEnumType,
-        "trainingDataSchema": TrainingDataSchemaOutputTypeDef,
+        "trainingDataSchema": TrainingDataSchemaTypeDef,
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "trainingResult": TrainingResultTypeDef,
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
         "trainingResultV2": TrainingResultV2TypeDef,
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post1/types_aiobotocore_frauddetector.egg-info/SOURCES.txt` & `types-aiobotocore-frauddetector-2.5.2.post2/types_aiobotocore_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

