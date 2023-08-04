# Comparing `tmp/types-aiobotocore-logs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-logs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-logs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-logs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-logs-2.5.2.post1.tar` & `types-aiobotocore-logs-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.845533 types-aiobotocore-logs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-08-02 14:52:35.845533 types-aiobotocore-logs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.845533 types-aiobotocore-logs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 14:42:27.000000 types-aiobotocore-logs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.837533 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40498 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37469 2023-08-02 14:42:31.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37436 2023-08-02 14:42:29.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:28.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.845533 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:35.000000 types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12669 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2531 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2530 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      940 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40743 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40674 2023-08-04 13:43:20.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10812 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10810 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12339 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12328 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37094 2023-08-04 13:43:22.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37061 2023-08-04 13:43:22.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:16.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-logs-2.5.2.post1/LICENSE` & `types-aiobotocore-logs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post1/setup.py` & `types-aiobotocore-logs-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-logs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__init__.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__init__.pyi` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/__main__.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchLogs 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
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

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/client.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
-    MetricTransformationUnionTypeDef,
+    MetricTransformationTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
@@ -68,26 +68,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchLogsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DataAlreadyAcceptedException: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     InvalidSequenceTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
@@ -95,15 +92,14 @@
     OperationAbortedException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnrecognizedClientException: Type[BotocoreClientError]
 
-
 class CloudWatchLogsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
     """
 
     meta: ClientMeta
@@ -112,49 +108,45 @@
     def exceptions(self) -> Exceptions:
         """
         CloudWatchLogsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#exceptions)
         """
-
     async def associate_kms_key(
-        self, *, logGroupName: str, kmsKeyId: str
+        self, *, kmsKeyId: str, logGroupName: str = ..., resourceIdentifier: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Associates the specified KMS key with the specified log group.
+        Associates the specified KMS key with either one log group in the account, or
+        with all stored CloudWatch Logs query insights results in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.associate_kms_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#associate_kms_key)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#can_paginate)
         """
-
     async def cancel_export_task(self, *, taskId: str) -> EmptyResponseMetadataTypeDef:
         """
         Cancels the specified export task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.cancel_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#cancel_export_task)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#close)
         """
-
     async def create_export_task(
         self,
         *,
         logGroupName: str,
         fromTime: int,
         to: int,
         destination: str,
@@ -165,171 +157,155 @@
         """
         Creates an export task so that you can efficiently export data from a log group
         to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_export_task)
         """
-
     async def create_log_group(
         self, *, logGroupName: str, kmsKeyId: str = ..., tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log group with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_group)
         """
-
     async def create_log_stream(
         self, *, logGroupName: str, logStreamName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log stream for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_stream)
         """
-
     async def delete_account_policy(
         self, *, policyName: str, policyType: Literal["DATA_PROTECTION_POLICY"]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudWatch Logs account policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_account_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_account_policy)
         """
-
     async def delete_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the data protection policy from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_data_protection_policy)
         """
-
     async def delete_destination(self, *, destinationName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified destination, and eventually disables all the subscription
         filters that publish to it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_destination)
         """
-
     async def delete_log_group(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified log group and permanently deletes all the archived log
         events associated with the log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_log_group)
         """
-
     async def delete_log_stream(
         self, *, logGroupName: str, logStreamName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified log stream and permanently deletes all the archived log
         events associated with the log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_log_stream)
         """
-
     async def delete_metric_filter(
         self, *, logGroupName: str, filterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified metric filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_metric_filter)
         """
-
     async def delete_query_definition(
         self, *, queryDefinitionId: str
     ) -> DeleteQueryDefinitionResponseTypeDef:
         """
         Deletes a saved CloudWatch Logs Insights query definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_query_definition)
         """
-
     async def delete_resource_policy(
         self, *, policyName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a resource policy from this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_resource_policy)
         """
-
     async def delete_retention_policy(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified retention policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_retention_policy)
         """
-
     async def delete_subscription_filter(
         self, *, logGroupName: str, filterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified subscription filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_subscription_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_subscription_filter)
         """
-
     async def describe_account_policies(
         self,
         *,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         policyName: str = ...,
         accountIdentifiers: Sequence[str] = ...
     ) -> DescribeAccountPoliciesResponseTypeDef:
         """
         Returns a list of all CloudWatch Logs account policies in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_account_policies)
         """
-
     async def describe_destinations(
         self, *, DestinationNamePrefix: str = ..., nextToken: str = ..., limit: int = ...
     ) -> DescribeDestinationsResponseTypeDef:
         """
         Lists all your destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_destinations)
         """
-
     async def describe_export_tasks(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
         nextToken: str = ...,
         limit: int = ...
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Lists the specified export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_export_tasks)
         """
