# Comparing `tmp/types-aiobotocore-s3control-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-s3control-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3control-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3control-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-s3control-2.5.2.post1.tar` & `types-aiobotocore-s3control-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.989472 types-aiobotocore-s3control-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-08-02 14:52:55.989472 types-aiobotocore-s3control-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.989472 types-aiobotocore-s3control-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.985472 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45798 2023-08-02 14:48:28.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-08-02 14:48:28.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-08-02 14:48:28.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-02 14:48:28.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 14:48:28.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86389 2023-08-02 14:48:29.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86290 2023-08-02 14:48:29.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:27.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.989472 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:55.000000 types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13149 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11623 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      773 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      772 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    45691 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    45617 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13714 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13712 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2229 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2226 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    70218 2023-08-04 13:51:44.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    70141 2023-08-04 13:51:43.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13149 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/LICENSE` & `types-aiobotocore-s3control-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post1/setup.py` & `types-aiobotocore-s3control-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3control",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.S3Control 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__init__.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__init__.pyi` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/__main__.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3Control 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.S3Control 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/client.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointInputUnionTypeDef,
+    CreateMultiRegionAccessPointInputTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
@@ -52,58 +52,55 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    JobManifestGeneratorUnionTypeDef,
-    JobManifestUnionTypeDef,
-    JobOperationUnionTypeDef,
+    JobManifestGeneratorTypeDef,
+    JobManifestTypeDef,
+    JobOperationTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
-    ObjectLambdaConfigurationUnionTypeDef,
+    ObjectLambdaConfigurationTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    ReplicationConfigurationTypeDef,
     S3TagTypeDef,
-    StorageLensConfigurationUnionTypeDef,
+    StorageLensConfigurationTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("S3ControlClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     BucketAlreadyExists: Type[BotocoreClientError]
     BucketAlreadyOwnedByYou: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IdempotencyException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
@@ -111,15 +108,14 @@
     InvalidRequestException: Type[BotocoreClientError]
     JobStatusException: Type[BotocoreClientError]
     NoSuchPublicAccessBlockConfiguration: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class S3ControlClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
     """
 
     meta: ClientMeta
@@ -128,31 +124,28 @@
     def exceptions(self) -> Exceptions:
         """
         S3ControlClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#close)
         """
-
     async def create_access_point(
         self,
         *,
         AccountId: str,
         Name: str,
         Bucket: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
@@ -161,25 +154,23 @@
     ) -> CreateAccessPointResultTypeDef:
         """
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point)
         """
-
     async def create_access_point_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point_for_object_lambda)
         """
-
     async def create_bucket(
         self,
         *,
         Bucket: str,
         ACL: BucketCannedACLType = ...,
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
@@ -192,453 +183,406 @@
     ) -> CreateBucketResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_bucket)
         """
-
     async def create_job(
         self,
         *,
         AccountId: str,
-        Operation: JobOperationUnionTypeDef,
+        Operation: JobOperationTypeDef,
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: JobManifestUnionTypeDef = ...,
+        Manifest: JobManifestTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorUnionTypeDef = ...
+        ManifestGenerator: JobManifestGeneratorTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_job)
         """
-
     async def create_multi_region_access_point(
-        self,
-        *,
-        AccountId: str,
-        ClientToken: str,
-        Details: CreateMultiRegionAccessPointInputUnionTypeDef
+        self, *, AccountId: str, ClientToken: str, Details: CreateMultiRegionAccessPointInputTypeDef
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_multi_region_access_point)
         """
-
     async def delete_access_point(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point)
         """
-
     async def delete_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_for_object_lambda)
         """
-
     async def delete_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the access point policy for the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_policy)
         """
-
     async def delete_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_policy_for_object_lambda)
         """
-
     async def delete_bucket(self, *, AccountId: str, Bucket: str) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket)
         """
-
     async def delete_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_lifecycle_configuration)
         """
-
     async def delete_bucket_policy(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_policy)
         """
-
     async def delete_bucket_replication(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_replication)
         """
-
     async def delete_bucket_tagging(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_tagging)
         """
-
     async def delete_job_tagging(self, *, AccountId: str, JobId: str) -> Dict[str, Any]:
         """
         Removes the entire tag set from the specified S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_job_tagging)
         """
-
     async def delete_multi_region_access_point(
         self, *, AccountId: str, ClientToken: str, Details: DeleteMultiRegionAccessPointInputTypeDef
     ) -> DeleteMultiRegionAccessPointResultTypeDef:
         """
         Deletes a Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_multi_region_access_point)
         """
-
     async def delete_public_access_block(self, *, AccountId: str) -> EmptyResponseMetadataTypeDef:
         """
         Removes the `PublicAccessBlock` configuration for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_public_access_block)
         """
-
     async def delete_storage_lens_configuration(
         self, *, ConfigId: str, AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_storage_lens_configuration)
         """
-
     async def delete_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon S3 Storage Lens configuration tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_storage_lens_configuration_tagging)
         """
-
     async def describe_job(self, *, AccountId: str, JobId: str) -> DescribeJobResultTypeDef:
         """
         Retrieves the configuration parameters and status for a Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#describe_job)
         """
-
     async def describe_multi_region_access_point_operation(
         self, *, AccountId: str, RequestTokenARN: str
     ) -> DescribeMultiRegionAccessPointOperationResultTypeDef:
         """
         Retrieves the status of an asynchronous request to manage a Multi-Region Access
         Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_multi_region_access_point_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#describe_multi_region_access_point_operation)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#generate_presigned_url)
         """
-
     async def get_access_point(self, *, AccountId: str, Name: str) -> GetAccessPointResultTypeDef:
         """
         Returns configuration information about the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point)
         """
-
     async def get_access_point_configuration_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointConfigurationForObjectLambdaResultTypeDef:
         """
         Returns configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_configuration_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_configuration_for_object_lambda)
         """
-
     async def get_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointForObjectLambdaResultTypeDef:
         """
         Returns configuration information about the specified Object Lambda Access Point
         The following actions are related to `GetAccessPointForObjectLambda`: *
         `CreateAccessPointForObjectLambda
         <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.html>...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_for_object_lambda)
         """
-
     async def get_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyResultTypeDef:
         """
         Returns the access point policy associated with the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy)
         """
-
     async def get_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyForObjectLambdaResultTypeDef:
         """
         Returns the resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_for_object_lambda)
         """
-
     async def get_access_point_policy_status(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyStatusResultTypeDef:
         """
         Indicates whether the specified access point currently has a policy that allows
         public access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_status)
         """
-
     async def get_access_point_policy_status_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyStatusForObjectLambdaResultTypeDef:
         """
         Returns the status of the resource policy associated with an Object Lambda
         Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_status_for_object_lambda)
         """
-
     async def get_bucket(self, *, AccountId: str, Bucket: str) -> GetBucketResultTypeDef:
         """
         Gets an Amazon S3 on Outposts bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket)
         """
-
     async def get_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketLifecycleConfigurationResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_lifecycle_configuration)
         """
-
     async def get_bucket_policy(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketPolicyResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_policy)
         """
-
     async def get_bucket_replication(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketReplicationResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_replication)
         """
-
     async def get_bucket_tagging(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketTaggingResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_tagging)
         """
-
     async def get_bucket_versioning(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketVersioningResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_versioning)
         """
-
     async def get_job_tagging(self, *, AccountId: str, JobId: str) -> GetJobTaggingResultTypeDef:
         """
         Returns the tags on an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_job_tagging)
         """
-
     async def get_multi_region_access_point(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointResultTypeDef:
         """
         Returns configuration information about the specified Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point)
         """
-
     async def get_multi_region_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointPolicyResultTypeDef:
         """
         Returns the access control policy of the specified Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_policy)
         """
-
     async def get_multi_region_access_point_policy_status(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointPolicyStatusResultTypeDef:
         """
         Indicates whether the specified Multi-Region Access Point has an access control
         policy that allows public access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_policy_status)
         """
-
     async def get_multi_region_access_point_routes(
         self, *, AccountId: str, Mrap: str
     ) -> GetMultiRegionAccessPointRoutesResultTypeDef:
         """
         Returns the routing configuration for a Multi-Region Access Point, indicating
         which Regions are active or passive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_routes)
         """
-
     async def get_public_access_block(self, *, AccountId: str) -> GetPublicAccessBlockOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_public_access_block)
         """
-
     async def get_storage_lens_configuration(
         self, *, ConfigId: str, AccountId: str
     ) -> GetStorageLensConfigurationResultTypeDef:
         """
         Gets the Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_storage_lens_configuration)
         """
-
     async def get_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str
     ) -> GetStorageLensConfigurationTaggingResultTypeDef:
         """
         Gets the tags of Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_storage_lens_configuration_tagging)
         """
-
     async def list_access_points(
         self, *, AccountId: str, Bucket: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessPointsResultTypeDef:
         """
         Returns a list of the access points that are owned by the current account that's
         associated with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_points)
         """
-
     async def list_access_points_for_object_lambda(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessPointsForObjectLambdaResultTypeDef:
         """
         Returns some or all (up to 1,000) access points associated with the Object
         Lambda Access Point per call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_points_for_object_lambda)
         """
-
     async def list_jobs(
         self,
         *,
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -646,255 +590,233 @@
         """
         Lists current S3 Batch Operations jobs and jobs that have ended within the last
         30 days for the Amazon Web Services account making the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_jobs)
         """
-
     async def list_multi_region_access_points(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMultiRegionAccessPointsResultTypeDef:
         """
         Returns a list of the Multi-Region Access Points currently associated with the
         specified Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_multi_region_access_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_multi_region_access_points)
         """
-
     async def list_regional_buckets(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ..., OutpostId: str = ...
     ) -> ListRegionalBucketsResultTypeDef:
         """
         Returns a list of all Outposts buckets in an Outpost that are owned by the
         authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_regional_buckets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_regional_buckets)
         """
-
     async def list_storage_lens_configurations(
         self, *, AccountId: str, NextToken: str = ...
     ) -> ListStorageLensConfigurationsResultTypeDef:
         """
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_storage_lens_configurations)
         """
-
     async def put_access_point_configuration_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
-
     async def put_access_point_policy(
         self, *, AccountId: str, Name: str, Policy: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an access policy with the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_policy)
         """
-
     async def put_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str, Policy: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or replaces resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_policy_for_object_lambda)
         """
-
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         AccountId: str,
         Bucket: str,
         LifecycleConfiguration: LifecycleConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_lifecycle_configuration)
         """
-
     async def put_bucket_policy(
         self, *, AccountId: str, Bucket: str, Policy: str, ConfirmRemoveSelfBucketAccess: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_policy)
         """
-
     async def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef
+        ReplicationConfiguration: ReplicationConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_replication)
         """
-
     async def put_bucket_tagging(
         self, *, AccountId: str, Bucket: str, Tagging: TaggingTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_tagging)
         """
-
     async def put_bucket_versioning(
         self,
         *,
         AccountId: str,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         MFA: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_versioning)
         """
-
     async def put_job_tagging(
         self, *, AccountId: str, JobId: str, Tags: Sequence[S3TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the supplied tag-set on an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_job_tagging)
         """
-
     async def put_multi_region_access_point_policy(
         self,
         *,
         AccountId: str,
         ClientToken: str,
         Details: PutMultiRegionAccessPointPolicyInputTypeDef
     ) -> PutMultiRegionAccessPointPolicyResultTypeDef:
         """
         Associates an access control policy with the specified Multi-Region Access
         Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_multi_region_access_point_policy)
         """
-
     async def put_public_access_block(
         self,
         *,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
         AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or modifies the `PublicAccessBlock` configuration for an Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_public_access_block)
         """
-
     async def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: StorageLensConfigurationUnionTypeDef,
+        StorageLensConfiguration: StorageLensConfigurationTypeDef,
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration)
         """
-
     async def put_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str, Tags: Sequence[StorageLensTagTypeDef]
     ) -> Dict[str, Any]:
         """
         Put or replace tags on an existing Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration_tagging)
         """
-
     async def submit_multi_region_access_point_routes(
         self,
         *,
         AccountId: str,
         Mrap: str,
         RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef]
     ) -> Dict[str, Any]:
         """
         Submits an updated route configuration for a Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.submit_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#submit_multi_region_access_point_routes)
         """
-
     async def update_job_priority(
         self, *, AccountId: str, JobId: str, Priority: int
     ) -> UpdateJobPriorityResultTypeDef:
         """
         Updates an existing S3 Batch Operations job's priority.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_priority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_priority)
         """
-
     async def update_job_status(
         self,
         *,
         AccountId: str,
         JobId: str,
         RequestedJobStatus: RequestedJobStatusType,
         StatusUpdateReason: str = ...
     ) -> UpdateJobStatusResultTypeDef:
         """
         Updates the status for the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_status)
         """
-
     def get_paginator(
         self, operation_name: Literal["list_access_points_for_object_lambda"]
     ) -> ListAccessPointsForObjectLambdaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "S3ControlClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
         """
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/client.pyi` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointInputUnionTypeDef,
+    CreateMultiRegionAccessPointInputTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
@@ -52,55 +52,58 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    JobManifestGeneratorUnionTypeDef,
-    JobManifestUnionTypeDef,
-    JobOperationUnionTypeDef,
+    JobManifestGeneratorTypeDef,
+    JobManifestTypeDef,
+    JobOperationTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
-    ObjectLambdaConfigurationUnionTypeDef,
+    ObjectLambdaConfigurationTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    ReplicationConfigurationTypeDef,
     S3TagTypeDef,
-    StorageLensConfigurationUnionTypeDef,
+    StorageLensConfigurationTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("S3ControlClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     BucketAlreadyExists: Type[BotocoreClientError]
     BucketAlreadyOwnedByYou: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     IdempotencyException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
@@ -108,14 +111,15 @@
     InvalidRequestException: Type[BotocoreClientError]
     JobStatusException: Type[BotocoreClientError]
     NoSuchPublicAccessBlockConfiguration: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class S3ControlClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
     """
 
     meta: ClientMeta
@@ -124,28 +128,31 @@
     def exceptions(self) -> Exceptions:
         """
         S3ControlClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#close)
         """
+
     async def create_access_point(
         self,
         *,
         AccountId: str,
         Name: str,
         Bucket: str,
         VpcConfiguration: VpcConfigurationTypeDef = ...,
@@ -154,23 +161,25 @@
     ) -> CreateAccessPointResultTypeDef:
         """
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point)
         """
+
     async def create_access_point_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_access_point_for_object_lambda)
         """
+
     async def create_bucket(
         self,
         *,
         Bucket: str,
         ACL: BucketCannedACLType = ...,
         CreateBucketConfiguration: CreateBucketConfigurationTypeDef = ...,
         GrantFullControl: str = ...,
@@ -183,410 +192,449 @@
     ) -> CreateBucketResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_bucket)
         """
+
     async def create_job(
         self,
         *,
         AccountId: str,
-        Operation: JobOperationUnionTypeDef,
+        Operation: JobOperationTypeDef,
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: JobManifestUnionTypeDef = ...,
+        Manifest: JobManifestTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: JobManifestGeneratorUnionTypeDef = ...
+        ManifestGenerator: JobManifestGeneratorTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_job)
         """
+
     async def create_multi_region_access_point(
-        self,
-        *,
-        AccountId: str,
-        ClientToken: str,
-        Details: CreateMultiRegionAccessPointInputUnionTypeDef
+        self, *, AccountId: str, ClientToken: str, Details: CreateMultiRegionAccessPointInputTypeDef
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#create_multi_region_access_point)
         """
+
     async def delete_access_point(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point)
         """
+
     async def delete_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_for_object_lambda)
         """
+
     async def delete_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the access point policy for the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_policy)
         """
+
     async def delete_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_access_point_policy_for_object_lambda)
         """
+
     async def delete_bucket(self, *, AccountId: str, Bucket: str) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket)
         """
+
     async def delete_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_lifecycle_configuration)
         """
+
     async def delete_bucket_policy(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_policy)
         """
+
     async def delete_bucket_replication(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_replication)
         """
+
     async def delete_bucket_tagging(
         self, *, AccountId: str, Bucket: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_bucket_tagging)
         """
+
     async def delete_job_tagging(self, *, AccountId: str, JobId: str) -> Dict[str, Any]:
         """
         Removes the entire tag set from the specified S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_job_tagging)
         """
+
     async def delete_multi_region_access_point(
         self, *, AccountId: str, ClientToken: str, Details: DeleteMultiRegionAccessPointInputTypeDef
     ) -> DeleteMultiRegionAccessPointResultTypeDef:
         """
         Deletes a Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_multi_region_access_point)
         """
+
     async def delete_public_access_block(self, *, AccountId: str) -> EmptyResponseMetadataTypeDef:
         """
         Removes the `PublicAccessBlock` configuration for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_public_access_block)
         """
+
     async def delete_storage_lens_configuration(
         self, *, ConfigId: str, AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_storage_lens_configuration)
         """
+
     async def delete_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon S3 Storage Lens configuration tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.delete_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#delete_storage_lens_configuration_tagging)
         """
+
     async def describe_job(self, *, AccountId: str, JobId: str) -> DescribeJobResultTypeDef:
         """
         Retrieves the configuration parameters and status for a Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#describe_job)
         """
+
     async def describe_multi_region_access_point_operation(
         self, *, AccountId: str, RequestTokenARN: str
     ) -> DescribeMultiRegionAccessPointOperationResultTypeDef:
         """
         Retrieves the status of an asynchronous request to manage a Multi-Region Access
         Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.describe_multi_region_access_point_operation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#describe_multi_region_access_point_operation)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#generate_presigned_url)
         """
+
     async def get_access_point(self, *, AccountId: str, Name: str) -> GetAccessPointResultTypeDef:
         """
         Returns configuration information about the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point)
         """
+
     async def get_access_point_configuration_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointConfigurationForObjectLambdaResultTypeDef:
         """
         Returns configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_configuration_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_configuration_for_object_lambda)
         """
+
     async def get_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointForObjectLambdaResultTypeDef:
         """
         Returns configuration information about the specified Object Lambda Access Point
         The following actions are related to `GetAccessPointForObjectLambda`: *
         `CreateAccessPointForObjectLambda
         <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.html>...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_for_object_lambda)
         """
+
     async def get_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyResultTypeDef:
         """
         Returns the access point policy associated with the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy)
         """
+
     async def get_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyForObjectLambdaResultTypeDef:
         """
         Returns the resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_for_object_lambda)
         """
+
     async def get_access_point_policy_status(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyStatusResultTypeDef:
         """
         Indicates whether the specified access point currently has a policy that allows
         public access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_status)
         """
+
     async def get_access_point_policy_status_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyStatusForObjectLambdaResultTypeDef:
         """
         Returns the status of the resource policy associated with an Object Lambda
         Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_access_point_policy_status_for_object_lambda)
         """
+
     async def get_bucket(self, *, AccountId: str, Bucket: str) -> GetBucketResultTypeDef:
         """
         Gets an Amazon S3 on Outposts bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket)
         """
+
     async def get_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketLifecycleConfigurationResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_lifecycle_configuration)
         """
+
     async def get_bucket_policy(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketPolicyResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_policy)
         """
+
     async def get_bucket_replication(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketReplicationResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_replication)
         """
+
     async def get_bucket_tagging(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketTaggingResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_tagging)
         """
+
     async def get_bucket_versioning(
         self, *, AccountId: str, Bucket: str
     ) -> GetBucketVersioningResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_bucket_versioning)
         """
+
     async def get_job_tagging(self, *, AccountId: str, JobId: str) -> GetJobTaggingResultTypeDef:
         """
         Returns the tags on an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_job_tagging)
         """
+
     async def get_multi_region_access_point(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointResultTypeDef:
         """
         Returns configuration information about the specified Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point)
         """
+
     async def get_multi_region_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointPolicyResultTypeDef:
         """
         Returns the access control policy of the specified Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_policy)
         """
+
     async def get_multi_region_access_point_policy_status(
         self, *, AccountId: str, Name: str
     ) -> GetMultiRegionAccessPointPolicyStatusResultTypeDef:
         """
         Indicates whether the specified Multi-Region Access Point has an access control
         policy that allows public access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_policy_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_policy_status)
         """
+
     async def get_multi_region_access_point_routes(
         self, *, AccountId: str, Mrap: str
     ) -> GetMultiRegionAccessPointRoutesResultTypeDef:
         """
         Returns the routing configuration for a Multi-Region Access Point, indicating
         which Regions are active or passive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_multi_region_access_point_routes)
         """
+
     async def get_public_access_block(self, *, AccountId: str) -> GetPublicAccessBlockOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_public_access_block)
         """
+
     async def get_storage_lens_configuration(
         self, *, ConfigId: str, AccountId: str
     ) -> GetStorageLensConfigurationResultTypeDef:
         """
         Gets the Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_storage_lens_configuration)
         """
+
     async def get_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str
     ) -> GetStorageLensConfigurationTaggingResultTypeDef:
         """
         Gets the tags of Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_storage_lens_configuration_tagging)
         """
+
     async def list_access_points(
         self, *, AccountId: str, Bucket: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessPointsResultTypeDef:
         """
         Returns a list of the access points that are owned by the current account that's
         associated with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_points)
         """
+
     async def list_access_points_for_object_lambda(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessPointsForObjectLambdaResultTypeDef:
         """
         Returns some or all (up to 1,000) access points associated with the Object
         Lambda Access Point per call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_access_points_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_access_points_for_object_lambda)
         """
+
     async def list_jobs(
         self,
         *,
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -594,233 +642,255 @@
         """
         Lists current S3 Batch Operations jobs and jobs that have ended within the last
         30 days for the Amazon Web Services account making the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_jobs)
         """
+
     async def list_multi_region_access_points(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListMultiRegionAccessPointsResultTypeDef:
         """
         Returns a list of the Multi-Region Access Points currently associated with the
         specified Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_multi_region_access_points)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_multi_region_access_points)
         """
+
     async def list_regional_buckets(
         self, *, AccountId: str, NextToken: str = ..., MaxResults: int = ..., OutpostId: str = ...
     ) -> ListRegionalBucketsResultTypeDef:
         """
         Returns a list of all Outposts buckets in an Outpost that are owned by the
         authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_regional_buckets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_regional_buckets)
         """
+
     async def list_storage_lens_configurations(
         self, *, AccountId: str, NextToken: str = ...
     ) -> ListStorageLensConfigurationsResultTypeDef:
         """
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#list_storage_lens_configurations)
         """
+
     async def put_access_point_configuration_for_object_lambda(
-        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
+
     async def put_access_point_policy(
         self, *, AccountId: str, Name: str, Policy: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an access policy with the specified access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_policy)
         """
+
     async def put_access_point_policy_for_object_lambda(
         self, *, AccountId: str, Name: str, Policy: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or replaces resource policy for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_policy_for_object_lambda)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_access_point_policy_for_object_lambda)
         """
+
     async def put_bucket_lifecycle_configuration(
         self,
         *,
         AccountId: str,
         Bucket: str,
         LifecycleConfiguration: LifecycleConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_lifecycle_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_lifecycle_configuration)
         """
+
     async def put_bucket_policy(
         self, *, AccountId: str, Bucket: str, Policy: str, ConfirmRemoveSelfBucketAccess: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_policy)
         """
+
     async def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef
+        ReplicationConfiguration: ReplicationConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_replication)
         """
+
     async def put_bucket_tagging(
         self, *, AccountId: str, Bucket: str, Tagging: TaggingTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_tagging)
         """
+
     async def put_bucket_versioning(
         self,
         *,
         AccountId: str,
         Bucket: str,
         VersioningConfiguration: VersioningConfigurationTypeDef,
         MFA: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_versioning)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_bucket_versioning)
         """
+
     async def put_job_tagging(
         self, *, AccountId: str, JobId: str, Tags: Sequence[S3TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the supplied tag-set on an S3 Batch Operations job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_job_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_job_tagging)
         """
+
     async def put_multi_region_access_point_policy(
         self,
         *,
         AccountId: str,
         ClientToken: str,
         Details: PutMultiRegionAccessPointPolicyInputTypeDef
     ) -> PutMultiRegionAccessPointPolicyResultTypeDef:
         """
         Associates an access control policy with the specified Multi-Region Access
         Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_multi_region_access_point_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_multi_region_access_point_policy)
         """
+
     async def put_public_access_block(
         self,
         *,
         PublicAccessBlockConfiguration: PublicAccessBlockConfigurationTypeDef,
         AccountId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or modifies the `PublicAccessBlock` configuration for an Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_public_access_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_public_access_block)
         """
+
     async def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: StorageLensConfigurationUnionTypeDef,
+        StorageLensConfiguration: StorageLensConfigurationTypeDef,
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration)
         """
+
     async def put_storage_lens_configuration_tagging(
         self, *, ConfigId: str, AccountId: str, Tags: Sequence[StorageLensTagTypeDef]
     ) -> Dict[str, Any]:
         """
         Put or replace tags on an existing Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration_tagging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#put_storage_lens_configuration_tagging)
         """
+
     async def submit_multi_region_access_point_routes(
         self,
         *,
         AccountId: str,
         Mrap: str,
         RouteUpdates: Sequence[MultiRegionAccessPointRouteTypeDef]
     ) -> Dict[str, Any]:
         """
         Submits an updated route configuration for a Multi-Region Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.submit_multi_region_access_point_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#submit_multi_region_access_point_routes)
         """
+
     async def update_job_priority(
         self, *, AccountId: str, JobId: str, Priority: int
     ) -> UpdateJobPriorityResultTypeDef:
         """
         Updates an existing S3 Batch Operations job's priority.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_priority)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_priority)
         """
+
     async def update_job_status(
         self,
         *,
         AccountId: str,
         JobId: str,
         RequestedJobStatus: RequestedJobStatusType,
         StatusUpdateReason: str = ...
     ) -> UpdateJobStatusResultTypeDef:
         """
         Updates the status for the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.update_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#update_job_status)
         """
+
     def get_paginator(
         self, operation_name: Literal["list_access_points_for_object_lambda"]
     ) -> ListAccessPointsForObjectLambdaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "S3ControlClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/client/)
         """
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/literals.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,15 @@
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
@@ -312,14 +313,15 @@
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
@@ -398,26 +400,28 @@
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
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/literals.pyi` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,15 @@
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
@@ -310,14 +311,15 @@
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
@@ -396,26 +398,28 @@
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
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/paginator.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/paginator.pyi` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/type_defs.py` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "AccessControlTranslationTypeDef",
     "VpcConfigurationTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