-
     async def describe_log_groups(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         nextToken: str = ...,
@@ -338,15 +314,14 @@
     ) -> DescribeLogGroupsResponseTypeDef:
         """
         Lists the specified log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_groups)
         """
-
     async def describe_log_streams(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
@@ -356,15 +331,14 @@
     ) -> DescribeLogStreamsResponseTypeDef:
         """
         Lists the log streams for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_streams)
         """
-
     async def describe_metric_filters(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...,
@@ -373,15 +347,14 @@
     ) -> DescribeMetricFiltersResponseTypeDef:
         """
         Lists the specified metric filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_metric_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_metric_filters)
         """
-
     async def describe_queries(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -389,59 +362,57 @@
         """
         Returns a list of CloudWatch Logs Insights queries that are scheduled, running,
         or have been run recently in this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_queries)
         """
-
     async def describe_query_definitions(
         self, *, queryDefinitionNamePrefix: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeQueryDefinitionsResponseTypeDef:
         """
         This operation returns a paginated list of your saved CloudWatch Logs Insights
         query definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_query_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_query_definitions)
         """
-
     async def describe_resource_policies(
         self, *, nextToken: str = ..., limit: int = ...
     ) -> DescribeResourcePoliciesResponseTypeDef:
         """
         Lists the resource policies in this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_resource_policies)
         """
-
     async def describe_subscription_filters(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...
     ) -> DescribeSubscriptionFiltersResponseTypeDef:
         """
         Lists the subscription filters for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_subscription_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_subscription_filters)
         """
-
-    async def disassociate_kms_key(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
+    async def disassociate_kms_key(
+        self, *, logGroupName: str = ..., resourceIdentifier: str = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
-        Disassociates the associated KMS key from the specified log group.
+        Disassociates the specified KMS key from the specified log group or from all
+        CloudWatch Logs Insights query results in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.disassociate_kms_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#disassociate_kms_key)
         """
-
     async def filter_log_events(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
@@ -455,39 +426,36 @@
     ) -> FilterLogEventsResponseTypeDef:
         """
         Lists log events from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.filter_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#filter_log_events)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#generate_presigned_url)
         """
-
     async def get_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> GetDataProtectionPolicyResponseTypeDef:
         """
         Returns information about a log group data protection policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_data_protection_policy)
         """
-
     async def get_log_events(
         self,
         *,
         logStreamName: str,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         startTime: int = ...,
@@ -499,62 +467,56 @@
     ) -> GetLogEventsResponseTypeDef:
         """
         Lists log events from the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_events)
         """
-
     async def get_log_group_fields(
         self, *, logGroupName: str = ..., time: int = ..., logGroupIdentifier: str = ...
     ) -> GetLogGroupFieldsResponseTypeDef:
         """
         Returns a list of the fields that are included in log events in the specified
         log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_group_fields)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_group_fields)
         """
-
     async def get_log_record(
         self, *, logRecordPointer: str, unmask: bool = ...
     ) -> GetLogRecordResponseTypeDef:
         """
         Retrieves all of the fields and values of a single log event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_record)
         """
-
     async def get_query_results(self, *, queryId: str) -> GetQueryResultsResponseTypeDef:
         """
         Returns the results from the specified query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_query_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_query_results)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with a CloudWatch Logs resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_tags_for_resource)
         """
-
     async def list_tags_log_group(self, *, logGroupName: str) -> ListTagsLogGroupResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_tags_log_group)
         """