@@ -102,15 +101,14 @@
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
-    "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
     "ExistingObjectReplicationTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
@@ -130,29 +128,26 @@
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     "StorageLensTagTypeDef",
-    "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
-    "JobManifestGeneratorFilterOutputTypeDef",
     "TimestampTypeDef",
     "JobManifestLocationTypeDef",
-    "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
-    "LifecycleExpirationOutputTypeDef",
+    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionOutputTypeDef",
+    "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
@@ -165,18 +160,16 @@
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "ReplicaModificationsTypeDef",
     "S3ObjectOwnerTypeDef",
-    "S3ObjectMetadataOutputTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
-    "S3RetentionOutputTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
@@ -202,131 +195,96 @@
     "GetAccessPointForObjectLambdaResultTypeDef",
     "GetAccessPointResultTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "GetBucketTaggingResultTypeDef",
     "GetJobTaggingResultTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
-    "S3SetObjectTaggingOperationOutputTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
-    "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
-    "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "JobManifestGeneratorFilterTypeDef",
-    "LifecycleExpirationTypeDef",
     "S3ObjectMetadataTypeDef",
     "S3RetentionTypeDef",
-    "TransitionTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
-    "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
-    "S3SetObjectRetentionOperationOutputTypeDef",
-    "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
-    "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
-    "CreateMultiRegionAccessPointInputUnionTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
-    "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
-    "JobManifestUnionTypeDef",
     "JobListDescriptorTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
     "PrefixLevelTypeDef",
-    "S3AccessControlListOutputTypeDef",
     "S3AccessControlListTypeDef",
-    "S3CopyObjectOperationOutputTypeDef",
     "S3CopyObjectOperationTypeDef",
-    "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
-    "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
-    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
-    "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
     "ListJobsResultTypeDef",
-    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
     "BucketLevelTypeDef",
-    "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
-    "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
-    "ObjectLambdaConfigurationUnionTypeDef",
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
-    "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     "AccountLevelTypeDef",
-    "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "JobManifestGeneratorUnionTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
-    "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
-    "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
-    "StorageLensConfigurationUnionTypeDef",
-    "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobOperationUnionTypeDef",
+    "JobDescriptorTypeDef",
     "DescribeJobResultTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -416,21 +374,19 @@
     "_OptionalAwsLambdaTransformationTypeDef",
     {
         "FunctionPayload": str,
     },
     total=False,
 )
 
-
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
-
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -486,19 +442,17 @@
         "Format": Literal["Report_CSV_20180820"],
         "Prefix": str,
         "ReportScope": JobReportScopeType,
     },
     total=False,
 )
 
-
 class JobReportTypeDef(_RequiredJobReportTypeDef, _OptionalJobReportTypeDef):
     pass
 
-
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -513,19 +467,17 @@
     "_OptionalRegionTypeDef",
     {
         "BucketAccountId": str,
     },
     total=False,
 )
 