-
     async def put_account_policy(
         self,
         *,
         policyName: str,
         policyDocument: str,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         scope: Literal["ALL"] = ...
@@ -562,112 +524,103 @@
         """
         Creates an account-level data protection policy that applies to all log groups
         in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_account_policy)
         """
-
     async def put_data_protection_policy(
         self, *, logGroupIdentifier: str, policyDocument: str
     ) -> PutDataProtectionPolicyResponseTypeDef:
         """
         Creates a data protection policy for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_data_protection_policy)
         """
-
     async def put_destination(
         self, *, destinationName: str, targetArn: str, roleArn: str, tags: Mapping[str, str] = ...
     ) -> PutDestinationResponseTypeDef:
         """
         Creates or updates a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_destination)
         """
-
     async def put_destination_policy(
         self, *, destinationName: str, accessPolicy: str, forceUpdate: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an access policy associated with an existing destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_destination_policy)
         """
-
     async def put_log_events(
         self,
         *,
         logGroupName: str,
         logStreamName: str,
         logEvents: Sequence[InputLogEventTypeDef],
         sequenceToken: str = ...
     ) -> PutLogEventsResponseTypeDef:
         """
         Uploads a batch of log events to the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_log_events)
         """
-
     async def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationUnionTypeDef]
+        metricTransformations: Sequence[MetricTransformationTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_metric_filter)
         """
-
     async def put_query_definition(
         self,
         *,
         name: str,
         queryString: str,
         queryDefinitionId: str = ...,
         logGroupNames: Sequence[str] = ...
     ) -> PutQueryDefinitionResponseTypeDef:
         """
         Creates or updates a query definition for CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_query_definition)
         """
-
     async def put_resource_policy(
         self, *, policyName: str = ..., policyDocument: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a resource policy allowing other Amazon Web Services services
         to put log events to this account, such as Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_resource_policy)
         """
-
     async def put_retention_policy(
         self, *, logGroupName: str, retentionInDays: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the retention of the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_retention_policy)
         """
-
     async def put_subscription_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
         destinationArn: str,
@@ -677,15 +630,14 @@
         """
         Creates or updates a subscription filter and associates it with the specified
         log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_subscription_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_subscription_filter)
         """
-
     async def start_query(
         self,
         *,
         startTime: int,
         endTime: int,
         queryString: str,
         logGroupName: str = ...,
@@ -695,160 +647,143 @@
     ) -> StartQueryResponseTypeDef:
         """
         Schedules a query of a log group using CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_query)
         """
-
     async def stop_query(self, *, queryId: str) -> StopQueryResponseTypeDef:
         """
         Stops a CloudWatch Logs Insights query that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.stop_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#stop_query)
         """
-
     async def tag_log_group(
         self, *, logGroupName: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#tag_log_group)
         """
-
     async def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Assigns one or more tags (key-value pairs) to the specified CloudWatch Logs
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#tag_resource)
         """
-
     async def test_metric_filter(
         self, *, filterPattern: str, logEventMessages: Sequence[str]
     ) -> TestMetricFilterResponseTypeDef:
         """
         Tests the filter pattern of a metric filter against a sample of log event
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.test_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#test_metric_filter)
         """
-
     async def untag_log_group(
         self, *, logGroupName: str, tags: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#untag_log_group)
         """
-
     async def untag_resource(
         self, *, resourceArn: str, tagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes one or more tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#untag_resource)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_destinations"]
     ) -> DescribeDestinationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_export_tasks"]
     ) -> DescribeExportTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_log_groups"]
     ) -> DescribeLogGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_log_streams"]
     ) -> DescribeLogStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_metric_filters"]
     ) -> DescribeMetricFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_queries"]
     ) -> DescribeQueriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_resource_policies"]
     ) -> DescribeResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_subscription_filters"]
     ) -> DescribeSubscriptionFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["filter_log_events"]
     ) -> FilterLogEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "CloudWatchLogsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
         """
```

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/client.pyi` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     GetLogEventsResponseTypeDef,
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
-    MetricTransformationUnionTypeDef,
+    MetricTransformationTypeDef,
     PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
@@ -68,23 +68,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CloudWatchLogsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DataAlreadyAcceptedException: Type[BotocoreClientError]
     InvalidOperationException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     InvalidSequenceTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
@@ -92,14 +95,15 @@
     OperationAbortedException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     UnrecognizedClientException: Type[BotocoreClientError]
 
+
 class CloudWatchLogsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
     """
 
     meta: ClientMeta
@@ -108,44 +112,50 @@
     def exceptions(self) -> Exceptions:
         """
         CloudWatchLogsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#exceptions)
         """
+
     async def associate_kms_key(
-        self, *, logGroupName: str, kmsKeyId: str
+        self, *, kmsKeyId: str, logGroupName: str = ..., resourceIdentifier: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Associates the specified KMS key with the specified log group.
+        Associates the specified KMS key with either one log group in the account, or
+        with all stored CloudWatch Logs query insights results in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.associate_kms_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#associate_kms_key)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#can_paginate)
         """
+
     async def cancel_export_task(self, *, taskId: str) -> EmptyResponseMetadataTypeDef:
         """
         Cancels the specified export task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.cancel_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#cancel_export_task)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#close)
         """
+
     async def create_export_task(
         self,
         *,
         logGroupName: str,
         fromTime: int,
         to: int,
         destination: str,
@@ -156,155 +166,171 @@
         """
         Creates an export task so that you can efficiently export data from a log group
         to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_export_task)
         """
+
     async def create_log_group(
         self, *, logGroupName: str, kmsKeyId: str = ..., tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log group with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_group)
         """
+
     async def create_log_stream(
         self, *, logGroupName: str, logStreamName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log stream for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_stream)
         """
+
     async def delete_account_policy(
         self, *, policyName: str, policyType: Literal["DATA_PROTECTION_POLICY"]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudWatch Logs account policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_account_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_account_policy)
         """
+
     async def delete_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the data protection policy from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_data_protection_policy)
         """
+
     async def delete_destination(self, *, destinationName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified destination, and eventually disables all the subscription
         filters that publish to it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_destination)
         """
+
     async def delete_log_group(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified log group and permanently deletes all the archived log
         events associated with the log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_log_group)
         """
+
     async def delete_log_stream(
         self, *, logGroupName: str, logStreamName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified log stream and permanently deletes all the archived log
         events associated with the log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_log_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_log_stream)
         """
+
     async def delete_metric_filter(
         self, *, logGroupName: str, filterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified metric filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_metric_filter)
         """
+
     async def delete_query_definition(
         self, *, queryDefinitionId: str
     ) -> DeleteQueryDefinitionResponseTypeDef:
         """
         Deletes a saved CloudWatch Logs Insights query definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_query_definition)
         """
+
     async def delete_resource_policy(
         self, *, policyName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a resource policy from this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_resource_policy)
         """
+
     async def delete_retention_policy(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified retention policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_retention_policy)
         """
+
     async def delete_subscription_filter(
         self, *, logGroupName: str, filterName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified subscription filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_subscription_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#delete_subscription_filter)
         """
+
     async def describe_account_policies(
         self,
         *,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         policyName: str = ...,
         accountIdentifiers: Sequence[str] = ...
     ) -> DescribeAccountPoliciesResponseTypeDef:
         """
         Returns a list of all CloudWatch Logs account policies in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_account_policies)
         """
+
     async def describe_destinations(
         self, *, DestinationNamePrefix: str = ..., nextToken: str = ..., limit: int = ...
     ) -> DescribeDestinationsResponseTypeDef:
         """
         Lists all your destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_destinations)
         """
+
     async def describe_export_tasks(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
         nextToken: str = ...,
         limit: int = ...
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Lists the specified export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_export_tasks)
         """
+
     async def describe_log_groups(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         nextToken: str = ...,
@@ -313,14 +339,15 @@
     ) -> DescribeLogGroupsResponseTypeDef:
         """
         Lists the specified log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_groups)
         """
+
     async def describe_log_streams(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
@@ -330,14 +357,15 @@
     ) -> DescribeLogStreamsResponseTypeDef:
         """
         Lists the log streams for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_streams)
         """
+
     async def describe_metric_filters(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...,
@@ -346,14 +374,15 @@
     ) -> DescribeMetricFiltersResponseTypeDef:
         """
         Lists the specified metric filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_metric_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_metric_filters)
         """
+
     async def describe_queries(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -361,54 +390,62 @@
         """
         Returns a list of CloudWatch Logs Insights queries that are scheduled, running,
         or have been run recently in this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_queries)
         """
+
     async def describe_query_definitions(
         self, *, queryDefinitionNamePrefix: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeQueryDefinitionsResponseTypeDef:
         """
         This operation returns a paginated list of your saved CloudWatch Logs Insights
         query definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_query_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_query_definitions)
         """
+
     async def describe_resource_policies(
         self, *, nextToken: str = ..., limit: int = ...
     ) -> DescribeResourcePoliciesResponseTypeDef:
         """
         Lists the resource policies in this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_resource_policies)
         """
+
     async def describe_subscription_filters(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...
     ) -> DescribeSubscriptionFiltersResponseTypeDef:
         """
         Lists the subscription filters for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_subscription_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_subscription_filters)
         """
-    async def disassociate_kms_key(self, *, logGroupName: str) -> EmptyResponseMetadataTypeDef:
+
+    async def disassociate_kms_key(
+        self, *, logGroupName: str = ..., resourceIdentifier: str = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
-        Disassociates the associated KMS key from the specified log group.
+        Disassociates the specified KMS key from the specified log group or from all
+        CloudWatch Logs Insights query results in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.disassociate_kms_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#disassociate_kms_key)
         """
+
     async def filter_log_events(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
@@ -422,36 +459,39 @@
     ) -> FilterLogEventsResponseTypeDef:
         """
         Lists log events from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.filter_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#filter_log_events)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#generate_presigned_url)
         """
+
     async def get_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> GetDataProtectionPolicyResponseTypeDef:
         """
         Returns information about a log group data protection policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_data_protection_policy)
         """
+
     async def get_log_events(
         self,
         *,
         logStreamName: str,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         startTime: int = ...,
@@ -463,56 +503,62 @@
     ) -> GetLogEventsResponseTypeDef:
         """
         Lists log events from the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_events)
         """
+
     async def get_log_group_fields(
         self, *, logGroupName: str = ..., time: int = ..., logGroupIdentifier: str = ...
     ) -> GetLogGroupFieldsResponseTypeDef:
         """
         Returns a list of the fields that are included in log events in the specified
         log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_group_fields)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_group_fields)
         """
+
     async def get_log_record(
         self, *, logRecordPointer: str, unmask: bool = ...
     ) -> GetLogRecordResponseTypeDef:
         """
         Retrieves all of the fields and values of a single log event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_record)
         """
+
     async def get_query_results(self, *, queryId: str) -> GetQueryResultsResponseTypeDef:
         """
         Returns the results from the specified query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_query_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_query_results)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with a CloudWatch Logs resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_tags_for_resource)
         """
+
     async def list_tags_log_group(self, *, logGroupName: str) -> ListTagsLogGroupResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_tags_log_group)
         """