-
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
-
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -660,28 +612,19 @@
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-ExcludeOutputTypeDef = TypedDict(
-    "ExcludeOutputTypeDef",
-    {
-        "Buckets": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
 ExcludeTypeDef = TypedDict(
     "ExcludeTypeDef",
     {
-        "Buckets": Sequence[str],
-        "Regions": Sequence[str],
+        "Buckets": List[str],
+        "Regions": List[str],
     },
     total=False,
 )
 
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
@@ -859,21 +802,19 @@
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
-
 class MultiRegionAccessPointRouteTypeDef(
     _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
 ):
     pass
 
-
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -897,52 +838,32 @@
     "StorageLensTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-IncludeOutputTypeDef = TypedDict(
-    "IncludeOutputTypeDef",
-    {
-        "Buckets": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
 IncludeTypeDef = TypedDict(
     "IncludeTypeDef",
     {
-        "Buckets": Sequence[str],
-        "Regions": Sequence[str],
+        "Buckets": List[str],
+        "Regions": List[str],
     },
     total=False,
 )
 
 JobFailureTypeDef = TypedDict(
     "JobFailureTypeDef",
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
-JobManifestGeneratorFilterOutputTypeDef = TypedDict(
-    "JobManifestGeneratorFilterOutputTypeDef",
-    {
-        "EligibleForReplication": bool,
-        "CreatedAfter": datetime,
-        "CreatedBefore": datetime,
-        "ObjectReplicationStatuses": List[ReplicationStatusType],
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
@@ -951,61 +872,36 @@
     "_OptionalJobManifestLocationTypeDef",
     {
         "ObjectVersionId": str,
     },
     total=False,
 )
 
-
 class JobManifestLocationTypeDef(
     _RequiredJobManifestLocationTypeDef, _OptionalJobManifestLocationTypeDef
 ):
     pass
 
-
-_RequiredJobManifestSpecOutputTypeDef = TypedDict(
-    "_RequiredJobManifestSpecOutputTypeDef",
-    {
-        "Format": JobManifestFormatType,
-    },
-)
-_OptionalJobManifestSpecOutputTypeDef = TypedDict(
-    "_OptionalJobManifestSpecOutputTypeDef",
-    {
-        "Fields": List[JobManifestFieldNameType],
-    },
-    total=False,
-)
-
-
-class JobManifestSpecOutputTypeDef(
-    _RequiredJobManifestSpecOutputTypeDef, _OptionalJobManifestSpecOutputTypeDef
-):
-    pass
-
-
 _RequiredJobManifestSpecTypeDef = TypedDict(
     "_RequiredJobManifestSpecTypeDef",
     {
         "Format": JobManifestFormatType,
     },
 )
 _OptionalJobManifestSpecTypeDef = TypedDict(
     "_OptionalJobManifestSpecTypeDef",
     {
         "Fields": Sequence[JobManifestFieldNameType],
     },
     total=False,
 )
 
-
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
-
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1023,16 +919,16 @@
     "JobTimersTypeDef",
     {
         "ElapsedTimeInActiveSeconds": int,
     },
     total=False,
 )
 
-LifecycleExpirationOutputTypeDef = TypedDict(
-    "LifecycleExpirationOutputTypeDef",
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
@@ -1051,16 +947,16 @@
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-TransitionOutputTypeDef = TypedDict(
-    "TransitionOutputTypeDef",
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
@@ -1086,22 +982,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAccessPointsForObjectLambdaRequestRequestTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1110,21 +1004,19 @@
         "Bucket": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAccessPointsRequestRequestTypeDef(
     _RequiredListAccessPointsRequestRequestTypeDef, _OptionalListAccessPointsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -1133,21 +1025,19 @@
         "JobStatuses": Sequence[JobStatusType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListMultiRegionAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiRegionAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListMultiRegionAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1155,22 +1045,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMultiRegionAccessPointsRequestRequestTypeDef(
     _RequiredListMultiRegionAccessPointsRequestRequestTypeDef,
     _OptionalListMultiRegionAccessPointsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListRegionalBucketsRequestRequestTypeDef = TypedDict(
     "_RequiredListRegionalBucketsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListRegionalBucketsRequestRequestTypeDef = TypedDict(
@@ -1179,22 +1067,20 @@
         "NextToken": str,
         "MaxResults": int,
         "OutpostId": str,
     },
     total=False,
 )
 
-
 class ListRegionalBucketsRequestRequestTypeDef(
     _RequiredListRegionalBucketsRequestRequestTypeDef,
     _OptionalListRegionalBucketsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRegionalBucketTypeDef = TypedDict(
     "_RequiredRegionalBucketTypeDef",
     {
         "Bucket": str,
         "PublicAccessBlockEnabled": bool,
         "CreationDate": datetime,
     },
@@ -1204,19 +1090,17 @@
     {
         "BucketArn": str,
         "OutpostId": str,
     },
     total=False,
 )
 
-
 class RegionalBucketTypeDef(_RequiredRegionalBucketTypeDef, _OptionalRegionalBucketTypeDef):
     pass
 
-
 _RequiredListStorageLensConfigurationEntryTypeDef = TypedDict(
     "_RequiredListStorageLensConfigurationEntryTypeDef",
     {
         "Id": str,
         "StorageLensArn": str,
         "HomeRegion": str,
     },
@@ -1225,44 +1109,40 @@
     "_OptionalListStorageLensConfigurationEntryTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
 
-
 class ListStorageLensConfigurationEntryTypeDef(
     _RequiredListStorageLensConfigurationEntryTypeDef,
     _OptionalListStorageLensConfigurationEntryTypeDef,
 ):
     pass
 
-
 _RequiredListStorageLensConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListStorageLensConfigurationsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListStorageLensConfigurationsRequestRequestTypeDef = TypedDict(
     "_OptionalListStorageLensConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1334,21 +1214,19 @@
     "_OptionalPutBucketPolicyRequestRequestTypeDef",
     {
         "ConfirmRemoveSelfBucketAccess": bool,
     },
     total=False,
 )
 
-
 class PutBucketPolicyRequestRequestTypeDef(
     _RequiredPutBucketPolicyRequestRequestTypeDef, _OptionalPutBucketPolicyRequestRequestTypeDef
 ):
     pass
 
-
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
@@ -1366,32 +1244,14 @@
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-S3ObjectMetadataOutputTypeDef = TypedDict(
-    "S3ObjectMetadataOutputTypeDef",
-    {
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "UserMetadata": Dict[str, str],
-        "ContentLength": int,
-        "ContentMD5": str,
-        "ContentType": str,
-        "HttpExpiresDate": datetime,
-        "RequesterCharged": bool,
-        "SSEAlgorithm": S3SSEAlgorithmType,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
@@ -1401,23 +1261,14 @@
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
-S3RetentionOutputTypeDef = TypedDict(
-    "S3RetentionOutputTypeDef",
-    {
-        "RetainUntilDate": datetime,
-        "Mode": S3ObjectLockRetentionModeType,
-    },
-    total=False,
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -1456,21 +1307,19 @@
     "_OptionalUpdateJobStatusRequestRequestTypeDef",
     {
         "StatusUpdateReason": str,
     },
     total=False,
 )
 
-
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
@@ -1482,19 +1331,17 @@
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
-
 DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": DeleteMultiRegionAccessPointInputTypeDef,
     },
@@ -1528,21 +1375,19 @@
     {
         "ObjectLambdaAccessPointArn": str,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
     },
     total=False,
 )
 
-
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
-
 CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointArn": str,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1681,21 +1526,19 @@
         "VpcConfiguration": VpcConfigurationTypeDef,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
-
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
@@ -1754,21 +1597,19 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "OutpostId": str,
     },
     total=False,
 )
 
-
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
-
 GetBucketTaggingResultTypeDef = TypedDict(
     "GetBucketTaggingResultTypeDef",
     {
         "TagSet": List[S3TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1777,30 +1618,19 @@
     "GetJobTaggingResultTypeDef",
     {
         "Tags": List[S3TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagTypeDef],
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[S3TagTypeDef],
+        "Tags": List[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 PutJobTaggingRequestRequestTypeDef = TypedDict(
@@ -1808,36 +1638,19 @@
     {
         "AccountId": str,
         "JobId": str,
         "Tags": Sequence[S3TagTypeDef],
     },
 )
 
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagTypeDef],
-    },
-    total=False,
-)
-
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[S3TagTypeDef],
-    },
-    total=False,
-)
-
-S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
-    "S3SetObjectTaggingOperationOutputTypeDef",
-    {
-        "TagSet": List[S3TagTypeDef],
+        "Tags": List[S3TagTypeDef],
     },
     total=False,
 )
 
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
@@ -1849,37 +1662,14 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
-_RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
-    {
-        "Name": str,
-        "Regions": List[RegionTypeDef],
-    },
-)
-_OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
-    {
-        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateMultiRegionAccessPointInputOutputTypeDef(
-    _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
-    _OptionalCreateMultiRegionAccessPointInputOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateMultiRegionAccessPointInputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
         "Regions": Sequence[RegionTypeDef],
     },
 )
@@ -1887,31 +1677,20 @@
     "_OptionalCreateMultiRegionAccessPointInputTypeDef",
     {
         "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
-
-GeneratedManifestEncryptionOutputTypeDef = TypedDict(
-    "GeneratedManifestEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSEncryptionTypeDef,
-    },
-    total=False,
-)
-
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSEncryptionTypeDef,
     },
     total=False,
@@ -1983,24 +1762,14 @@
         "CreatedAfter": TimestampTypeDef,
         "CreatedBefore": TimestampTypeDef,
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Days": int,
-        "ExpiredObjectDeleteMarker": bool,
-    },
-    total=False,
-)
-
 S3ObjectMetadataTypeDef = TypedDict(
     "S3ObjectMetadataTypeDef",
     {
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
         "ContentLanguage": str,
@@ -2020,41 +1789,23 @@
     {
         "RetainUntilDate": TimestampTypeDef,
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Days": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
         "Location": JobManifestLocationTypeDef,
     },
     total=False,
 )
 
-JobManifestOutputTypeDef = TypedDict(
-    "JobManifestOutputTypeDef",
-    {
-        "Spec": JobManifestSpecOutputTypeDef,
-        "Location": JobManifestLocationTypeDef,
-    },
-)
-
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
         "Location": JobManifestLocationTypeDef,
     },
 )
@@ -2080,22 +1831,20 @@
     "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
 ):
     pass
 
-
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2120,19 +1869,17 @@
     "_OptionalMetricsTypeDef",
     {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
     total=False,
 )
 
-
 class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
     pass
 
-
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
@@ -2188,22 +1935,20 @@
     "_OptionalPutBucketVersioningRequestRequestTypeDef",
     {
         "MFA": str,
     },
     total=False,
 )
 
-
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
@@ -2212,49 +1957,18 @@
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
-_RequiredS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
-    "_RequiredS3SetObjectRetentionOperationOutputTypeDef",
-    {
-        "Retention": S3RetentionOutputTypeDef,
-    },
-)
-_OptionalS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
-    "_OptionalS3SetObjectRetentionOperationOutputTypeDef",
-    {
-        "BypassGovernanceRetention": bool,
-    },
-    total=False,
-)
-
-
-class S3SetObjectRetentionOperationOutputTypeDef(
-    _RequiredS3SetObjectRetentionOperationOutputTypeDef,
-    _OptionalS3SetObjectRetentionOperationOutputTypeDef,
-):
-    pass
-
-
-StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
-    "StorageLensDataExportEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSTypeDef,
-    },
-    total=False,
-)
-
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
-        "SSES3": Mapping[str, Any],
+        "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
@@ -2270,22 +1984,14 @@
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
-    "ObjectLambdaTransformationConfigurationOutputTypeDef",
-    {
-        "Actions": List[ObjectLambdaTransformationConfigurationActionType],
-        "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
-    },
-)
-
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
         "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
@@ -2295,48 +2001,26 @@
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagTypeDef,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -2351,57 +2035,30 @@
         "Tagging": TaggingTypeDef,
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
-        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
+        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputTypeDef,
         "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
         "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
-CreateMultiRegionAccessPointInputUnionTypeDef = Union[
-    CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
-]
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
 )
 
-_RequiredS3ManifestOutputLocationOutputTypeDef = TypedDict(
-    "_RequiredS3ManifestOutputLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
-    },
-)
-_OptionalS3ManifestOutputLocationOutputTypeDef = TypedDict(
-    "_OptionalS3ManifestOutputLocationOutputTypeDef",
-    {
-        "ExpectedManifestBucketOwner": str,
-        "ManifestPrefix": str,
-        "ManifestEncryption": GeneratedManifestEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class S3ManifestOutputLocationOutputTypeDef(
-    _RequiredS3ManifestOutputLocationOutputTypeDef, _OptionalS3ManifestOutputLocationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ManifestOutputLocationTypeDef = TypedDict(
     "_RequiredS3ManifestOutputLocationTypeDef",
     {
         "Bucket": str,
         "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
     },
 )
@@ -2411,43 +2068,38 @@
         "ExpectedManifestBucketOwner": str,
         "ManifestPrefix": str,
         "ManifestEncryption": GeneratedManifestEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
-
 _RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_RequiredS3SetObjectRetentionOperationTypeDef",
     {
         "Retention": S3RetentionTypeDef,
     },
 )
 _OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_OptionalS3SetObjectRetentionOperationTypeDef",
     {
         "BypassGovernanceRetention": bool,
     },
     total=False,
 )
 
-
 class S3SetObjectRetentionOperationTypeDef(
     _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
 ):
     pass
 
-
-JobManifestUnionTypeDef = Union[JobManifestTypeDef, JobManifestOutputTypeDef]
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2474,19 +2126,17 @@
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Metrics": MetricsTypeDef,
         "StorageClass": ReplicationStorageClassType,
     },
     total=False,
 )
 