+
     async def put_account_policy(
         self,
         *,
         policyName: str,
         policyDocument: str,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         scope: Literal["ALL"] = ...
@@ -520,103 +566,112 @@
         """
         Creates an account-level data protection policy that applies to all log groups
         in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_account_policy)
         """
+
     async def put_data_protection_policy(
         self, *, logGroupIdentifier: str, policyDocument: str
     ) -> PutDataProtectionPolicyResponseTypeDef:
         """
         Creates a data protection policy for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_data_protection_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_data_protection_policy)
         """
+
     async def put_destination(
         self, *, destinationName: str, targetArn: str, roleArn: str, tags: Mapping[str, str] = ...
     ) -> PutDestinationResponseTypeDef:
         """
         Creates or updates a destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_destination)
         """
+
     async def put_destination_policy(
         self, *, destinationName: str, accessPolicy: str, forceUpdate: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an access policy associated with an existing destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_destination_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_destination_policy)
         """
+
     async def put_log_events(
         self,
         *,
         logGroupName: str,
         logStreamName: str,
         logEvents: Sequence[InputLogEventTypeDef],
         sequenceToken: str = ...
     ) -> PutLogEventsResponseTypeDef:
         """
         Uploads a batch of log events to the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_log_events)
         """
+
     async def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationUnionTypeDef]
+        metricTransformations: Sequence[MetricTransformationTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_metric_filter)
         """
+
     async def put_query_definition(
         self,
         *,
         name: str,
         queryString: str,
         queryDefinitionId: str = ...,
         logGroupNames: Sequence[str] = ...
     ) -> PutQueryDefinitionResponseTypeDef:
         """
         Creates or updates a query definition for CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_query_definition)
         """
+
     async def put_resource_policy(
         self, *, policyName: str = ..., policyDocument: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a resource policy allowing other Amazon Web Services services
         to put log events to this account, such as Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_resource_policy)
         """
+
     async def put_retention_policy(
         self, *, logGroupName: str, retentionInDays: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the retention of the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_retention_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_retention_policy)
         """
+
     async def put_subscription_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
         destinationArn: str,
@@ -626,14 +681,15 @@
         """
         Creates or updates a subscription filter and associates it with the specified
         log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_subscription_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_subscription_filter)
         """