-
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2520,81 +2170,33 @@
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
-_RequiredS3AccessControlListOutputTypeDef = TypedDict(
-    "_RequiredS3AccessControlListOutputTypeDef",
-    {
-        "Owner": S3ObjectOwnerTypeDef,
-    },
-)
-_OptionalS3AccessControlListOutputTypeDef = TypedDict(
-    "_OptionalS3AccessControlListOutputTypeDef",
-    {
-        "Grants": List[S3GrantTypeDef],
-    },
-    total=False,
-)
-
-
-class S3AccessControlListOutputTypeDef(
-    _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
-):
-    pass
-
-
 _RequiredS3AccessControlListTypeDef = TypedDict(
     "_RequiredS3AccessControlListTypeDef",
     {
         "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListTypeDef = TypedDict(
     "_OptionalS3AccessControlListTypeDef",
     {
         "Grants": Sequence[S3GrantTypeDef],
     },
     total=False,
 )
 
-
 class S3AccessControlListTypeDef(
     _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
 ):
     pass
 
-
-S3CopyObjectOperationOutputTypeDef = TypedDict(
-    "S3CopyObjectOperationOutputTypeDef",
-    {
-        "TargetResource": str,
-        "CannedAccessControlList": S3CannedAccessControlListType,
-        "AccessControlGrants": List[S3GrantTypeDef],
-        "MetadataDirective": S3MetadataDirectiveType,
-        "ModifiedSinceConstraint": datetime,
-        "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
-        "NewObjectTagging": List[S3TagTypeDef],
-        "RedirectLocation": str,
-        "RequesterPays": bool,
-        "StorageClass": S3StorageClassType,
-        "UnModifiedSinceConstraint": datetime,
-        "SSEAwsKmsKeyId": str,
-        "TargetKeyPrefix": str,
-        "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
-        "ObjectLockMode": S3ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "BucketKeyEnabled": bool,
-        "ChecksumAlgorithm": S3ChecksumAlgorithmType,
-    },
-    total=False,
-)
-
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
@@ -2612,39 +2214,14 @@
         "ObjectLockRetainUntilDate": TimestampTypeDef,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
-_RequiredS3BucketDestinationOutputTypeDef = TypedDict(
-    "_RequiredS3BucketDestinationOutputTypeDef",
-    {
-        "Format": FormatType,
-        "OutputSchemaVersion": Literal["V_1"],
-        "AccountId": str,
-        "Arn": str,
-    },
-)
-_OptionalS3BucketDestinationOutputTypeDef = TypedDict(
-    "_OptionalS3BucketDestinationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Encryption": StorageLensDataExportEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class S3BucketDestinationOutputTypeDef(
-    _RequiredS3BucketDestinationOutputTypeDef, _OptionalS3BucketDestinationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3BucketDestinationTypeDef = TypedDict(
     "_RequiredS3BucketDestinationTypeDef",
     {
         "Format": FormatType,
         "OutputSchemaVersion": Literal["V_1"],
         "AccountId": str,
         "Arn": str,
@@ -2655,44 +2232,19 @@
     {
         "Prefix": str,
         "Encryption": StorageLensDataExportEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class S3BucketDestinationTypeDef(
     _RequiredS3BucketDestinationTypeDef, _OptionalS3BucketDestinationTypeDef
 ):
     pass
 
-
-_RequiredObjectLambdaConfigurationOutputTypeDef = TypedDict(
-    "_RequiredObjectLambdaConfigurationOutputTypeDef",
-    {
-        "SupportingAccessPoint": str,
-        "TransformationConfigurations": List[ObjectLambdaTransformationConfigurationOutputTypeDef],
-    },
-)
-_OptionalObjectLambdaConfigurationOutputTypeDef = TypedDict(
-    "_OptionalObjectLambdaConfigurationOutputTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "AllowedFeatures": List[ObjectLambdaAllowedFeatureType],
-    },
-    total=False,
-)
-
-
-class ObjectLambdaConfigurationOutputTypeDef(
-    _RequiredObjectLambdaConfigurationOutputTypeDef, _OptionalObjectLambdaConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredObjectLambdaConfigurationTypeDef = TypedDict(
     "_RequiredObjectLambdaConfigurationTypeDef",
     {
         "SupportingAccessPoint": str,
         "TransformationConfigurations": Sequence[ObjectLambdaTransformationConfigurationTypeDef],
     },
 )
@@ -2701,97 +2253,42 @@
     {
         "CloudWatchMetricsEnabled": bool,
         "AllowedFeatures": Sequence[ObjectLambdaAllowedFeatureType],
     },
     total=False,
 )
 
-
 class ObjectLambdaConfigurationTypeDef(
     _RequiredObjectLambdaConfigurationTypeDef, _OptionalObjectLambdaConfigurationTypeDef
 ):
     pass
 
-
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
-    {
-        "Expiration": LifecycleExpirationOutputTypeDef,
-        "ID": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
-        "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
-        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
-    },
-    total=False,
-)
-
-
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Transitions": Sequence[TransitionTypeDef],
-        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
+        "Transitions": List[TransitionTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
-
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
-
-_RequiredS3JobManifestGeneratorOutputTypeDef = TypedDict(
-    "_RequiredS3JobManifestGeneratorOutputTypeDef",
-    {
-        "SourceBucket": str,
-        "EnableManifestOutput": bool,
-    },
-)
-_OptionalS3JobManifestGeneratorOutputTypeDef = TypedDict(
-    "_OptionalS3JobManifestGeneratorOutputTypeDef",
-    {
-        "ExpectedBucketOwner": str,
-        "ManifestOutputLocation": S3ManifestOutputLocationOutputTypeDef,
-        "Filter": JobManifestGeneratorFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class S3JobManifestGeneratorOutputTypeDef(
-    _RequiredS3JobManifestGeneratorOutputTypeDef, _OptionalS3JobManifestGeneratorOutputTypeDef
-):
-    pass
-
-
 _RequiredS3JobManifestGeneratorTypeDef = TypedDict(
     "_RequiredS3JobManifestGeneratorTypeDef",
     {
         "SourceBucket": str,
         "EnableManifestOutput": bool,
     },
 )
@@ -2801,59 +2298,28 @@
         "ExpectedBucketOwner": str,
         "ManifestOutputLocation": S3ManifestOutputLocationTypeDef,
         "Filter": JobManifestGeneratorFilterTypeDef,
     },
     total=False,
 )
 
-
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
-
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
-    {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
-        "Bucket": str,
-    },
-)
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
-    {
-        "ID": str,
-        "Priority": int,
-        "Prefix": str,
-        "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
-    },
-    total=False,
-)
-
-
-class ReplicationRuleOutputTypeDef(
-    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
         "Bucket": str,
     },
@@ -2868,19 +2334,17 @@
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
     total=False,
 )
 
-
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
-
 AsyncOperationTypeDef = TypedDict(
     "AsyncOperationTypeDef",
     {
         "CreationTime": datetime,
         "Operation": AsyncOperationNameType,
         "RequestTokenARN": str,
         "RequestParameters": AsyncRequestParametersTypeDef,
@@ -2898,124 +2362,87 @@
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
-S3AccessControlPolicyOutputTypeDef = TypedDict(
-    "S3AccessControlPolicyOutputTypeDef",
-    {
-        "AccessControlList": S3AccessControlListOutputTypeDef,
-        "CannedAccessControlList": S3CannedAccessControlListType,
-    },
-    total=False,
-)
-
 S3AccessControlPolicyTypeDef = TypedDict(
     "S3AccessControlPolicyTypeDef",
     {
         "AccessControlList": S3AccessControlListTypeDef,
         "CannedAccessControlList": S3CannedAccessControlListType,
     },
     total=False,
 )
 
-StorageLensDataExportOutputTypeDef = TypedDict(
-    "StorageLensDataExportOutputTypeDef",
-    {
-        "S3BucketDestination": S3BucketDestinationOutputTypeDef,
-        "CloudWatchMetrics": CloudWatchMetricsTypeDef,
-    },
-    total=False,
-)
-
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationTypeDef,
         "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
-GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
-    {
-        "Configuration": ObjectLambdaConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
-ObjectLambdaConfigurationUnionTypeDef = Union[
-    ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-]
+GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+    {
+        "Configuration": ObjectLambdaConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
 GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationResultTypeDef",
     {
-        "Rules": List[LifecycleRuleOutputTypeDef],
+        "Rules": List[LifecycleRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
     total=False,
 )
 
-JobManifestGeneratorOutputTypeDef = TypedDict(
-    "JobManifestGeneratorOutputTypeDef",
-    {
-        "S3JobManifestGenerator": S3JobManifestGeneratorOutputTypeDef,
-    },
-    total=False,
-)
-
 JobManifestGeneratorTypeDef = TypedDict(
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
-ReplicationConfigurationOutputTypeDef = TypedDict(
-    "ReplicationConfigurationOutputTypeDef",
-    {
-        "Role": str,
-        "Rules": List[ReplicationRuleOutputTypeDef],
-    },
-)
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": Sequence[ReplicationRuleTypeDef],
+        "Rules": List[ReplicationRuleTypeDef],
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
@@ -3036,27 +2463,17 @@
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
-
 class AccountLevelTypeDef(_RequiredAccountLevelTypeDef, _OptionalAccountLevelTypeDef):
     pass
 
-
-S3SetObjectAclOperationOutputTypeDef = TypedDict(
-    "S3SetObjectAclOperationOutputTypeDef",
-    {
-        "AccessControlPolicy": S3AccessControlPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 S3SetObjectAclOperationTypeDef = TypedDict(
     "S3SetObjectAclOperationTypeDef",
     {
         "AccessControlPolicy": S3AccessControlPolicyTypeDef,
     },
     total=False,
 )
@@ -3072,72 +2489,37 @@
     "_OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "LifecycleConfiguration": LifecycleConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-JobManifestGeneratorUnionTypeDef = Union[
-    JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
-]
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
-_RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStorageLensConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "AccountLevel": AccountLevelTypeDef,
-        "IsEnabled": bool,
-    },
-)
-_OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStorageLensConfigurationOutputTypeDef",
-    {
-        "Include": IncludeOutputTypeDef,
-        "Exclude": ExcludeOutputTypeDef,
-        "DataExport": StorageLensDataExportOutputTypeDef,
-        "AwsOrg": StorageLensAwsOrgTypeDef,
-        "StorageLensArn": str,
-    },
-    total=False,
-)
-
-
-class StorageLensConfigurationOutputTypeDef(
-    _RequiredStorageLensConfigurationOutputTypeDef, _OptionalStorageLensConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredStorageLensConfigurationTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -3150,37 +2532,19 @@
         "DataExport": StorageLensDataExportTypeDef,
         "AwsOrg": StorageLensAwsOrgTypeDef,
         "StorageLensArn": str,
     },
     total=False,
 )
 
-
 class StorageLensConfigurationTypeDef(
     _RequiredStorageLensConfigurationTypeDef, _OptionalStorageLensConfigurationTypeDef
 ):
     pass
 
-
-JobOperationOutputTypeDef = TypedDict(
-    "JobOperationOutputTypeDef",
-    {
-        "LambdaInvoke": LambdaInvokeOperationTypeDef,
-        "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
-        "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
-        "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
-        "S3DeleteObjectTagging": Dict[str, Any],
-        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationTypeDef,
-        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationTypeDef,
-        "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
-        "S3ReplicateObject": Dict[str, Any],
-    },
-    total=False,
-)
-
 JobOperationTypeDef = TypedDict(
     "JobOperationTypeDef",
     {
         "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationTypeDef,
         "S3PutObjectTagging": S3SetObjectTaggingOperationTypeDef,
@@ -3192,15 +2556,15 @@
     },
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
-        "StorageLensConfiguration": StorageLensConfigurationOutputTypeDef,
+        "StorageLensConfiguration": StorageLensConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
@@ -3213,51 +2577,20 @@
     "_OptionalPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "Tags": Sequence[StorageLensTagTypeDef],
     },
     total=False,
 )
 
-
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-StorageLensConfigurationUnionTypeDef = Union[
-    StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
-]
-JobDescriptorTypeDef = TypedDict(
-    "JobDescriptorTypeDef",
-    {
-        "JobId": str,
-        "ConfirmationRequired": bool,
-        "Description": str,
-        "JobArn": str,
-        "Status": JobStatusType,
-        "Manifest": JobManifestOutputTypeDef,
-        "Operation": JobOperationOutputTypeDef,
-        "Priority": int,
-        "ProgressSummary": JobProgressSummaryTypeDef,
-        "StatusUpdateReason": str,
-        "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportTypeDef,
-        "CreationTime": datetime,
-        "TerminationDate": datetime,
-        "RoleArn": str,
-        "SuspendedDate": datetime,
-        "SuspendedCause": str,
-        "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
-        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "AccountId": str,
         "Operation": JobOperationTypeDef,
         "Report": JobReportTypeDef,
         "ClientRequestToken": str,
@@ -3273,22 +2606,45 @@
         "Description": str,
         "Tags": Sequence[S3TagTypeDef],
         "ManifestGenerator": JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
+JobDescriptorTypeDef = TypedDict(
+    "JobDescriptorTypeDef",
+    {
+        "JobId": str,
+        "ConfirmationRequired": bool,
+        "Description": str,
+        "JobArn": str,
+        "Status": JobStatusType,
+        "Manifest": JobManifestTypeDef,
+        "Operation": JobOperationTypeDef,
+        "Priority": int,
+        "ProgressSummary": JobProgressSummaryTypeDef,
+        "StatusUpdateReason": str,
+        "FailureReasons": List[JobFailureTypeDef],
+        "Report": JobReportTypeDef,
+        "CreationTime": datetime,
+        "TerminationDate": datetime,
+        "RoleArn": str,
+        "SuspendedDate": datetime,
+        "SuspendedCause": str,
+        "ManifestGenerator": JobManifestGeneratorTypeDef,
+        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
+    },
+    total=False,
+)
 
-JobOperationUnionTypeDef = Union[JobOperationTypeDef, JobOperationOutputTypeDef]
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control/type_defs.pyi` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "AccessControlTranslationTypeDef",
     "VpcConfigurationTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
@@ -101,15 +102,14 @@
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
-    "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
     "ExistingObjectReplicationTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
@@ -129,29 +129,26 @@
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     "StorageLensTagTypeDef",
-    "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
-    "JobManifestGeneratorFilterOutputTypeDef",
     "TimestampTypeDef",
     "JobManifestLocationTypeDef",
-    "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
-    "LifecycleExpirationOutputTypeDef",
+    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionOutputTypeDef",
+    "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
@@ -164,18 +161,16 @@
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "ReplicaModificationsTypeDef",
     "S3ObjectOwnerTypeDef",
-    "S3ObjectMetadataOutputTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
-    "S3RetentionOutputTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
@@ -201,131 +196,96 @@
     "GetAccessPointForObjectLambdaResultTypeDef",
     "GetAccessPointResultTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "GetBucketTaggingResultTypeDef",
     "GetJobTaggingResultTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
-    "S3SetObjectTaggingOperationOutputTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
-    "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
-    "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "JobManifestGeneratorFilterTypeDef",
-    "LifecycleExpirationTypeDef",
     "S3ObjectMetadataTypeDef",
     "S3RetentionTypeDef",
-    "TransitionTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
-    "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
-    "S3SetObjectRetentionOperationOutputTypeDef",
-    "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
-    "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
-    "CreateMultiRegionAccessPointInputUnionTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
-    "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
-    "JobManifestUnionTypeDef",
     "JobListDescriptorTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
     "PrefixLevelTypeDef",
-    "S3AccessControlListOutputTypeDef",
     "S3AccessControlListTypeDef",
-    "S3CopyObjectOperationOutputTypeDef",
     "S3CopyObjectOperationTypeDef",
-    "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
-    "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
-    "LifecycleRuleOutputTypeDef",
     "LifecycleRuleTypeDef",
-    "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
     "ListJobsResultTypeDef",
-    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
     "BucketLevelTypeDef",
-    "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
-    "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
-    "ObjectLambdaConfigurationUnionTypeDef",
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
-    "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     "AccountLevelTypeDef",
-    "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "JobManifestGeneratorUnionTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
-    "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
-    "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
-    "StorageLensConfigurationUnionTypeDef",
-    "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobOperationUnionTypeDef",
+    "JobDescriptorTypeDef",
     "DescribeJobResultTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -415,19 +375,21 @@
     "_OptionalAwsLambdaTransformationTypeDef",
     {
         "FunctionPayload": str,
     },
     total=False,
 )
 
+
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
+
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -483,17 +445,19 @@
         "Format": Literal["Report_CSV_20180820"],
         "Prefix": str,
         "ReportScope": JobReportScopeType,
     },
     total=False,
 )
 
+
 class JobReportTypeDef(_RequiredJobReportTypeDef, _OptionalJobReportTypeDef):
     pass
 
+
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -508,17 +472,19 @@
     "_OptionalRegionTypeDef",
     {
         "BucketAccountId": str,
     },
     total=False,
 )
 
+
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
+
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -653,28 +619,19 @@
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-ExcludeOutputTypeDef = TypedDict(
-    "ExcludeOutputTypeDef",
-    {
-        "Buckets": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
 ExcludeTypeDef = TypedDict(
     "ExcludeTypeDef",
     {
-        "Buckets": Sequence[str],
-        "Regions": Sequence[str],
+        "Buckets": List[str],
+        "Regions": List[str],
     },
     total=False,
 )
 
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
@@ -852,19 +809,21 @@
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
+
 class MultiRegionAccessPointRouteTypeDef(
     _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
 ):
     pass
 
+
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -888,52 +847,32 @@
     "StorageLensTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-IncludeOutputTypeDef = TypedDict(
-    "IncludeOutputTypeDef",
-    {
-        "Buckets": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
 IncludeTypeDef = TypedDict(
     "IncludeTypeDef",
     {
-        "Buckets": Sequence[str],
-        "Regions": Sequence[str],
+        "Buckets": List[str],
+        "Regions": List[str],
     },
     total=False,
 )
 
 JobFailureTypeDef = TypedDict(
     "JobFailureTypeDef",
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
-JobManifestGeneratorFilterOutputTypeDef = TypedDict(
-    "JobManifestGeneratorFilterOutputTypeDef",
-    {
-        "EligibleForReplication": bool,
-        "CreatedAfter": datetime,
-        "CreatedBefore": datetime,
-        "ObjectReplicationStatuses": List[ReplicationStatusType],
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
@@ -942,37 +881,20 @@
     "_OptionalJobManifestLocationTypeDef",
     {
         "ObjectVersionId": str,
     },
     total=False,
 )
 
+
 class JobManifestLocationTypeDef(
     _RequiredJobManifestLocationTypeDef, _OptionalJobManifestLocationTypeDef
 ):
     pass
 
-_RequiredJobManifestSpecOutputTypeDef = TypedDict(
-    "_RequiredJobManifestSpecOutputTypeDef",
-    {
-        "Format": JobManifestFormatType,
-    },
-)
-_OptionalJobManifestSpecOutputTypeDef = TypedDict(
-    "_OptionalJobManifestSpecOutputTypeDef",
-    {
-        "Fields": List[JobManifestFieldNameType],
-    },
-    total=False,
-)
-
-class JobManifestSpecOutputTypeDef(
-    _RequiredJobManifestSpecOutputTypeDef, _OptionalJobManifestSpecOutputTypeDef
-):
-    pass
 
 _RequiredJobManifestSpecTypeDef = TypedDict(
     "_RequiredJobManifestSpecTypeDef",
     {
         "Format": JobManifestFormatType,
     },
 )
@@ -980,17 +902,19 @@
     "_OptionalJobManifestSpecTypeDef",
     {
         "Fields": Sequence[JobManifestFieldNameType],
     },
     total=False,
 )
 
+
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
+
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1008,16 +932,16 @@
     "JobTimersTypeDef",
     {
         "ElapsedTimeInActiveSeconds": int,
     },
     total=False,
 )
 
-LifecycleExpirationOutputTypeDef = TypedDict(
-    "LifecycleExpirationOutputTypeDef",
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
@@ -1036,16 +960,16 @@
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-TransitionOutputTypeDef = TypedDict(
-    "TransitionOutputTypeDef",
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
@@ -1071,20 +995,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAccessPointsForObjectLambdaRequestRequestTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1093,19 +1019,21 @@
         "Bucket": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAccessPointsRequestRequestTypeDef(
     _RequiredListAccessPointsRequestRequestTypeDef, _OptionalListAccessPointsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -1114,19 +1042,21 @@
         "JobStatuses": Sequence[JobStatusType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListMultiRegionAccessPointsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiRegionAccessPointsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListMultiRegionAccessPointsRequestRequestTypeDef = TypedDict(
@@ -1134,20 +1064,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMultiRegionAccessPointsRequestRequestTypeDef(
     _RequiredListMultiRegionAccessPointsRequestRequestTypeDef,
     _OptionalListMultiRegionAccessPointsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListRegionalBucketsRequestRequestTypeDef = TypedDict(
     "_RequiredListRegionalBucketsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListRegionalBucketsRequestRequestTypeDef = TypedDict(
@@ -1156,20 +1088,22 @@
         "NextToken": str,
         "MaxResults": int,
         "OutpostId": str,
     },
     total=False,
 )
 
+
 class ListRegionalBucketsRequestRequestTypeDef(
     _RequiredListRegionalBucketsRequestRequestTypeDef,
     _OptionalListRegionalBucketsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRegionalBucketTypeDef = TypedDict(
     "_RequiredRegionalBucketTypeDef",
     {
         "Bucket": str,
         "PublicAccessBlockEnabled": bool,
         "CreationDate": datetime,
     },
@@ -1179,17 +1113,19 @@
     {
         "BucketArn": str,
         "OutpostId": str,
     },
     total=False,
 )
 
+
 class RegionalBucketTypeDef(_RequiredRegionalBucketTypeDef, _OptionalRegionalBucketTypeDef):
     pass
 
+
 _RequiredListStorageLensConfigurationEntryTypeDef = TypedDict(
     "_RequiredListStorageLensConfigurationEntryTypeDef",
     {
         "Id": str,
         "StorageLensArn": str,
         "HomeRegion": str,
     },
@@ -1198,40 +1134,44 @@
     "_OptionalListStorageLensConfigurationEntryTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
 
+
 class ListStorageLensConfigurationEntryTypeDef(
     _RequiredListStorageLensConfigurationEntryTypeDef,
     _OptionalListStorageLensConfigurationEntryTypeDef,
 ):
     pass
 
+
 _RequiredListStorageLensConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListStorageLensConfigurationsRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListStorageLensConfigurationsRequestRequestTypeDef = TypedDict(
     "_OptionalListStorageLensConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1303,19 +1243,21 @@
     "_OptionalPutBucketPolicyRequestRequestTypeDef",
     {
         "ConfirmRemoveSelfBucketAccess": bool,
     },
     total=False,
 )
 
+
 class PutBucketPolicyRequestRequestTypeDef(
     _RequiredPutBucketPolicyRequestRequestTypeDef, _OptionalPutBucketPolicyRequestRequestTypeDef
 ):
     pass
 
+
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
@@ -1333,32 +1275,14 @@
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-S3ObjectMetadataOutputTypeDef = TypedDict(
-    "S3ObjectMetadataOutputTypeDef",
-    {
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "UserMetadata": Dict[str, str],
-        "ContentLength": int,
-        "ContentMD5": str,
-        "ContentType": str,
-        "HttpExpiresDate": datetime,
-        "RequesterCharged": bool,
-        "SSEAlgorithm": S3SSEAlgorithmType,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
@@ -1368,23 +1292,14 @@
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
-S3RetentionOutputTypeDef = TypedDict(
-    "S3RetentionOutputTypeDef",
-    {
-        "RetainUntilDate": datetime,
-        "Mode": S3ObjectLockRetentionModeType,
-    },
-    total=False,
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -1423,19 +1338,21 @@
     "_OptionalUpdateJobStatusRequestRequestTypeDef",
     {
         "StatusUpdateReason": str,
     },
     total=False,
 )
 
+
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
@@ -1447,17 +1364,19 @@
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
+
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
+
 DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": DeleteMultiRegionAccessPointInputTypeDef,
     },
@@ -1491,19 +1410,21 @@
     {
         "ObjectLambdaAccessPointArn": str,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
     },
     total=False,
 )
 
+
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
+
 CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointArn": str,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1642,19 +1563,21 @@
         "VpcConfiguration": VpcConfigurationTypeDef,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "BucketAccountId": str,
     },
     total=False,
 )
 
+
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
+
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
@@ -1713,19 +1636,21 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "OutpostId": str,
     },
     total=False,
 )
 
+
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
+
 GetBucketTaggingResultTypeDef = TypedDict(
     "GetBucketTaggingResultTypeDef",
     {
         "TagSet": List[S3TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1734,30 +1659,19 @@
     "GetJobTaggingResultTypeDef",
     {
         "Tags": List[S3TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagTypeDef],
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[S3TagTypeDef],
+        "Tags": List[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 PutJobTaggingRequestRequestTypeDef = TypedDict(
@@ -1765,36 +1679,19 @@
     {
         "AccountId": str,
         "JobId": str,
         "Tags": Sequence[S3TagTypeDef],
     },
 )
 
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[S3TagTypeDef],
-    },
-    total=False,
-)
-
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[S3TagTypeDef],
-    },
-    total=False,
-)
-
-S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
-    "S3SetObjectTaggingOperationOutputTypeDef",
-    {
-        "TagSet": List[S3TagTypeDef],
+        "Tags": List[S3TagTypeDef],
     },
     total=False,
 )
 
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
@@ -1806,35 +1703,14 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
-_RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
-    {
-        "Name": str,
-        "Regions": List[RegionTypeDef],
-    },
-)
-_OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
-    "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
-    {
-        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateMultiRegionAccessPointInputOutputTypeDef(
-    _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
-    _OptionalCreateMultiRegionAccessPointInputOutputTypeDef,
-):
-    pass
-
 _RequiredCreateMultiRegionAccessPointInputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
         "Regions": Sequence[RegionTypeDef],
     },
 )
@@ -1842,28 +1718,21 @@
     "_OptionalCreateMultiRegionAccessPointInputTypeDef",
     {
         "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
-GeneratedManifestEncryptionOutputTypeDef = TypedDict(
-    "GeneratedManifestEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSEncryptionTypeDef,
-    },
-    total=False,
-)
 
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSEncryptionTypeDef,
     },
@@ -1936,24 +1805,14 @@
         "CreatedAfter": TimestampTypeDef,
         "CreatedBefore": TimestampTypeDef,
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Days": int,
-        "ExpiredObjectDeleteMarker": bool,
-    },
-    total=False,
-)
-
 S3ObjectMetadataTypeDef = TypedDict(
     "S3ObjectMetadataTypeDef",
     {
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
         "ContentLanguage": str,
@@ -1973,41 +1832,23 @@
     {
         "RetainUntilDate": TimestampTypeDef,
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Days": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
         "Location": JobManifestLocationTypeDef,
     },
     total=False,
 )
 
-JobManifestOutputTypeDef = TypedDict(
-    "JobManifestOutputTypeDef",
-    {
-        "Spec": JobManifestSpecOutputTypeDef,
-        "Location": JobManifestLocationTypeDef,
-    },
-)
-
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
         "Location": JobManifestLocationTypeDef,
     },
 )
@@ -2033,20 +1874,22 @@
     "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
     _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
 ):
     pass
 
+
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2071,17 +1914,19 @@
     "_OptionalMetricsTypeDef",
     {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
     total=False,
 )
 
+
 class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
     pass
 
+
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
@@ -2137,20 +1982,22 @@
     "_OptionalPutBucketVersioningRequestRequestTypeDef",
     {
         "MFA": str,
     },
     total=False,
 )
 
+
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
+
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
@@ -2159,47 +2006,18 @@
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
-_RequiredS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
-    "_RequiredS3SetObjectRetentionOperationOutputTypeDef",
-    {
-        "Retention": S3RetentionOutputTypeDef,
-    },
-)
-_OptionalS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
-    "_OptionalS3SetObjectRetentionOperationOutputTypeDef",
-    {
-        "BypassGovernanceRetention": bool,
-    },
-    total=False,
-)
-
-class S3SetObjectRetentionOperationOutputTypeDef(
-    _RequiredS3SetObjectRetentionOperationOutputTypeDef,
-    _OptionalS3SetObjectRetentionOperationOutputTypeDef,
-):
-    pass
-
-StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
-    "StorageLensDataExportEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSTypeDef,
-    },
-    total=False,
-)
-
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
-        "SSES3": Mapping[str, Any],
+        "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
@@ -2215,22 +2033,14 @@
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
-    "ObjectLambdaTransformationConfigurationOutputTypeDef",
-    {
-        "Actions": List[ObjectLambdaTransformationConfigurationActionType],
-        "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
-    },
-)
-
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
         "ContentTransformation": ObjectLambdaContentTransformationTypeDef,
     },
 )
@@ -2240,48 +2050,26 @@
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagTypeDef,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
-        "ObjectSizeGreaterThan": int,
-        "ObjectSizeLessThan": int,
-    },
-    total=False,
-)
-
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": LifecycleRuleAndOperatorTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": S3TagTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": S3TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -2296,55 +2084,30 @@
         "Tagging": TaggingTypeDef,
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
-        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
+        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputTypeDef,
         "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
         "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
-CreateMultiRegionAccessPointInputUnionTypeDef = Union[
-    CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
-]
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
 )
 
-_RequiredS3ManifestOutputLocationOutputTypeDef = TypedDict(
-    "_RequiredS3ManifestOutputLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
-    },
-)
-_OptionalS3ManifestOutputLocationOutputTypeDef = TypedDict(
-    "_OptionalS3ManifestOutputLocationOutputTypeDef",
-    {
-        "ExpectedManifestBucketOwner": str,
-        "ManifestPrefix": str,
-        "ManifestEncryption": GeneratedManifestEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-class S3ManifestOutputLocationOutputTypeDef(
-    _RequiredS3ManifestOutputLocationOutputTypeDef, _OptionalS3ManifestOutputLocationOutputTypeDef
-):
-    pass
-
 _RequiredS3ManifestOutputLocationTypeDef = TypedDict(
     "_RequiredS3ManifestOutputLocationTypeDef",
     {
         "Bucket": str,
         "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
     },
 )
@@ -2354,39 +2117,42 @@
         "ExpectedManifestBucketOwner": str,
         "ManifestPrefix": str,
         "ManifestEncryption": GeneratedManifestEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
+
 _RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_RequiredS3SetObjectRetentionOperationTypeDef",
     {
         "Retention": S3RetentionTypeDef,
     },
 )
 _OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_OptionalS3SetObjectRetentionOperationTypeDef",
     {
         "BypassGovernanceRetention": bool,
     },
     total=False,
 )
 
+
 class S3SetObjectRetentionOperationTypeDef(
     _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
 ):
     pass
 
-JobManifestUnionTypeDef = Union[JobManifestTypeDef, JobManifestOutputTypeDef]
+
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2413,17 +2179,19 @@
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Metrics": MetricsTypeDef,
         "StorageClass": ReplicationStorageClassType,
     },
     total=False,
 )
 
+
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
+
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2457,76 +2225,34 @@
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
-_RequiredS3AccessControlListOutputTypeDef = TypedDict(
-    "_RequiredS3AccessControlListOutputTypeDef",
-    {
-        "Owner": S3ObjectOwnerTypeDef,
-    },
-)
-_OptionalS3AccessControlListOutputTypeDef = TypedDict(
-    "_OptionalS3AccessControlListOutputTypeDef",
-    {
-        "Grants": List[S3GrantTypeDef],
-    },
-    total=False,
-)
-
-class S3AccessControlListOutputTypeDef(
-    _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
-):
-    pass
-
 _RequiredS3AccessControlListTypeDef = TypedDict(
     "_RequiredS3AccessControlListTypeDef",
     {
         "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListTypeDef = TypedDict(
     "_OptionalS3AccessControlListTypeDef",
     {
         "Grants": Sequence[S3GrantTypeDef],
     },
     total=False,
 )
 
+
 class S3AccessControlListTypeDef(
     _RequiredS3AccessControlListTypeDef, _OptionalS3AccessControlListTypeDef
 ):
     pass
 
-S3CopyObjectOperationOutputTypeDef = TypedDict(
-    "S3CopyObjectOperationOutputTypeDef",
-    {
-        "TargetResource": str,
-        "CannedAccessControlList": S3CannedAccessControlListType,
-        "AccessControlGrants": List[S3GrantTypeDef],
-        "MetadataDirective": S3MetadataDirectiveType,
-        "ModifiedSinceConstraint": datetime,
-        "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
-        "NewObjectTagging": List[S3TagTypeDef],
-        "RedirectLocation": str,
-        "RequesterPays": bool,
-        "StorageClass": S3StorageClassType,
-        "UnModifiedSinceConstraint": datetime,
-        "SSEAwsKmsKeyId": str,
-        "TargetKeyPrefix": str,
-        "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
-        "ObjectLockMode": S3ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "BucketKeyEnabled": bool,
-        "ChecksumAlgorithm": S3ChecksumAlgorithmType,
-    },
-    total=False,
-)
 
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
@@ -2545,37 +2271,14 @@
         "ObjectLockRetainUntilDate": TimestampTypeDef,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
-_RequiredS3BucketDestinationOutputTypeDef = TypedDict(
-    "_RequiredS3BucketDestinationOutputTypeDef",
-    {
-        "Format": FormatType,
-        "OutputSchemaVersion": Literal["V_1"],
-        "AccountId": str,
-        "Arn": str,
-    },
-)
-_OptionalS3BucketDestinationOutputTypeDef = TypedDict(
-    "_OptionalS3BucketDestinationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Encryption": StorageLensDataExportEncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
-class S3BucketDestinationOutputTypeDef(
-    _RequiredS3BucketDestinationOutputTypeDef, _OptionalS3BucketDestinationOutputTypeDef
-):
-    pass
-
 _RequiredS3BucketDestinationTypeDef = TypedDict(
     "_RequiredS3BucketDestinationTypeDef",
     {
         "Format": FormatType,
         "OutputSchemaVersion": Literal["V_1"],
         "AccountId": str,
         "Arn": str,
@@ -2586,39 +2289,20 @@
     {
         "Prefix": str,
         "Encryption": StorageLensDataExportEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class S3BucketDestinationTypeDef(
     _RequiredS3BucketDestinationTypeDef, _OptionalS3BucketDestinationTypeDef
 ):
     pass
 
-_RequiredObjectLambdaConfigurationOutputTypeDef = TypedDict(
-    "_RequiredObjectLambdaConfigurationOutputTypeDef",
-    {
-        "SupportingAccessPoint": str,
-        "TransformationConfigurations": List[ObjectLambdaTransformationConfigurationOutputTypeDef],
-    },
-)
-_OptionalObjectLambdaConfigurationOutputTypeDef = TypedDict(
-    "_OptionalObjectLambdaConfigurationOutputTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "AllowedFeatures": List[ObjectLambdaAllowedFeatureType],
-    },
-    total=False,
-)
-
-class ObjectLambdaConfigurationOutputTypeDef(
-    _RequiredObjectLambdaConfigurationOutputTypeDef, _OptionalObjectLambdaConfigurationOutputTypeDef
-):
-    pass
 
 _RequiredObjectLambdaConfigurationTypeDef = TypedDict(
     "_RequiredObjectLambdaConfigurationTypeDef",
     {
         "SupportingAccessPoint": str,
         "TransformationConfigurations": Sequence[ObjectLambdaTransformationConfigurationTypeDef],
     },
@@ -2628,88 +2312,45 @@
     {
         "CloudWatchMetricsEnabled": bool,
         "AllowedFeatures": Sequence[ObjectLambdaAllowedFeatureType],
     },
     total=False,
 )
 
+
 class ObjectLambdaConfigurationTypeDef(
     _RequiredObjectLambdaConfigurationTypeDef, _OptionalObjectLambdaConfigurationTypeDef
 ):
     pass
 
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
-    {
-        "Expiration": LifecycleExpirationOutputTypeDef,
-        "ID": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
-        "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
-        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
-    },
-    total=False,
-)
-
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
-):
-    pass
 
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Transitions": Sequence[TransitionTypeDef],
-        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
+        "Transitions": List[TransitionTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
+
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
-_RequiredS3JobManifestGeneratorOutputTypeDef = TypedDict(
-    "_RequiredS3JobManifestGeneratorOutputTypeDef",
-    {
-        "SourceBucket": str,
-        "EnableManifestOutput": bool,
-    },
-)
-_OptionalS3JobManifestGeneratorOutputTypeDef = TypedDict(
-    "_OptionalS3JobManifestGeneratorOutputTypeDef",
-    {
-        "ExpectedBucketOwner": str,
-        "ManifestOutputLocation": S3ManifestOutputLocationOutputTypeDef,
-        "Filter": JobManifestGeneratorFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-class S3JobManifestGeneratorOutputTypeDef(
-    _RequiredS3JobManifestGeneratorOutputTypeDef, _OptionalS3JobManifestGeneratorOutputTypeDef
-):
-    pass
 
 _RequiredS3JobManifestGeneratorTypeDef = TypedDict(
     "_RequiredS3JobManifestGeneratorTypeDef",
     {
         "SourceBucket": str,
         "EnableManifestOutput": bool,
     },
@@ -2720,55 +2361,30 @@
         "ExpectedBucketOwner": str,
         "ManifestOutputLocation": S3ManifestOutputLocationTypeDef,
         "Filter": JobManifestGeneratorFilterTypeDef,
     },
     total=False,
 )
 
+
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
+
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
-    {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
-        "Bucket": str,
-    },
-)
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
-    {
-        "ID": str,
-        "Priority": int,
-        "Prefix": str,
-        "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
-    },
-    total=False,
-)
-
-class ReplicationRuleOutputTypeDef(
-    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
-):
-    pass
-
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
         "Bucket": str,
     },
@@ -2783,17 +2399,19 @@
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
     total=False,
 )
 
+
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
+
 AsyncOperationTypeDef = TypedDict(
     "AsyncOperationTypeDef",
     {
         "CreationTime": datetime,
         "Operation": AsyncOperationNameType,
         "RequestTokenARN": str,
         "RequestParameters": AsyncRequestParametersTypeDef,
@@ -2811,124 +2429,87 @@
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
-S3AccessControlPolicyOutputTypeDef = TypedDict(
-    "S3AccessControlPolicyOutputTypeDef",
-    {
-        "AccessControlList": S3AccessControlListOutputTypeDef,
-        "CannedAccessControlList": S3CannedAccessControlListType,
-    },
-    total=False,
-)
-
 S3AccessControlPolicyTypeDef = TypedDict(
     "S3AccessControlPolicyTypeDef",
     {
         "AccessControlList": S3AccessControlListTypeDef,
         "CannedAccessControlList": S3CannedAccessControlListType,
     },
     total=False,
 )
 
-StorageLensDataExportOutputTypeDef = TypedDict(
-    "StorageLensDataExportOutputTypeDef",
-    {
-        "S3BucketDestination": S3BucketDestinationOutputTypeDef,
-        "CloudWatchMetrics": CloudWatchMetricsTypeDef,
-    },
-    total=False,
-)
-
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationTypeDef,
         "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
-GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
-    {
-        "Configuration": ObjectLambdaConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
-ObjectLambdaConfigurationUnionTypeDef = Union[
-    ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-]
+GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+    {
+        "Configuration": ObjectLambdaConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
 GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationResultTypeDef",
     {
-        "Rules": List[LifecycleRuleOutputTypeDef],
+        "Rules": List[LifecycleRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
     total=False,
 )
 
-JobManifestGeneratorOutputTypeDef = TypedDict(
-    "JobManifestGeneratorOutputTypeDef",
-    {
-        "S3JobManifestGenerator": S3JobManifestGeneratorOutputTypeDef,
-    },
-    total=False,
-)
-
 JobManifestGeneratorTypeDef = TypedDict(
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
-ReplicationConfigurationOutputTypeDef = TypedDict(
-    "ReplicationConfigurationOutputTypeDef",
-    {
-        "Role": str,
-        "Rules": List[ReplicationRuleOutputTypeDef],
-    },
-)
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": Sequence[ReplicationRuleTypeDef],
+        "Rules": List[ReplicationRuleTypeDef],
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
@@ -2949,24 +2530,18 @@
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
+
 class AccountLevelTypeDef(_RequiredAccountLevelTypeDef, _OptionalAccountLevelTypeDef):
     pass
 
-S3SetObjectAclOperationOutputTypeDef = TypedDict(
-    "S3SetObjectAclOperationOutputTypeDef",
-    {
-        "AccessControlPolicy": S3AccessControlPolicyOutputTypeDef,
-    },
-    total=False,
-)
 
 S3SetObjectAclOperationTypeDef = TypedDict(
     "S3SetObjectAclOperationTypeDef",
     {
         "AccessControlPolicy": S3AccessControlPolicyTypeDef,
     },
     total=False,
@@ -2983,68 +2558,39 @@
     "_OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "LifecycleConfiguration": LifecycleConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-JobManifestGeneratorUnionTypeDef = Union[
-    JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
-]
+
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
-_RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStorageLensConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "AccountLevel": AccountLevelTypeDef,
-        "IsEnabled": bool,
-    },
-)
-_OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStorageLensConfigurationOutputTypeDef",
-    {
-        "Include": IncludeOutputTypeDef,
-        "Exclude": ExcludeOutputTypeDef,
-        "DataExport": StorageLensDataExportOutputTypeDef,
-        "AwsOrg": StorageLensAwsOrgTypeDef,
-        "StorageLensArn": str,
-    },
-    total=False,
-)
-
-class StorageLensConfigurationOutputTypeDef(
-    _RequiredStorageLensConfigurationOutputTypeDef, _OptionalStorageLensConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredStorageLensConfigurationTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -3057,34 +2603,20 @@
         "DataExport": StorageLensDataExportTypeDef,
         "AwsOrg": StorageLensAwsOrgTypeDef,
         "StorageLensArn": str,
     },
     total=False,
 )
 
+
 class StorageLensConfigurationTypeDef(
     _RequiredStorageLensConfigurationTypeDef, _OptionalStorageLensConfigurationTypeDef
 ):
     pass
 
-JobOperationOutputTypeDef = TypedDict(
-    "JobOperationOutputTypeDef",
-    {
-        "LambdaInvoke": LambdaInvokeOperationTypeDef,
-        "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
-        "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
-        "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
-        "S3DeleteObjectTagging": Dict[str, Any],
-        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationTypeDef,
-        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationTypeDef,
-        "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
-        "S3ReplicateObject": Dict[str, Any],
-    },
-    total=False,
-)
 
 JobOperationTypeDef = TypedDict(
     "JobOperationTypeDef",
     {
         "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationTypeDef,
@@ -3097,15 +2629,15 @@
     },
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
-        "StorageLensConfiguration": StorageLensConfigurationOutputTypeDef,
+        "StorageLensConfiguration": StorageLensConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
@@ -3118,48 +2650,21 @@
     "_OptionalPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "Tags": Sequence[StorageLensTagTypeDef],
     },
     total=False,
 )
 
+
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
-StorageLensConfigurationUnionTypeDef = Union[
-    StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
-]
-JobDescriptorTypeDef = TypedDict(
-    "JobDescriptorTypeDef",
-    {
-        "JobId": str,
-        "ConfirmationRequired": bool,
-        "Description": str,
-        "JobArn": str,
-        "Status": JobStatusType,
-        "Manifest": JobManifestOutputTypeDef,
-        "Operation": JobOperationOutputTypeDef,
-        "Priority": int,
-        "ProgressSummary": JobProgressSummaryTypeDef,
-        "StatusUpdateReason": str,
-        "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportTypeDef,
-        "CreationTime": datetime,
-        "TerminationDate": datetime,
-        "RoleArn": str,
-        "SuspendedDate": datetime,
-        "SuspendedCause": str,
-        "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
-        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "AccountId": str,
         "Operation": JobOperationTypeDef,
         "Report": JobReportTypeDef,
@@ -3176,20 +2681,47 @@
         "Description": str,
         "Tags": Sequence[S3TagTypeDef],
         "ManifestGenerator": JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-JobOperationUnionTypeDef = Union[JobOperationTypeDef, JobOperationOutputTypeDef]
+
+JobDescriptorTypeDef = TypedDict(
+    "JobDescriptorTypeDef",
+    {
+        "JobId": str,
+        "ConfirmationRequired": bool,
+        "Description": str,
+        "JobArn": str,
+        "Status": JobStatusType,
+        "Manifest": JobManifestTypeDef,
+        "Operation": JobOperationTypeDef,
+        "Priority": int,
+        "ProgressSummary": JobProgressSummaryTypeDef,
+        "StatusUpdateReason": str,
+        "FailureReasons": List[JobFailureTypeDef],
+        "Report": JobReportTypeDef,
+        "CreationTime": datetime,
+        "TerminationDate": datetime,
+        "RoleArn": str,
+        "SuspendedDate": datetime,
+        "SuspendedCause": str,
+        "ManifestGenerator": JobManifestGeneratorTypeDef,
+        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-s3control-2.5.2.post1/types_aiobotocore_s3control.egg-info/SOURCES.txt` & `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