+
     async def start_query(
         self,
         *,
         startTime: int,
         endTime: int,
         queryString: str,
         logGroupName: str = ...,
@@ -643,143 +699,160 @@
     ) -> StartQueryResponseTypeDef:
         """
         Schedules a query of a log group using CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_query)
         """
+
     async def stop_query(self, *, queryId: str) -> StopQueryResponseTypeDef:
         """
         Stops a CloudWatch Logs Insights query that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.stop_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#stop_query)
         """
+
     async def tag_log_group(
         self, *, logGroupName: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#tag_log_group)
         """
+
     async def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Assigns one or more tags (key-value pairs) to the specified CloudWatch Logs
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#tag_resource)
         """
+
     async def test_metric_filter(
         self, *, filterPattern: str, logEventMessages: Sequence[str]
     ) -> TestMetricFilterResponseTypeDef:
         """
         Tests the filter pattern of a metric filter against a sample of log event
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.test_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#test_metric_filter)
         """
+
     async def untag_log_group(
         self, *, logGroupName: str, tags: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#untag_log_group)
         """
+
     async def untag_resource(
         self, *, resourceArn: str, tagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes one or more tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#untag_resource)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_destinations"]
     ) -> DescribeDestinationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_export_tasks"]
     ) -> DescribeExportTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_log_groups"]
     ) -> DescribeLogGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_log_streams"]
     ) -> DescribeLogStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_metric_filters"]
     ) -> DescribeMetricFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_queries"]
     ) -> DescribeQueriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_resource_policies"]
     ) -> DescribeResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_subscription_filters"]
     ) -> DescribeSubscriptionFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["filter_log_events"]
     ) -> FilterLogEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "CloudWatchLogsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/)
         """
```

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/literals.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataProtectionStatusType",
     "DescribeDestinationsPaginatorName",
     "DescribeExportTasksPaginatorName",
     "DescribeLogGroupsPaginatorName",
     "DescribeLogStreamsPaginatorName",
     "DescribeMetricFiltersPaginatorName",
@@ -41,15 +40,14 @@
     "CloudWatchLogsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DataProtectionStatusType = Literal["ACTIVATED", "ARCHIVED", "DELETED", "DISABLED"]
 DescribeDestinationsPaginatorName = Literal["describe_destinations"]
 DescribeExportTasksPaginatorName = Literal["describe_export_tasks"]
 DescribeLogGroupsPaginatorName = Literal["describe_log_groups"]
 DescribeLogStreamsPaginatorName = Literal["describe_log_streams"]
 DescribeMetricFiltersPaginatorName = Literal["describe_metric_filters"]
 DescribeQueriesPaginatorName = Literal["describe_queries"]
@@ -108,14 +106,15 @@
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
@@ -211,14 +210,15 @@
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
@@ -297,26 +297,28 @@
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
@@ -488,14 +490,15 @@
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

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/literals.pyi` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataProtectionStatusType",
     "DescribeDestinationsPaginatorName",
     "DescribeExportTasksPaginatorName",
     "DescribeLogGroupsPaginatorName",
     "DescribeLogStreamsPaginatorName",
     "DescribeMetricFiltersPaginatorName",
@@ -40,14 +41,15 @@
     "CloudWatchLogsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DataProtectionStatusType = Literal["ACTIVATED", "ARCHIVED", "DELETED", "DISABLED"]
 DescribeDestinationsPaginatorName = Literal["describe_destinations"]
 DescribeExportTasksPaginatorName = Literal["describe_export_tasks"]
 DescribeLogGroupsPaginatorName = Literal["describe_log_groups"]
 DescribeLogStreamsPaginatorName = Literal["describe_log_streams"]
 DescribeMetricFiltersPaginatorName = Literal["describe_metric_filters"]
 DescribeQueriesPaginatorName = Literal["describe_queries"]
@@ -106,14 +108,15 @@
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
@@ -209,14 +212,15 @@
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
@@ -295,26 +299,28 @@
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
@@ -486,14 +492,15 @@
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

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/paginator.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/paginator.pyi` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/type_defs.py` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_logs.type_defs import AccountPolicyTypeDef
 
     data: AccountPolicyTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataProtectionStatusType,
     DistributionType,
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
@@ -84,15 +84,14 @@
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
     "MetricFilterMatchRecordTypeDef",
-    "MetricTransformationOutputTypeDef",
     "MetricTransformationTypeDef",
     "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
@@ -141,19 +140,18 @@
     "FilterLogEventsResponseTypeDef",
     "GetLogEventsResponseTypeDef",
     "GetLogGroupFieldsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "PutLogEventsRequestRequestTypeDef",
     "TestMetricFilterResponseTypeDef",
     "MetricFilterTypeDef",
-    "MetricTransformationUnionTypeDef",
+    "PutMetricFilterRequestRequestTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
-    "PutMetricFilterRequestRequestTypeDef",
 )
 
 AccountPolicyTypeDef = TypedDict(
     "AccountPolicyTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
@@ -161,21 +159,35 @@
         "policyType": Literal["DATA_PROTECTION_POLICY"],
         "scope": Literal["ALL"],
         "accountId": str,
     },
     total=False,
 )
 
-AssociateKmsKeyRequestRequestTypeDef = TypedDict(
-    "AssociateKmsKeyRequestRequestTypeDef",
+_RequiredAssociateKmsKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateKmsKeyRequestRequestTypeDef",
     {
-        "logGroupName": str,
         "kmsKeyId": str,
     },
 )
+_OptionalAssociateKmsKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateKmsKeyRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "resourceIdentifier": str,
+    },
+    total=False,
+)
+
+
+class AssociateKmsKeyRequestRequestTypeDef(
+    _RequiredAssociateKmsKeyRequestRequestTypeDef, _OptionalAssociateKmsKeyRequestRequestTypeDef
+):
+    pass
+
 
 CancelExportTaskRequestRequestTypeDef = TypedDict(
     "CancelExportTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
@@ -562,15 +574,17 @@
     total=False,
 )
 
 DisassociateKmsKeyRequestRequestTypeDef = TypedDict(
     "DisassociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
+        "resourceIdentifier": str,
     },
+    total=False,
 )
 
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
@@ -765,52 +779,27 @@
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredMetricTransformationOutputTypeDef = TypedDict(
-    "_RequiredMetricTransformationOutputTypeDef",
-    {
-        "metricName": str,
-        "metricNamespace": str,
-        "metricValue": str,
-    },
-)
-_OptionalMetricTransformationOutputTypeDef = TypedDict(
-    "_OptionalMetricTransformationOutputTypeDef",
-    {
-        "defaultValue": float,
-        "dimensions": Dict[str, str],
-        "unit": StandardUnitType,
-    },
-    total=False,
-)
-
-
-class MetricTransformationOutputTypeDef(
-    _RequiredMetricTransformationOutputTypeDef, _OptionalMetricTransformationOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricTransformationTypeDef = TypedDict(
     "_RequiredMetricTransformationTypeDef",
     {
         "metricName": str,
         "metricNamespace": str,
         "metricValue": str,
     },
 )
 _OptionalMetricTransformationTypeDef = TypedDict(
     "_OptionalMetricTransformationTypeDef",
     {
         "defaultValue": float,
-        "dimensions": Mapping[str, str],
+        "dimensions": Dict[str, str],
         "unit": StandardUnitType,
     },
     total=False,
 )
 
 
 class MetricTransformationTypeDef(
@@ -1392,14 +1381,15 @@
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
+        "encryptionKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
@@ -1432,24 +1422,31 @@
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": List[MetricTransformationOutputTypeDef],
+        "metricTransformations": List[MetricTransformationTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
-MetricTransformationUnionTypeDef = Union[
-    MetricTransformationTypeDef, MetricTransformationOutputTypeDef
-]
+PutMetricFilterRequestRequestTypeDef = TypedDict(
+    "PutMetricFilterRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "filterName": str,
+        "filterPattern": str,
+        "metricTransformations": Sequence[MetricTransformationTypeDef],
+    },
+)
+
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1468,17 +1465,7 @@
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-PutMetricFilterRequestRequestTypeDef = TypedDict(
-    "PutMetricFilterRequestRequestTypeDef",
-    {
-        "logGroupName": str,
-        "filterName": str,
-        "filterPattern": str,
-        "metricTransformations": Sequence[MetricTransformationUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs/type_defs.pyi` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_logs.type_defs import AccountPolicyTypeDef
 
     data: AccountPolicyTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataProtectionStatusType,
     DistributionType,
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
@@ -83,15 +83,14 @@
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
     "MetricFilterMatchRecordTypeDef",
-    "MetricTransformationOutputTypeDef",
     "MetricTransformationTypeDef",
     "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
@@ -140,19 +139,18 @@
     "FilterLogEventsResponseTypeDef",
     "GetLogEventsResponseTypeDef",
     "GetLogGroupFieldsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "PutLogEventsRequestRequestTypeDef",
     "TestMetricFilterResponseTypeDef",
     "MetricFilterTypeDef",
-    "MetricTransformationUnionTypeDef",
+    "PutMetricFilterRequestRequestTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
-    "PutMetricFilterRequestRequestTypeDef",
 )
 
 AccountPolicyTypeDef = TypedDict(
     "AccountPolicyTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
@@ -160,21 +158,33 @@
         "policyType": Literal["DATA_PROTECTION_POLICY"],
         "scope": Literal["ALL"],
         "accountId": str,
     },
     total=False,
 )
 
-AssociateKmsKeyRequestRequestTypeDef = TypedDict(
-    "AssociateKmsKeyRequestRequestTypeDef",
+_RequiredAssociateKmsKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateKmsKeyRequestRequestTypeDef",
     {
-        "logGroupName": str,
         "kmsKeyId": str,
     },
 )
+_OptionalAssociateKmsKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateKmsKeyRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "resourceIdentifier": str,
+    },
+    total=False,
+)
+
+class AssociateKmsKeyRequestRequestTypeDef(
+    _RequiredAssociateKmsKeyRequestRequestTypeDef, _OptionalAssociateKmsKeyRequestRequestTypeDef
+):
+    pass
 
 CancelExportTaskRequestRequestTypeDef = TypedDict(
     "CancelExportTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
@@ -553,15 +563,17 @@
     total=False,
 )
 
 DisassociateKmsKeyRequestRequestTypeDef = TypedDict(
     "DisassociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
+        "resourceIdentifier": str,
     },
+    total=False,
 )
 
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
@@ -752,50 +764,27 @@
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredMetricTransformationOutputTypeDef = TypedDict(
-    "_RequiredMetricTransformationOutputTypeDef",
-    {
-        "metricName": str,
-        "metricNamespace": str,
-        "metricValue": str,
-    },
-)
-_OptionalMetricTransformationOutputTypeDef = TypedDict(
-    "_OptionalMetricTransformationOutputTypeDef",
-    {
-        "defaultValue": float,
-        "dimensions": Dict[str, str],
-        "unit": StandardUnitType,
-    },
-    total=False,
-)
-
-class MetricTransformationOutputTypeDef(
-    _RequiredMetricTransformationOutputTypeDef, _OptionalMetricTransformationOutputTypeDef
-):
-    pass
-
 _RequiredMetricTransformationTypeDef = TypedDict(
     "_RequiredMetricTransformationTypeDef",
     {
         "metricName": str,
         "metricNamespace": str,
         "metricValue": str,
     },
 )
 _OptionalMetricTransformationTypeDef = TypedDict(
     "_OptionalMetricTransformationTypeDef",
     {
         "defaultValue": float,
-        "dimensions": Mapping[str, str],
+        "dimensions": Dict[str, str],
         "unit": StandardUnitType,
     },
     total=False,
 )
 
 class MetricTransformationTypeDef(
     _RequiredMetricTransformationTypeDef, _OptionalMetricTransformationTypeDef
@@ -1361,14 +1350,15 @@
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
+        "encryptionKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
@@ -1399,24 +1389,31 @@
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
         "filterPattern": str,
-        "metricTransformations": List[MetricTransformationOutputTypeDef],
+        "metricTransformations": List[MetricTransformationTypeDef],
         "creationTime": int,
         "logGroupName": str,
     },
     total=False,
 )
 
-MetricTransformationUnionTypeDef = Union[
-    MetricTransformationTypeDef, MetricTransformationOutputTypeDef
-]
+PutMetricFilterRequestRequestTypeDef = TypedDict(
+    "PutMetricFilterRequestRequestTypeDef",
+    {
+        "logGroupName": str,
+        "filterName": str,
+        "filterPattern": str,
+        "metricTransformations": Sequence[MetricTransformationTypeDef],
+    },
+)
+
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1435,17 +1432,7 @@
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-PutMetricFilterRequestRequestTypeDef = TypedDict(
-    "PutMetricFilterRequestRequestTypeDef",
-    {
-        "logGroupName": str,
-        "filterName": str,
-        "filterPattern": str,
-        "metricTransformations": Sequence[MetricTransformationUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-logs-2.5.2.post1/types_aiobotocore_logs.egg-info/SOURCES.txt` & `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

