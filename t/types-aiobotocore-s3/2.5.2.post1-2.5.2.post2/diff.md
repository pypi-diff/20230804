# Comparing `tmp/types-aiobotocore-s3-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-s3-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-s3-2.5.2.post1.tar` & `types-aiobotocore-s3-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.177474 types-aiobotocore-s3-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35834 2023-08-02 14:52:55.169474 types-aiobotocore-s3-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.177474 types-aiobotocore-s3-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.169474 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87231 2023-08-02 14:48:19.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    87110 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   124335 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   124114 2023-08-02 14:48:19.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   199186 2023-08-02 14:48:26.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   198849 2023-08-02 14:48:22.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:18.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-02 14:48:20.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.169474 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35834 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:55.000000 types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.456643 types-aiobotocore-s3-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17692 2023-08-04 13:59:24.446643 types-aiobotocore-s3-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16194 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.456643 types-aiobotocore-s3-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.426643 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2294 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2292 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    87379 2023-08-04 13:51:31.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    87258 2023-08-04 13:51:30.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16722 2023-08-04 13:51:33.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16720 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7661 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7653 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   124985 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   124764 2023-08-04 13:51:31.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   194181 2023-08-04 13:51:40.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   193855 2023-08-04 13:51:35.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5561 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5556 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.446643 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17692 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      864 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/LICENSE` & `types-aiobotocore-s3-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post1/setup.py` & `types-aiobotocore-s3-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__init__.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__init__.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/__main__.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.S3 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/client.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
-    AnalyticsConfigurationUnionTypeDef,
+    AnalyticsConfigurationTypeDef,
     BlobTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CompleteMultipartUploadOutputTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
@@ -91,52 +91,52 @@
     GetObjectOutputTypeDef,
     GetObjectRetentionOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     GetObjectTorrentOutputTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
-    IntelligentTieringConfigurationUnionTypeDef,
-    InventoryConfigurationUnionTypeDef,
+    IntelligentTieringConfigurationTypeDef,
+    InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
     ListBucketAnalyticsConfigurationsOutputTypeDef,
     ListBucketIntelligentTieringConfigurationsOutputTypeDef,
     ListBucketInventoryConfigurationsOutputTypeDef,
     ListBucketMetricsConfigurationsOutputTypeDef,
     ListBucketsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
     ListObjectsV2OutputTypeDef,
     ListObjectVersionsOutputTypeDef,
     ListPartsOutputTypeDef,
-    MetricsConfigurationUnionTypeDef,
+    MetricsConfigurationTypeDef,
     NotificationConfigurationDeprecatedResponseTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     NotificationConfigurationResponseTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
-    ObjectLockRetentionUnionTypeDef,
+    ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
-    OwnershipControlsUnionTypeDef,
+    OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectLegalHoldOutputTypeDef,
     PutObjectLockConfigurationOutputTypeDef,
     PutObjectOutputTypeDef,
     PutObjectRetentionOutputTypeDef,
     PutObjectTaggingOutputTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
     SelectObjectContentOutputTypeDef,
-    ServerSideEncryptionConfigurationUnionTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
     TimestampTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
@@ -1138,15 +1138,16 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectVersionsOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_object_versions)
         """
@@ -1157,15 +1158,16 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectsOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects)
         """
@@ -1178,15 +1180,16 @@
         EncodingType: Literal["url"] = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects_v2)
         """
@@ -1249,15 +1252,15 @@
         """
 
     async def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        AnalyticsConfiguration: AnalyticsConfigurationUnionTypeDef,
+        AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets an analytics configuration for the bucket (specified by the analytics
         configuration ID).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
@@ -1279,15 +1282,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_cors)
         """
 
     async def put_bucket_encryption(
         self,
         *,
         Bucket: str,
-        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationUnionTypeDef,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This action uses the `encryption` subresource to configure default encryption
         and Amazon S3 Bucket Keys for an existing bucket.
@@ -1297,29 +1300,29 @@
         """
 
     async def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationUnionTypeDef
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts a S3 Intelligent-Tiering configuration to the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
 
     async def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        InventoryConfiguration: InventoryConfigurationUnionTypeDef,
+        InventoryConfiguration: InventoryConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This implementation of the `PUT` action adds an inventory configuration
         (identified by the inventory ID) to the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
@@ -1374,15 +1377,15 @@
         """
 
     async def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        MetricsConfiguration: MetricsConfigurationUnionTypeDef,
+        MetricsConfiguration: MetricsConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets a metrics configuration (specified by the metrics configuration ID) for the
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
@@ -1421,15 +1424,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification_configuration)
         """
 
     async def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
-        OwnershipControls: OwnershipControlsUnionTypeDef,
+        OwnershipControls: OwnershipControlsTypeDef,
         ContentMD5: str = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or modifies `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
@@ -1452,15 +1455,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_policy)
         """
 
     async def put_bucket_replication(
         self,
         *,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef,
+        ReplicationConfiguration: ReplicationConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a replication configuration or replaces an existing one.
 
@@ -1641,15 +1644,15 @@
         """
 
     async def put_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
-        Retention: ObjectLockRetentionUnionTypeDef = ...,
+        Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> PutObjectRetentionOutputTypeDef:
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/client.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
-    AnalyticsConfigurationUnionTypeDef,
+    AnalyticsConfigurationTypeDef,
     BlobTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
     CompleteMultipartUploadOutputTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
@@ -91,52 +91,52 @@
     GetObjectOutputTypeDef,
     GetObjectRetentionOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     GetObjectTorrentOutputTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     HeadObjectOutputTypeDef,
     InputSerializationTypeDef,
-    IntelligentTieringConfigurationUnionTypeDef,
-    InventoryConfigurationUnionTypeDef,
+    IntelligentTieringConfigurationTypeDef,
+    InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
     ListBucketAnalyticsConfigurationsOutputTypeDef,
     ListBucketIntelligentTieringConfigurationsOutputTypeDef,
     ListBucketInventoryConfigurationsOutputTypeDef,
     ListBucketMetricsConfigurationsOutputTypeDef,
     ListBucketsOutputTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
     ListObjectsV2OutputTypeDef,
     ListObjectVersionsOutputTypeDef,
     ListPartsOutputTypeDef,
-    MetricsConfigurationUnionTypeDef,
+    MetricsConfigurationTypeDef,
     NotificationConfigurationDeprecatedResponseTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     NotificationConfigurationResponseTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
-    ObjectLockRetentionUnionTypeDef,
+    ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
-    OwnershipControlsUnionTypeDef,
+    OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectLegalHoldOutputTypeDef,
     PutObjectLockConfigurationOutputTypeDef,
     PutObjectOutputTypeDef,
     PutObjectRetentionOutputTypeDef,
     PutObjectTaggingOutputTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
     SelectObjectContentOutputTypeDef,
-    ServerSideEncryptionConfigurationUnionTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
     TimestampTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
@@ -1065,15 +1065,16 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectVersionsOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_object_versions)
         """
@@ -1083,15 +1084,16 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectsOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects)
         """
@@ -1103,15 +1105,16 @@
         EncodingType: Literal["url"] = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> ListObjectsV2OutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#list_objects_v2)
         """
@@ -1170,15 +1173,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_acl)
         """
     async def put_bucket_analytics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        AnalyticsConfiguration: AnalyticsConfigurationUnionTypeDef,
+        AnalyticsConfiguration: AnalyticsConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets an analytics configuration for the bucket (specified by the analytics
         configuration ID).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_analytics_configuration)
@@ -1198,15 +1201,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_cors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_cors)
         """
     async def put_bucket_encryption(
         self,
         *,
         Bucket: str,
-        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationUnionTypeDef,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This action uses the `encryption` subresource to configure default encryption
         and Amazon S3 Bucket Keys for an existing bucket.
@@ -1215,28 +1218,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_encryption)
         """
     async def put_bucket_intelligent_tiering_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        IntelligentTieringConfiguration: IntelligentTieringConfigurationUnionTypeDef
+        IntelligentTieringConfiguration: IntelligentTieringConfigurationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts a S3 Intelligent-Tiering configuration to the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_intelligent_tiering_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_intelligent_tiering_configuration)
         """
     async def put_bucket_inventory_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        InventoryConfiguration: InventoryConfigurationUnionTypeDef,
+        InventoryConfiguration: InventoryConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This implementation of the `PUT` action adds an inventory configuration
         (identified by the inventory ID) to the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_inventory_configuration)
@@ -1287,15 +1290,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_logging)
         """
     async def put_bucket_metrics_configuration(
         self,
         *,
         Bucket: str,
         Id: str,
-        MetricsConfiguration: MetricsConfigurationUnionTypeDef,
+        MetricsConfiguration: MetricsConfigurationTypeDef,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets a metrics configuration (specified by the metrics configuration ID) for the
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_metrics_configuration)
@@ -1331,15 +1334,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_notification_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_notification_configuration)
         """
     async def put_bucket_ownership_controls(
         self,
         *,
         Bucket: str,
-        OwnershipControls: OwnershipControlsUnionTypeDef,
+        OwnershipControls: OwnershipControlsTypeDef,
         ContentMD5: str = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or modifies `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_ownership_controls)
@@ -1360,15 +1363,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_bucket_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_bucket_policy)
         """
     async def put_bucket_replication(
         self,
         *,
         Bucket: str,
-        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef,
+        ReplicationConfiguration: ReplicationConfigurationTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         Token: str = ...,
         ExpectedBucketOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a replication configuration or replaces an existing one.
 
@@ -1540,15 +1543,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/client/#put_object_lock_configuration)
         """
     async def put_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
-        Retention: ObjectLockRetentionUnionTypeDef = ...,
+        Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> PutObjectRetentionOutputTypeDef:
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/literals.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "ObjectLockLegalHoldStatusType",
     "ObjectLockModeType",
     "ObjectLockRetentionModeType",
     "ObjectNotExistsWaiterName",
     "ObjectOwnershipType",
     "ObjectStorageClassType",
     "ObjectVersionStorageClassType",
+    "OptionalObjectAttributesType",
     "OwnerOverrideType",
     "PayerType",
     "PermissionType",
     "ProtocolType",
     "QuoteFieldsType",
     "ReplicaModificationsStatusType",
     "ReplicationRuleStatusType",
@@ -105,23 +106,25 @@
     "EU",
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "cn-north-1",
     "cn-northwest-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-2",
     "us-gov-east-1",
@@ -180,17 +183,19 @@
     "BucketKeyStatus",
     "ChecksumAlgorithm",
     "ETag",
     "EncryptionStatus",
     "IntelligentTieringAccessTier",
     "IsMultipartUploaded",
     "LastModifiedDate",
+    "ObjectAccessControlList",
     "ObjectLockLegalHoldStatus",
     "ObjectLockMode",
     "ObjectLockRetainUntilDate",
+    "ObjectOwner",
     "ReplicationStatus",
     "Size",
     "StorageClass",
 ]
 JSONTypeType = Literal["DOCUMENT", "LINES"]
 ListMultipartUploadsPaginatorName = Literal["list_multipart_uploads"]
 ListObjectVersionsPaginatorName = Literal["list_object_versions"]
@@ -227,14 +232,15 @@
     "OUTPOSTS",
     "REDUCED_REDUNDANCY",
     "SNOW",
     "STANDARD",
     "STANDARD_IA",
 ]
 ObjectVersionStorageClassType = Literal["STANDARD"]
+OptionalObjectAttributesType = Literal["RestoreStatus"]
 OwnerOverrideType = Literal["Destination"]
 PayerType = Literal["BucketOwner", "Requester"]
 PermissionType = Literal["FULL_CONTROL", "READ", "READ_ACP", "WRITE", "WRITE_ACP"]
 ProtocolType = Literal["http", "https"]
 QuoteFieldsType = Literal["ALWAYS", "ASNEEDED"]
 ReplicaModificationsStatusType = Literal["Disabled", "Enabled"]
 ReplicationRuleStatusType = Literal["Disabled", "Enabled"]
@@ -276,14 +282,15 @@
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
@@ -379,14 +386,15 @@
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
@@ -465,26 +473,28 @@
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
@@ -653,14 +663,15 @@
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

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/literals.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     "ObjectLockLegalHoldStatusType",
     "ObjectLockModeType",
     "ObjectLockRetentionModeType",
     "ObjectNotExistsWaiterName",
     "ObjectOwnershipType",
     "ObjectStorageClassType",
     "ObjectVersionStorageClassType",
+    "OptionalObjectAttributesType",
     "OwnerOverrideType",
     "PayerType",
     "PermissionType",
     "ProtocolType",
     "QuoteFieldsType",
     "ReplicaModificationsStatusType",
     "ReplicationRuleStatusType",
@@ -103,23 +104,25 @@
     "EU",
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "cn-north-1",
     "cn-northwest-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-2",
     "us-gov-east-1",
@@ -178,17 +181,19 @@
     "BucketKeyStatus",
     "ChecksumAlgorithm",
     "ETag",
     "EncryptionStatus",
     "IntelligentTieringAccessTier",
     "IsMultipartUploaded",
     "LastModifiedDate",
+    "ObjectAccessControlList",
     "ObjectLockLegalHoldStatus",
     "ObjectLockMode",
     "ObjectLockRetainUntilDate",
+    "ObjectOwner",
     "ReplicationStatus",
     "Size",
     "StorageClass",
 ]
 JSONTypeType = Literal["DOCUMENT", "LINES"]
 ListMultipartUploadsPaginatorName = Literal["list_multipart_uploads"]
 ListObjectVersionsPaginatorName = Literal["list_object_versions"]
@@ -225,14 +230,15 @@
     "OUTPOSTS",
     "REDUCED_REDUNDANCY",
     "SNOW",
     "STANDARD",
     "STANDARD_IA",
 ]
 ObjectVersionStorageClassType = Literal["STANDARD"]
+OptionalObjectAttributesType = Literal["RestoreStatus"]
 OwnerOverrideType = Literal["Destination"]
 PayerType = Literal["BucketOwner", "Requester"]
 PermissionType = Literal["FULL_CONTROL", "READ", "READ_ACP", "WRITE", "WRITE_ACP"]
 ProtocolType = Literal["http", "https"]
 QuoteFieldsType = Literal["ALWAYS", "ASNEEDED"]
 ReplicaModificationsStatusType = Literal["Disabled", "Enabled"]
 ReplicationRuleStatusType = Literal["Disabled", "Enabled"]
@@ -274,14 +280,15 @@
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
@@ -377,14 +384,15 @@
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
@@ -463,26 +471,28 @@
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
@@ -651,14 +661,15 @@
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

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/paginator.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         list_object_versions_paginator: ListObjectVersionsPaginator = client.get_paginator("list_object_versions")
         list_objects_paginator: ListObjectsPaginator = client.get_paginator("list_objects")
         list_objects_v2_paginator: ListObjectsV2Paginator = client.get_paginator("list_objects_v2")
         list_parts_paginator: ListPartsPaginator = client.get_paginator("list_parts")
     ```
 """
 import sys
-from typing import AsyncIterator, Generic, Iterator, TypeVar
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
@@ -102,14 +102,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectversionspaginator)
         """
 
@@ -125,14 +126,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectspaginator)
         """
 
@@ -150,14 +152,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectsv2paginator)
         """
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/paginator.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         list_object_versions_paginator: ListObjectVersionsPaginator = client.get_paginator("list_object_versions")
         list_objects_paginator: ListObjectsPaginator = client.get_paginator("list_objects")
         list_objects_v2_paginator: ListObjectsV2Paginator = client.get_paginator("list_objects_v2")
         list_parts_paginator: ListPartsPaginator = client.get_paginator("list_parts")
     ```
 """
 import sys
-from typing import AsyncIterator, Generic, Iterator, TypeVar
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListMultipartUploadsOutputTypeDef,
     ListObjectsOutputTypeDef,
@@ -97,14 +97,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectversionspaginator)
         """
 
@@ -119,14 +120,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectspaginator)
         """
 
@@ -143,14 +145,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/paginators/#listobjectsv2paginator)
         """
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/service_resource.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,53 +60,56 @@
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BlobTypeDef,
-    BucketLifecycleConfigurationTypeDef,
-    BucketLoggingStatusTypeDef,
+    BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
+    BucketLoggingStatusBucketLoggingTypeDef,
     CompletedMultipartUploadTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
     CopySourceTypeDef,
-    CORSConfigurationTypeDef,
-    CORSRuleOutputTypeDef,
+    CORSConfigurationBucketCorsTypeDef,
+    CORSRuleBucketCorsTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketOutputTypeDef,
     DeleteObjectOutputTypeDef,
     DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseTypeDef,
     FileobjTypeDef,
     GetObjectOutputTypeDef,
     GrantTypeDef,
     HeadObjectOutputTypeDef,
     IndexDocumentResponseTypeDef,
     InitiatorResponseTypeDef,
-    LambdaFunctionConfigurationOutputTypeDef,
-    LifecycleConfigurationTypeDef,
-    LifecycleRuleOutputTypeDef,
-    LoggingEnabledTypeDef,
-    NotificationConfigurationTypeDef,
+    LambdaFunctionConfigurationBucketNotificationTypeDef,
+    LifecycleConfigurationBucketLifecycleTypeDef,
+    LifecycleRuleBucketLifecycleConfigurationTypeDef,
+    LoggingEnabledResponseTypeDef,
+    NotificationConfigurationBucketNotificationTypeDef,
     OwnerResponseTypeDef,
+    OwnerTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectOutputTypeDef,
-    QueueConfigurationOutputTypeDef,
+    QueueConfigurationBucketNotificationTypeDef,
     RedirectAllRequestsToResponseTypeDef,
     RequestPaymentConfigurationTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
+    RestoreStatusResponseTypeDef,
+    RestoreStatusTypeDef,
     RoutingRuleTypeDef,
-    RuleOutputTypeDef,
+    RuleBucketLifecycleTypeDef,
     TaggingTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationOutputTypeDef,
+    TopicConfigurationBucketNotificationTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 try:
@@ -282,15 +285,16 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> "BucketObjectVersionsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
@@ -342,15 +346,16 @@
         *,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> "BucketObjectsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
 
     async def delete(
         self,
@@ -440,15 +445,15 @@
 
 class BucketAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl)
     """
 
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -508,15 +513,15 @@
 
 class BucketCors(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: Awaitable[List[CORSRuleOutputTypeDef]]
+    cors_rules: Awaitable[List[CORSRuleBucketCorsTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
@@ -547,15 +552,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsload-method)
         """
 
     async def put(
         self,
         *,
-        CORSConfiguration: CORSConfigurationTypeDef,
+        CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Sets the `cors` configuration for your bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
@@ -577,15 +582,15 @@
 
 class BucketLifecycle(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: Awaitable[List[RuleOutputTypeDef]]
+    rules: Awaitable[List[RuleBucketLifecycleTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
@@ -617,15 +622,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleload-method)
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleput-method)
@@ -646,15 +651,15 @@
 
 class BucketLifecycleConfiguration(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: Awaitable[List[LifecycleRuleOutputTypeDef]]
+    rules: Awaitable[List[LifecycleRuleBucketLifecycleConfigurationTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
@@ -686,15 +691,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationload-method)
         """
 
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Creates a new lifecycle configuration for the bucket or replaces an existing
         lifecycle configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
@@ -716,15 +721,15 @@
 
 class BucketLogging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging)
     """
 
-    logging_enabled: Awaitable[LoggingEnabledTypeDef]
+    logging_enabled: Awaitable[LoggingEnabledResponseTypeDef]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.Bucket)
@@ -747,15 +752,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingload-method)
         """
 
     async def put(
         self,
         *,
-        BucketLoggingStatus: BucketLoggingStatusTypeDef,
+        BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Set the logging parameters for a bucket and to specify permissions for who can
         view and modify the logging parameters.
 
@@ -778,17 +783,19 @@
 
 class BucketNotification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: Awaitable[List[TopicConfigurationOutputTypeDef]]
-    queue_configurations: Awaitable[List[QueueConfigurationOutputTypeDef]]
-    lambda_function_configurations: Awaitable[List[LambdaFunctionConfigurationOutputTypeDef]]
+    topic_configurations: Awaitable[List[TopicConfigurationBucketNotificationTypeDef]]
+    queue_configurations: Awaitable[List[QueueConfigurationBucketNotificationTypeDef]]
+    lambda_function_configurations: Awaitable[
+        List[LambdaFunctionConfigurationBucketNotificationTypeDef]
+    ]
     event_bridge_configuration: Awaitable[Dict[str, Any]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -812,15 +819,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationload-method)
         """
 
     async def put(
         self,
         *,
-        NotificationConfiguration: NotificationConfigurationTypeDef,
+        NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
         ExpectedBucketOwner: str = ...,
         SkipDestinationValidation: bool = ...
     ) -> None:
         """
         Enables notifications of specified events for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
@@ -1295,15 +1302,15 @@
 
 class ObjectAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl)
     """
 
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     request_charged: Awaitable[Literal["requester"]]
     bucket_name: str
     object_key: str
 
     async def Object(self) -> "_Object":
         """
@@ -1377,14 +1384,15 @@
     size: Awaitable[int]
     storage_class: Awaitable[Literal["STANDARD"]]
     key: Awaitable[str]
     version_id: Awaitable[str]
     is_latest: Awaitable[bool]
     last_modified: Awaitable[datetime]
     owner: Awaitable[OwnerResponseTypeDef]
+    restore_status: Awaitable[RestoreStatusResponseTypeDef]
     bucket_name: str
     object_key: str
     id: str
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
@@ -1480,15 +1488,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartupload)
     """
 
     upload_id: Awaitable[str]
     key: Awaitable[str]
     initiated: Awaitable[datetime]
     storage_class: Awaitable[StorageClassType]
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     initiator: Awaitable[InitiatorResponseTypeDef]
     checksum_algorithm: Awaitable[ChecksumAlgorithmType]
     bucket_name: str
     object_key: str
     id: str
     parts: MultipartUploadPartsCollection
 
@@ -1949,15 +1957,16 @@
     """
 
     last_modified: Awaitable[datetime]
     e_tag: Awaitable[str]
     checksum_algorithm: Awaitable[List[ChecksumAlgorithmType]]
     size: Awaitable[int]
     storage_class: Awaitable[ObjectStorageClassType]
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
+    restore_status: Awaitable[RestoreStatusTypeDef]
     bucket_name: str
     key: str
 
     async def Acl(self) -> _ObjectAcl:
         """
         Creates a ObjectAcl resource.
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/service_resource.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,53 +60,56 @@
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
     AbortMultipartUploadOutputTypeDef,
     AccessControlPolicyTypeDef,
     BlobTypeDef,
-    BucketLifecycleConfigurationTypeDef,
-    BucketLoggingStatusTypeDef,
+    BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
+    BucketLoggingStatusBucketLoggingTypeDef,
     CompletedMultipartUploadTypeDef,
     CopyObjectOutputTypeDef,
     CopySourceOrStrTypeDef,
     CopySourceTypeDef,
-    CORSConfigurationTypeDef,
-    CORSRuleOutputTypeDef,
+    CORSConfigurationBucketCorsTypeDef,
+    CORSRuleBucketCorsTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketOutputTypeDef,
     DeleteObjectOutputTypeDef,
     DeleteObjectsOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseTypeDef,
     FileobjTypeDef,
     GetObjectOutputTypeDef,
     GrantTypeDef,
     HeadObjectOutputTypeDef,
     IndexDocumentResponseTypeDef,
     InitiatorResponseTypeDef,
-    LambdaFunctionConfigurationOutputTypeDef,
-    LifecycleConfigurationTypeDef,
-    LifecycleRuleOutputTypeDef,
-    LoggingEnabledTypeDef,
-    NotificationConfigurationTypeDef,
+    LambdaFunctionConfigurationBucketNotificationTypeDef,
+    LifecycleConfigurationBucketLifecycleTypeDef,
+    LifecycleRuleBucketLifecycleConfigurationTypeDef,
+    LoggingEnabledResponseTypeDef,
+    NotificationConfigurationBucketNotificationTypeDef,
     OwnerResponseTypeDef,
+    OwnerTypeDef,
     PutObjectAclOutputTypeDef,
     PutObjectOutputTypeDef,
-    QueueConfigurationOutputTypeDef,
+    QueueConfigurationBucketNotificationTypeDef,
     RedirectAllRequestsToResponseTypeDef,
     RequestPaymentConfigurationTypeDef,
     RestoreObjectOutputTypeDef,
     RestoreRequestTypeDef,
+    RestoreStatusResponseTypeDef,
+    RestoreStatusTypeDef,
     RoutingRuleTypeDef,
-    RuleOutputTypeDef,
+    RuleBucketLifecycleTypeDef,
     TaggingTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TopicConfigurationOutputTypeDef,
+    TopicConfigurationBucketNotificationTypeDef,
     UploadPartCopyOutputTypeDef,
     UploadPartOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 try:
@@ -265,15 +268,16 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
-        RequestPayer: Literal["requester"] = ...
+        RequestPayer: Literal["requester"] = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> "BucketObjectVersionsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
     async def delete(
         self,
         *,
@@ -317,15 +321,16 @@
         *,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        ExpectedBucketOwner: str = ...
+        ExpectedBucketOwner: str = ...,
+        OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
     ) -> "BucketObjectsCollection":
         """
         Get items from the collection, passing keyword arguments along as parameters to the underlying service operation, which are typically used to filter the results.
         """
     async def delete(
         self,
         *,
@@ -401,15 +406,15 @@
 
 class BucketAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketacl)
     """
 
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -463,15 +468,15 @@
 
 class BucketCors(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: Awaitable[List[CORSRuleOutputTypeDef]]
+    cors_rules: Awaitable[List[CORSRuleBucketCorsTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
@@ -498,15 +503,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketcorsload-method)
         """
     async def put(
         self,
         *,
-        CORSConfiguration: CORSConfigurationTypeDef,
+        CORSConfiguration: CORSConfigurationBucketCorsTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Sets the `cors` configuration for your bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.put)
@@ -525,15 +530,15 @@
 
 class BucketLifecycle(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: Awaitable[List[RuleOutputTypeDef]]
+    rules: Awaitable[List[RuleBucketLifecycleTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
@@ -561,15 +566,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleload-method)
         """
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: LifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: LifecycleConfigurationBucketLifecycleTypeDef = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.put)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleput-method)
@@ -587,15 +592,15 @@
 
 class BucketLifecycleConfiguration(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: Awaitable[List[LifecycleRuleOutputTypeDef]]
+    rules: Awaitable[List[LifecycleRuleBucketLifecycleConfigurationTypeDef]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
@@ -623,15 +628,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlifecycleconfigurationload-method)
         """
     async def put(
         self,
         *,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
-        LifecycleConfiguration: BucketLifecycleConfigurationTypeDef = ...,
+        LifecycleConfiguration: BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Creates a new lifecycle configuration for the bucket or replaces an existing
         lifecycle configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.put)
@@ -650,15 +655,15 @@
 
 class BucketLogging(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLogging)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketlogging)
     """
 
-    logging_enabled: Awaitable[LoggingEnabledTypeDef]
+    logging_enabled: Awaitable[LoggingEnabledResponseTypeDef]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.Bucket)
@@ -678,15 +683,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLogging.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketloggingload-method)
         """
     async def put(
         self,
         *,
-        BucketLoggingStatus: BucketLoggingStatusTypeDef,
+        BucketLoggingStatus: BucketLoggingStatusBucketLoggingTypeDef,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
     ) -> None:
         """
         Set the logging parameters for a bucket and to specify permissions for who can
         view and modify the logging parameters.
 
@@ -706,17 +711,19 @@
 
 class BucketNotification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: Awaitable[List[TopicConfigurationOutputTypeDef]]
-    queue_configurations: Awaitable[List[QueueConfigurationOutputTypeDef]]
-    lambda_function_configurations: Awaitable[List[LambdaFunctionConfigurationOutputTypeDef]]
+    topic_configurations: Awaitable[List[TopicConfigurationBucketNotificationTypeDef]]
+    queue_configurations: Awaitable[List[QueueConfigurationBucketNotificationTypeDef]]
+    lambda_function_configurations: Awaitable[
+        List[LambdaFunctionConfigurationBucketNotificationTypeDef]
+    ]
     event_bridge_configuration: Awaitable[Dict[str, Any]]
     bucket_name: str
 
     async def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -737,15 +744,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#bucketnotificationload-method)
         """
     async def put(
         self,
         *,
-        NotificationConfiguration: NotificationConfigurationTypeDef,
+        NotificationConfiguration: NotificationConfigurationBucketNotificationTypeDef,
         ExpectedBucketOwner: str = ...,
         SkipDestinationValidation: bool = ...
     ) -> None:
         """
         Enables notifications of specified events for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketNotification.put)
@@ -1177,15 +1184,15 @@
 
 class ObjectAcl(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#objectacl)
     """
 
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     grants: Awaitable[List[GrantTypeDef]]
     request_charged: Awaitable[Literal["requester"]]
     bucket_name: str
     object_key: str
 
     async def Object(self) -> "_Object":
         """
@@ -1253,14 +1260,15 @@
     size: Awaitable[int]
     storage_class: Awaitable[Literal["STANDARD"]]
     key: Awaitable[str]
     version_id: Awaitable[str]
     is_latest: Awaitable[bool]
     last_modified: Awaitable[datetime]
     owner: Awaitable[OwnerResponseTypeDef]
+    restore_status: Awaitable[RestoreStatusResponseTypeDef]
     bucket_name: str
     object_key: str
     id: str
 
     async def Object(self) -> "_Object":
         """
         Creates a Object resource.
@@ -1350,15 +1358,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/service_resource/#multipartupload)
     """
 
     upload_id: Awaitable[str]
     key: Awaitable[str]
     initiated: Awaitable[datetime]
     storage_class: Awaitable[StorageClassType]
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
     initiator: Awaitable[InitiatorResponseTypeDef]
     checksum_algorithm: Awaitable[ChecksumAlgorithmType]
     bucket_name: str
     object_key: str
     id: str
     parts: MultipartUploadPartsCollection
 
@@ -1792,15 +1800,16 @@
     """
 
     last_modified: Awaitable[datetime]
     e_tag: Awaitable[str]
     checksum_algorithm: Awaitable[List[ChecksumAlgorithmType]]
     size: Awaitable[int]
     storage_class: Awaitable[ObjectStorageClassType]
-    owner: Awaitable[OwnerResponseTypeDef]
+    owner: Awaitable[OwnerTypeDef]
+    restore_status: Awaitable[RestoreStatusTypeDef]
     bucket_name: str
     key: str
 
     async def Acl(self) -> _ObjectAcl:
         """
         Creates a ObjectAcl resource.
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/type_defs.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,33 +85,31 @@
 
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
-    "OwnerTypeDef",
     "AccessControlTranslationTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "BlobTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "FileobjTypeDef",
     "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
+    "CORSRuleBucketCorsTypeDef",
     "CORSRuleTypeDef",
-    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
-    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "TimestampTypeDef",
     "CopyPartResultTypeDef",
@@ -178,15 +176,15 @@
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "ObjectLockRetentionOutputTypeDef",
+    "ObjectLockRetentionTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
@@ -195,33 +193,31 @@
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
-    "LifecycleExpirationOutputTypeDef",
+    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionOutputTypeDef",
+    "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
-    "QueueConfigurationDeprecatedOutputTypeDef",
-    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "OwnershipControlsRuleTypeDef",
     "ProgressTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
@@ -253,38 +249,34 @@
     "GetBucketVersioningOutputTypeDef",
     "GetObjectOutputTypeDef",
     "GetObjectTorrentOutputTypeDef",
     "HeadObjectOutputTypeDef",
     "IndexDocumentResponseTypeDef",
     "InitiatorResponseTypeDef",
     "OwnerResponseTypeDef",
+    "OwnerTypeDef",
     "PutObjectAclOutputTypeDef",
     "PutObjectLegalHoldOutputTypeDef",
     "PutObjectLockConfigurationOutputTypeDef",
     "PutObjectOutputTypeDef",
     "PutObjectRetentionOutputTypeDef",
     "PutObjectTaggingOutputTypeDef",
     "RedirectAllRequestsToResponseTypeDef",
     "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseTypeDef",
+    "RestoreStatusTypeDef",
     "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
-    "DeleteMarkerEntryTypeDef",
-    "ObjectTypeDef",
-    "ObjectVersionTypeDef",
-    "AnalyticsAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
-    "IntelligentTieringAndOperatorOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
+    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
-    "MetricsAndOperatorOutputTypeDef",
     "MetricsAndOperatorTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
@@ -292,15 +284,15 @@
     "ObjectCopyRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "ListBucketsOutputTypeDef",
+    "CORSConfigurationBucketCorsTypeDef",
     "CORSConfigurationTypeDef",
     "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
     "CopyObjectOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
@@ -308,200 +300,187 @@
     "CreateMultipartUploadRequestRequestTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "LifecycleExpirationTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
+    "LifecycleExpirationBucketLifecycleTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "TransitionTypeDef",
+    "TransitionBucketLifecycleConfigurationTypeDef",
+    "TransitionBucketLifecycleTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "UploadPartCopyOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockRuleTypeDef",
     "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
-    "S3KeyFilterOutputTypeDef",
+    "S3KeyFilterBucketNotificationTypeDef",
     "S3KeyFilterTypeDef",
     "GetBucketPolicyStatusOutputTypeDef",
     "GetObjectAttributesPartsTypeDef",
     "GetObjectLegalHoldOutputTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "GetObjectRetentionOutputTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
-    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
-    "RuleOutputTypeDef",
+    "RuleTypeDef",
     "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
-    "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
-    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
     "ProgressEventTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "StatsEventTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListObjectsV2OutputTypeDef",
-    "ListObjectVersionsOutputTypeDef",
-    "AnalyticsFilterOutputTypeDef",
+    "DeleteMarkerEntryTypeDef",
+    "ListBucketsOutputTypeDef",
+    "ListPartsOutputTypeDef",
+    "MultipartUploadTypeDef",
+    "ObjectTypeDef",
+    "ObjectVersionTypeDef",
     "AnalyticsFilterTypeDef",
-    "IntelligentTieringFilterOutputTypeDef",
     "IntelligentTieringFilterTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
+    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleFilterTypeDef",
-    "MetricsFilterOutputTypeDef",
     "MetricsFilterTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
-    "ObjectLockRetentionUnionTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
-    "RuleTypeDef",
+    "RuleBucketLifecycleTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
-    "NotificationConfigurationFilterOutputTypeDef",
+    "NotificationConfigurationFilterBucketNotificationTypeDef",
     "NotificationConfigurationFilterTypeDef",
     "GetObjectAttributesOutputTypeDef",
     "AccessControlPolicyTypeDef",
     "GetBucketAclOutputTypeDef",
     "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
-    "LoggingEnabledOutputTypeDef",
+    "LoggingEnabledBucketLoggingTypeDef",
+    "LoggingEnabledResponseTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputTypeDef",
-    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
     "GetBucketLifecycleOutputTypeDef",
+    "LifecycleConfigurationTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
     "GetBucketOwnershipControlsOutputTypeDef",
-    "OwnershipControlsUnionTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
     "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "SelectObjectContentEventStreamTypeDef",
-    "IntelligentTieringConfigurationOutputTypeDef",
+    "ListMultipartUploadsOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListObjectsV2OutputTypeDef",
+    "ListObjectVersionsOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
-    "LifecycleRuleOutputTypeDef",
+    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleTypeDef",
-    "MetricsConfigurationOutputTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisTypeDef",
-    "LifecycleConfigurationTypeDef",
+    "LifecycleConfigurationBucketLifecycleTypeDef",
     "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
-    "LambdaFunctionConfigurationOutputTypeDef",
-    "QueueConfigurationOutputTypeDef",
-    "TopicConfigurationOutputTypeDef",
+    "LambdaFunctionConfigurationBucketNotificationTypeDef",
+    "QueueConfigurationBucketNotificationTypeDef",
+    "TopicConfigurationBucketNotificationTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
-    "GetBucketLoggingOutputTypeDef",
+    "BucketLoggingStatusBucketLoggingTypeDef",
     "BucketLoggingStatusTypeDef",
-    "InventoryDestinationOutputTypeDef",
+    "GetBucketLoggingOutputTypeDef",
     "InventoryDestinationTypeDef",
-    "ReplicationRuleOutputTypeDef",
+    "PutBucketLifecycleRequestRequestTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
     "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationUnionTypeDef",
     "SelectObjectContentOutputTypeDef",
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
-    "IntelligentTieringConfigurationUnionTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
     "BucketLifecycleConfigurationTypeDef",
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     "GetBucketMetricsConfigurationOutputTypeDef",
     "ListBucketMetricsConfigurationsOutputTypeDef",
-    "MetricsConfigurationUnionTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
-    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
-    "PutBucketLifecycleRequestRequestTypeDef",
+    "NotificationConfigurationBucketNotificationTypeDef",
     "NotificationConfigurationResponseTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
-    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
-    "AnalyticsConfigurationUnionTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
     "GetBucketInventoryConfigurationOutputTypeDef",
     "ListBucketInventoryConfigurationsOutputTypeDef",
-    "InventoryConfigurationUnionTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
@@ -557,23 +536,14 @@
     "AccelerateConfigurationTypeDef",
     {
         "Status": BucketAccelerateStatusType,
     },
     total=False,
 )
 
-OwnerTypeDef = TypedDict(
-    "OwnerTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-    },
-    total=False,
-)
-
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
@@ -683,57 +653,59 @@
 
 class BucketUploadFileRequestTypeDef(
     _RequiredBucketUploadFileRequestTypeDef, _OptionalBucketUploadFileRequestTypeDef
 ):
     pass
 
 
-_RequiredCORSRuleTypeDef = TypedDict(
-    "_RequiredCORSRuleTypeDef",
+_RequiredCORSRuleBucketCorsTypeDef = TypedDict(
+    "_RequiredCORSRuleBucketCorsTypeDef",
     {
         "AllowedMethods": Sequence[str],
         "AllowedOrigins": Sequence[str],
     },
 )
-_OptionalCORSRuleTypeDef = TypedDict(
-    "_OptionalCORSRuleTypeDef",
+_OptionalCORSRuleBucketCorsTypeDef = TypedDict(
+    "_OptionalCORSRuleBucketCorsTypeDef",
     {
         "ID": str,
         "AllowedHeaders": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAgeSeconds": int,
     },
     total=False,
 )
 
 
-class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
+class CORSRuleBucketCorsTypeDef(
+    _RequiredCORSRuleBucketCorsTypeDef, _OptionalCORSRuleBucketCorsTypeDef
+):
     pass
 
 
-_RequiredCORSRuleOutputTypeDef = TypedDict(
-    "_RequiredCORSRuleOutputTypeDef",
+_RequiredCORSRuleTypeDef = TypedDict(
+    "_RequiredCORSRuleTypeDef",
     {
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
     },
 )
-_OptionalCORSRuleOutputTypeDef = TypedDict(
-    "_OptionalCORSRuleOutputTypeDef",
+_OptionalCORSRuleTypeDef = TypedDict(
+    "_OptionalCORSRuleTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
     },
     total=False,
 )
 
 
-class CORSRuleOutputTypeDef(_RequiredCORSRuleOutputTypeDef, _OptionalCORSRuleOutputTypeDef):
+class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
     pass
 
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
@@ -841,32 +813,20 @@
 
 class ClientUploadFileRequestTypeDef(
     _RequiredClientUploadFileRequestTypeDef, _OptionalClientUploadFileRequestTypeDef
 ):
     pass
 
 
-CloudFunctionConfigurationOutputTypeDef = TypedDict(
-    "CloudFunctionConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "Event": EventType,
-        "Events": List[EventType],
-        "CloudFunction": str,
-        "InvocationRole": str,
-    },
-    total=False,
-)
-
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
     total=False,
 )
 
 CommonPrefixTypeDef = TypedDict(
@@ -2080,16 +2040,16 @@
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-ObjectLockRetentionOutputTypeDef = TypedDict(
-    "ObjectLockRetentionOutputTypeDef",
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
     total=False,
 )
 
@@ -2307,16 +2267,16 @@
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": str,
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
@@ -2336,16 +2296,16 @@
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
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
@@ -2493,14 +2453,15 @@
         "EncodingType": Literal["url"],
         "KeyMarker": str,
         "MaxKeys": int,
         "Prefix": str,
         "VersionIdMarker": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
@@ -2521,14 +2482,15 @@
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Marker": str,
         "MaxKeys": int,
         "Prefix": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
@@ -2550,14 +2512,15 @@
         "MaxKeys": int,
         "Prefix": str,
         "ContinuationToken": str,
         "FetchOwner": bool,
         "StartAfter": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
@@ -2622,52 +2585,30 @@
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
 
-QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "QueueConfigurationDeprecatedOutputTypeDef",
-    {
-        "Id": str,
-        "Event": EventType,
-        "Events": List[EventType],
-        "Queue": str,
-    },
-    total=False,
-)
-
-TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "TopicConfigurationDeprecatedOutputTypeDef",
-    {
-        "Id": str,
-        "Events": List[EventType],
-        "Event": EventType,
-        "Topic": str,
-    },
-    total=False,
-)
-
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Queue": str,
     },
     total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Event": EventType,
         "Topic": str,
     },
     total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
@@ -3146,14 +3087,23 @@
     {
         "DisplayName": str,
         "ID": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OwnerTypeDef = TypedDict(
+    "OwnerTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutObjectAclOutputTypeDef = TypedDict(
     "PutObjectAclOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3225,14 +3175,32 @@
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RestoreStatusResponseTypeDef = TypedDict(
+    "RestoreStatusResponseTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusTypeDef = TypedDict(
+    "RestoreStatusTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UploadPartOutputTypeDef = TypedDict(
     "UploadPartOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3267,70 +3235,19 @@
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteMarkerEntryTypeDef = TypedDict(
-    "DeleteMarkerEntryTypeDef",
-    {
-        "Owner": OwnerTypeDef,
-        "Key": str,
-        "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
-    },
-    total=False,
-)
-
-ObjectTypeDef = TypedDict(
-    "ObjectTypeDef",
-    {
-        "Key": str,
-        "LastModified": datetime,
-        "ETag": str,
-        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
-        "Size": int,
-        "StorageClass": ObjectStorageClassType,
-        "Owner": OwnerTypeDef,
-    },
-    total=False,
-)
-
-ObjectVersionTypeDef = TypedDict(
-    "ObjectVersionTypeDef",
-    {
-        "ETag": str,
-        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
-        "Size": int,
-        "StorageClass": Literal["STANDARD"],
-        "Key": str,
-        "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
-        "Owner": OwnerTypeDef,
-    },
-    total=False,
-)
-
-AnalyticsAndOperatorOutputTypeDef = TypedDict(
-    "AnalyticsAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
@@ -3344,88 +3261,60 @@
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
-    "IntelligentTieringAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
+LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
-MetricsAndOperatorOutputTypeDef = TypedDict(
-    "MetricsAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-        "AccessPointArn": str,
-    },
-    total=False,
-)
-
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
-        "AccessPointArn": str,
-    },
-    total=False,
-)
-
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
         "Tags": List[TagTypeDef],
+        "AccessPointArn": str,
     },
     total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
@@ -3712,34 +3601,32 @@
 
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
 
-ListBucketsOutputTypeDef = TypedDict(
-    "ListBucketsOutputTypeDef",
+CORSConfigurationBucketCorsTypeDef = TypedDict(
+    "CORSConfigurationBucketCorsTypeDef",
     {
-        "Buckets": List[BucketTypeDef],
-        "Owner": OwnerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CORSRules": Sequence[CORSRuleBucketCorsTypeDef],
     },
 )
 
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleOutputTypeDef],
+        "CORSRules": List[CORSRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
@@ -4169,29 +4056,30 @@
 
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
+LifecycleExpirationBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
     {
         "Date": TimestampTypeDef,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+LifecycleExpirationBucketLifecycleTypeDef = TypedDict(
+    "LifecycleExpirationBucketLifecycleTypeDef",
     {
-        "Mode": ObjectLockRetentionModeType,
-        "RetainUntilDate": TimestampTypeDef,
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
@@ -4383,16 +4271,26 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
+TransitionBucketLifecycleConfigurationTypeDef = TypedDict(
+    "TransitionBucketLifecycleConfigurationTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
+TransitionBucketLifecycleTypeDef = TypedDict(
+    "TransitionBucketLifecycleTypeDef",
     {
         "Date": TimestampTypeDef,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
@@ -4580,26 +4478,26 @@
 )
 
 
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
 
-S3KeyFilterOutputTypeDef = TypedDict(
-    "S3KeyFilterOutputTypeDef",
+S3KeyFilterBucketNotificationTypeDef = TypedDict(
+    "S3KeyFilterBucketNotificationTypeDef",
     {
-        "FilterRules": List[FilterRuleTypeDef],
+        "FilterRules": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": Sequence[FilterRuleTypeDef],
+        "FilterRules": List[FilterRuleTypeDef],
     },
     total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
@@ -4656,19 +4554,48 @@
 ):
     pass
 
 
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionOutputTypeDef,
+        "Retention": ObjectLockRetentionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Retention": ObjectLockRetentionTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "BypassGovernanceRetention": bool,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+
+class PutObjectRetentionRequestRequestTypeDef(
+    _RequiredPutObjectRetentionRequestRequestTypeDef,
+    _OptionalPutObjectRetentionRequestRequestTypeDef,
+):
+    pass
+
+
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4830,88 +4757,65 @@
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
 
-MultipartUploadTypeDef = TypedDict(
-    "MultipartUploadTypeDef",
-    {
-        "UploadId": str,
-        "Key": str,
-        "Initiated": datetime,
-        "StorageClass": StorageClassType,
-        "Owner": OwnerTypeDef,
-        "Initiator": InitiatorTypeDef,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-    },
-    total=False,
-)
-
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "CSV": CSVInputTypeDef,
         "CompressionType": CompressionTypeType,
         "JSON": JSONInputTypeDef,
         "Parquet": Mapping[str, Any],
     },
     total=False,
 )
 
-InventoryEncryptionOutputTypeDef = TypedDict(
-    "InventoryEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSTypeDef,
-    },
-    total=False,
-)
-
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": Mapping[str, Any],
+        "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
+_RequiredRuleTypeDef = TypedDict(
+    "_RequiredRuleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
     },
 )
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
+_OptionalRuleTypeDef = TypedDict(
+    "_OptionalRuleTypeDef",
     {
-        "Expiration": LifecycleExpirationOutputTypeDef,
+        "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
-        "Transition": TransitionOutputTypeDef,
+        "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
 
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
 _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     {
         "Bucket": str,
@@ -4948,14 +4852,15 @@
     "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     {
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
@@ -4975,14 +4880,15 @@
     "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
     {
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListObjectsRequestListObjectsPaginateTypeDef(
@@ -5004,14 +4910,15 @@
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "FetchOwner": bool,
         "StartAfter": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
@@ -5046,36 +4953,14 @@
 class ListPartsRequestListPartsPaginateTypeDef(
     _RequiredListPartsRequestListPartsPaginateTypeDef,
     _OptionalListPartsRequestListPartsPaginateTypeDef,
 ):
     pass
 
 
-ListPartsOutputTypeDef = TypedDict(
-    "ListPartsOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "PartNumberMarker": int,
-        "NextPartNumberMarker": int,
-        "MaxParts": int,
-        "IsTruncated": bool,
-        "Parts": List[PartTypeDef],
-        "Initiator": InitiatorTypeDef,
-        "Owner": OwnerTypeDef,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
     },
 )
 _OptionalMetricsTypeDef = TypedDict(
@@ -5098,42 +4983,35 @@
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedResponseTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-OwnershipControlsOutputTypeDef = TypedDict(
-    "OwnershipControlsOutputTypeDef",
-    {
-        "Rules": List[OwnershipControlsRuleTypeDef],
-    },
-)
-
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": Sequence[OwnershipControlsRuleTypeDef],
+        "Rules": List[OwnershipControlsRuleTypeDef],
     },
 )
 
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": ProgressTypeDef,
@@ -5278,121 +5156,131 @@
     "StatsEventTypeDef",
     {
         "Details": StatsTypeDef,
     },
     total=False,
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+DeleteMarkerEntryTypeDef = TypedDict(
+    "DeleteMarkerEntryTypeDef",
     {
-        "IsTruncated": bool,
-        "Marker": str,
-        "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Owner": OwnerTypeDef,
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
     },
+    total=False,
 )
 
-ListObjectsV2OutputTypeDef = TypedDict(
-    "ListObjectsV2OutputTypeDef",
+ListBucketsOutputTypeDef = TypedDict(
+    "ListBucketsOutputTypeDef",
     {
-        "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "KeyCount": int,
-        "ContinuationToken": str,
-        "NextContinuationToken": str,
-        "StartAfter": str,
-        "RequestCharged": Literal["requester"],
+        "Buckets": List[BucketTypeDef],
+        "Owner": OwnerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectVersionsOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputTypeDef",
+ListPartsOutputTypeDef = TypedDict(
+    "ListPartsOutputTypeDef",
     {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "PartNumberMarker": int,
+        "NextPartNumberMarker": int,
+        "MaxParts": int,
         "IsTruncated": bool,
-        "KeyMarker": str,
-        "VersionIdMarker": str,
-        "NextKeyMarker": str,
-        "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
+        "Parts": List[PartTypeDef],
+        "Initiator": InitiatorTypeDef,
+        "Owner": OwnerTypeDef,
+        "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalyticsFilterOutputTypeDef = TypedDict(
-    "AnalyticsFilterOutputTypeDef",
+MultipartUploadTypeDef = TypedDict(
+    "MultipartUploadTypeDef",
     {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": AnalyticsAndOperatorOutputTypeDef,
+        "UploadId": str,
+        "Key": str,
+        "Initiated": datetime,
+        "StorageClass": StorageClassType,
+        "Owner": OwnerTypeDef,
+        "Initiator": InitiatorTypeDef,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-AnalyticsFilterTypeDef = TypedDict(
-    "AnalyticsFilterTypeDef",
+ObjectTypeDef = TypedDict(
+    "ObjectTypeDef",
     {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": AnalyticsAndOperatorTypeDef,
+        "Key": str,
+        "LastModified": datetime,
+        "ETag": str,
+        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
+        "Size": int,
+        "StorageClass": ObjectStorageClassType,
+        "Owner": OwnerTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
+    },
+    total=False,
+)
+
+ObjectVersionTypeDef = TypedDict(
+    "ObjectVersionTypeDef",
+    {
+        "ETag": str,
+        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
+        "Size": int,
+        "StorageClass": Literal["STANDARD"],
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
+        "Owner": OwnerTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
     total=False,
 )
 
-IntelligentTieringFilterOutputTypeDef = TypedDict(
-    "IntelligentTieringFilterOutputTypeDef",
+AnalyticsFilterTypeDef = TypedDict(
+    "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
-        "And": IntelligentTieringAndOperatorOutputTypeDef,
+        "And": AnalyticsAndOperatorTypeDef,
     },
     total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
     total=False,
 )
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
+LifecycleRuleFilterBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "And": LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef,
     },
     total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
@@ -5401,46 +5289,25 @@
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
     total=False,
 )
 
-MetricsFilterOutputTypeDef = TypedDict(
-    "MetricsFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "AccessPointArn": str,
-        "And": MetricsAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
     total=False,
 )
 
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -5660,15 +5527,15 @@
 ):
     pass
 
 
 _RequiredPutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "_RequiredPutBucketCorsRequestBucketCorsPutTypeDef",
     {
-        "CORSConfiguration": CORSConfigurationTypeDef,
+        "CORSConfiguration": CORSConfigurationBucketCorsTypeDef,
     },
 )
 _OptionalPutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "_OptionalPutBucketCorsRequestBucketCorsPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
@@ -5753,68 +5620,38 @@
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
 
-ObjectLockRetentionUnionTypeDef = Union[
-    ObjectLockRetentionTypeDef, ObjectLockRetentionOutputTypeDef
-]
-_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Retention": ObjectLockRetentionTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "BypassGovernanceRetention": bool,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-
-class PutObjectRetentionRequestRequestTypeDef(
-    _RequiredPutObjectRetentionRequestRequestTypeDef,
-    _OptionalPutObjectRetentionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
+_RequiredRuleBucketLifecycleTypeDef = TypedDict(
+    "_RequiredRuleBucketLifecycleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
     },
 )
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
+_OptionalRuleBucketLifecycleTypeDef = TypedDict(
+    "_OptionalRuleBucketLifecycleTypeDef",
     {
-        "Expiration": LifecycleExpirationTypeDef,
+        "Expiration": LifecycleExpirationBucketLifecycleTypeDef,
         "ID": str,
-        "Transition": TransitionTypeDef,
+        "Transition": TransitionBucketLifecycleTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
 
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+class RuleBucketLifecycleTypeDef(
+    _RequiredRuleBucketLifecycleTypeDef, _OptionalRuleBucketLifecycleTypeDef
+):
     pass
 
 
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
@@ -5871,18 +5708,18 @@
 
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
 
-NotificationConfigurationFilterOutputTypeDef = TypedDict(
-    "NotificationConfigurationFilterOutputTypeDef",
+NotificationConfigurationFilterBucketNotificationTypeDef = TypedDict(
+    "NotificationConfigurationFilterBucketNotificationTypeDef",
     {
-        "Key": S3KeyFilterOutputTypeDef,
+        "Key": S3KeyFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
@@ -5956,88 +5793,63 @@
 )
 
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
 
-_RequiredLoggingEnabledOutputTypeDef = TypedDict(
-    "_RequiredLoggingEnabledOutputTypeDef",
+_RequiredLoggingEnabledBucketLoggingTypeDef = TypedDict(
+    "_RequiredLoggingEnabledBucketLoggingTypeDef",
     {
         "TargetBucket": str,
         "TargetPrefix": str,
     },
 )
-_OptionalLoggingEnabledOutputTypeDef = TypedDict(
-    "_OptionalLoggingEnabledOutputTypeDef",
+_OptionalLoggingEnabledBucketLoggingTypeDef = TypedDict(
+    "_OptionalLoggingEnabledBucketLoggingTypeDef",
     {
-        "TargetGrants": List[TargetGrantTypeDef],
+        "TargetGrants": Sequence[TargetGrantTypeDef],
     },
     total=False,
 )
 
 
-class LoggingEnabledOutputTypeDef(
-    _RequiredLoggingEnabledOutputTypeDef, _OptionalLoggingEnabledOutputTypeDef
+class LoggingEnabledBucketLoggingTypeDef(
+    _RequiredLoggingEnabledBucketLoggingTypeDef, _OptionalLoggingEnabledBucketLoggingTypeDef
 ):
     pass
 
 
-LoggingEnabledTypeDef = TypedDict(
-    "LoggingEnabledTypeDef",
+LoggingEnabledResponseTypeDef = TypedDict(
+    "LoggingEnabledResponseTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListMultipartUploadsOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputTypeDef",
+_RequiredLoggingEnabledTypeDef = TypedDict(
+    "_RequiredLoggingEnabledTypeDef",
     {
-        "Bucket": str,
-        "KeyMarker": str,
-        "UploadIdMarker": str,
-        "NextKeyMarker": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "NextUploadIdMarker": str,
-        "MaxUploads": int,
-        "IsTruncated": bool,
-        "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredInventoryS3BucketDestinationOutputTypeDef = TypedDict(
-    "_RequiredInventoryS3BucketDestinationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Format": InventoryFormatType,
+        "TargetBucket": str,
+        "TargetPrefix": str,
     },
 )
-_OptionalInventoryS3BucketDestinationOutputTypeDef = TypedDict(
-    "_OptionalInventoryS3BucketDestinationOutputTypeDef",
+_OptionalLoggingEnabledTypeDef = TypedDict(
+    "_OptionalLoggingEnabledTypeDef",
     {
-        "AccountId": str,
-        "Prefix": str,
-        "Encryption": InventoryEncryptionOutputTypeDef,
+        "TargetGrants": List[TargetGrantTypeDef],
     },
     total=False,
 )
 
 
-class InventoryS3BucketDestinationOutputTypeDef(
-    _RequiredInventoryS3BucketDestinationOutputTypeDef,
-    _OptionalInventoryS3BucketDestinationOutputTypeDef,
-):
+class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
     pass
 
 
 _RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
     "_RequiredInventoryS3BucketDestinationTypeDef",
     {
         "Bucket": str,
@@ -6102,19 +5914,26 @@
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
+    {
+        "Rules": Sequence[RuleTypeDef],
+    },
+)
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -6158,20 +5977,19 @@
 ):
     pass
 
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsOutputTypeDef,
+        "OwnershipControls": OwnershipControlsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OwnershipControlsUnionTypeDef = Union[OwnershipControlsTypeDef, OwnershipControlsOutputTypeDef]
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
         "OwnershipControls": OwnershipControlsTypeDef,
     },
 )
@@ -6210,25 +6028,18 @@
         "IndexDocument": IndexDocumentTypeDef,
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "RoutingRules": Sequence[RoutingRuleTypeDef],
     },
     total=False,
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
-    },
-)
-
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
+        "Rules": List[ServerSideEncryptionRuleTypeDef],
     },
 )
 
 SelectObjectContentEventStreamTypeDef = TypedDict(
     "SelectObjectContentEventStreamTypeDef",
     {
         "Records": RecordsEventTypeDef,
@@ -6236,44 +6047,99 @@
         "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
     total=False,
 )
 
-_RequiredIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIntelligentTieringConfigurationOutputTypeDef",
+ListMultipartUploadsOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputTypeDef",
     {
-        "Id": str,
-        "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Bucket": str,
+        "KeyMarker": str,
+        "UploadIdMarker": str,
+        "NextKeyMarker": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "NextUploadIdMarker": str,
+        "MaxUploads": int,
+        "IsTruncated": bool,
+        "Uploads": List[MultipartUploadTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIntelligentTieringConfigurationOutputTypeDef",
+
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
     {
-        "Filter": IntelligentTieringFilterOutputTypeDef,
+        "IsTruncated": bool,
+        "Marker": str,
+        "NextMarker": str,
+        "Contents": List[ObjectTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListObjectsV2OutputTypeDef = TypedDict(
+    "ListObjectsV2OutputTypeDef",
+    {
+        "IsTruncated": bool,
+        "Contents": List[ObjectTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "KeyCount": int,
+        "ContinuationToken": str,
+        "NextContinuationToken": str,
+        "StartAfter": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class IntelligentTieringConfigurationOutputTypeDef(
-    _RequiredIntelligentTieringConfigurationOutputTypeDef,
-    _OptionalIntelligentTieringConfigurationOutputTypeDef,
-):
-    pass
-
+ListObjectVersionsOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputTypeDef",
+    {
+        "IsTruncated": bool,
+        "KeyMarker": str,
+        "VersionIdMarker": str,
+        "NextKeyMarker": str,
+        "NextVersionIdMarker": str,
+        "Versions": List[ObjectVersionTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
     "_RequiredIntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
         "Status": IntelligentTieringStatusType,
-        "Tierings": Sequence[TieringTypeDef],
+        "Tierings": List[TieringTypeDef],
     },
 )
 _OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
     "_OptionalIntelligentTieringConfigurationTypeDef",
     {
         "Filter": IntelligentTieringFilterTypeDef,
     },
@@ -6283,38 +6149,39 @@
 
 class IntelligentTieringConfigurationTypeDef(
     _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
 ):
     pass
 
 
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
+_RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
+    "_RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
+_OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
+    "_OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef",
     {
-        "Expiration": LifecycleExpirationOutputTypeDef,
+        "Expiration": LifecycleExpirationBucketLifecycleConfigurationTypeDef,
         "ID": str,
         "Prefix": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Filter": LifecycleRuleFilterBucketLifecycleConfigurationTypeDef,
+        "Transitions": Sequence[TransitionBucketLifecycleConfigurationTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
 
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+class LifecycleRuleBucketLifecycleConfigurationTypeDef(
+    _RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef,
+    _OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef,
 ):
     pass
 
 
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
@@ -6324,48 +6191,27 @@
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
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
 
 
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
 
-_RequiredMetricsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMetricsConfigurationOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalMetricsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMetricsConfigurationOutputTypeDef",
-    {
-        "Filter": MetricsFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MetricsConfigurationOutputTypeDef(
-    _RequiredMetricsConfigurationOutputTypeDef, _OptionalMetricsConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricsConfigurationTypeDef = TypedDict(
     "_RequiredMetricsConfigurationTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricsConfigurationTypeDef = TypedDict(
@@ -6387,18 +6233,18 @@
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
     total=False,
 )
 
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
+LifecycleConfigurationBucketLifecycleTypeDef = TypedDict(
+    "LifecycleConfigurationBucketLifecycleTypeDef",
     {
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleBucketLifecycleTypeDef],
     },
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
@@ -6429,89 +6275,91 @@
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLambdaFunctionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionConfigurationOutputTypeDef",
+_RequiredLambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredLambdaFunctionConfigurationBucketNotificationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalLambdaFunctionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionConfigurationOutputTypeDef",
+_OptionalLambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalLambdaFunctionConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
 
-class LambdaFunctionConfigurationOutputTypeDef(
-    _RequiredLambdaFunctionConfigurationOutputTypeDef,
-    _OptionalLambdaFunctionConfigurationOutputTypeDef,
+class LambdaFunctionConfigurationBucketNotificationTypeDef(
+    _RequiredLambdaFunctionConfigurationBucketNotificationTypeDef,
+    _OptionalLambdaFunctionConfigurationBucketNotificationTypeDef,
 ):
     pass
 
 
-_RequiredQueueConfigurationOutputTypeDef = TypedDict(
-    "_RequiredQueueConfigurationOutputTypeDef",
+_RequiredQueueConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredQueueConfigurationBucketNotificationTypeDef",
     {
         "QueueArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalQueueConfigurationOutputTypeDef = TypedDict(
-    "_OptionalQueueConfigurationOutputTypeDef",
+_OptionalQueueConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalQueueConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
 
-class QueueConfigurationOutputTypeDef(
-    _RequiredQueueConfigurationOutputTypeDef, _OptionalQueueConfigurationOutputTypeDef
+class QueueConfigurationBucketNotificationTypeDef(
+    _RequiredQueueConfigurationBucketNotificationTypeDef,
+    _OptionalQueueConfigurationBucketNotificationTypeDef,
 ):
     pass
 
 
-_RequiredTopicConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTopicConfigurationOutputTypeDef",
+_RequiredTopicConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredTopicConfigurationBucketNotificationTypeDef",
     {
         "TopicArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalTopicConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTopicConfigurationOutputTypeDef",
+_OptionalTopicConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalTopicConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
 
-class TopicConfigurationOutputTypeDef(
-    _RequiredTopicConfigurationOutputTypeDef, _OptionalTopicConfigurationOutputTypeDef
+class TopicConfigurationBucketNotificationTypeDef(
+    _RequiredTopicConfigurationBucketNotificationTypeDef,
+    _OptionalTopicConfigurationBucketNotificationTypeDef,
 ):
     pass
 
 
 _RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
     "_RequiredLambdaFunctionConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
     "_OptionalLambdaFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6526,15 +6374,15 @@
     pass
 
 
 _RequiredQueueConfigurationTypeDef = TypedDict(
     "_RequiredQueueConfigurationTypeDef",
     {
         "QueueArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalQueueConfigurationTypeDef = TypedDict(
     "_OptionalQueueConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6549,15 +6397,15 @@
     pass
 
 
 _RequiredTopicConfigurationTypeDef = TypedDict(
     "_RequiredTopicConfigurationTypeDef",
     {
         "TopicArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalTopicConfigurationTypeDef = TypedDict(
     "_OptionalTopicConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6671,68 +6519,65 @@
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
     },
     total=False,
 )
 
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
+BucketLoggingStatusBucketLoggingTypeDef = TypedDict(
+    "BucketLoggingStatusBucketLoggingTypeDef",
     {
-        "LoggingEnabled": LoggingEnabledOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoggingEnabled": LoggingEnabledBucketLoggingTypeDef,
     },
+    total=False,
 )
 
 BucketLoggingStatusTypeDef = TypedDict(
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
     },
     total=False,
 )
 
-InventoryDestinationOutputTypeDef = TypedDict(
-    "InventoryDestinationOutputTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
-        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
+        "LoggingEnabled": LoggingEnabledTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
     },
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
+_RequiredPutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutBucketLifecycleRequestRequestTypeDef",
     {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
+        "Bucket": str,
     },
 )
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
+_OptionalPutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutBucketLifecycleRequestRequestTypeDef",
     {
-        "ID": str,
-        "Priority": int,
-        "Prefix": str,
-        "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
+        "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
 
-class ReplicationRuleOutputTypeDef(
-    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+class PutBucketLifecycleRequestRequestTypeDef(
+    _RequiredPutBucketLifecycleRequestRequestTypeDef,
+    _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
@@ -6804,15 +6649,15 @@
 ):
     pass
 
 
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
@@ -6834,93 +6679,91 @@
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
 
-ServerSideEncryptionConfigurationUnionTypeDef = Union[
-    ServerSideEncryptionConfigurationTypeDef, ServerSideEncryptionConfigurationOutputTypeDef
-]
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "AioEventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntelligentTieringConfigurationUnionTypeDef = Union[
-    IntelligentTieringConfigurationTypeDef, IntelligentTieringConfigurationOutputTypeDef
-]
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
 
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = TypedDict(
+    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
     {
-        "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Rules": Sequence[LifecycleRuleBucketLifecycleConfigurationTypeDef],
     },
 )
 
 BucketLifecycleConfigurationTypeDef = TypedDict(
     "BucketLifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
 
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
+    {
+        "Rules": List[LifecycleRuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "MetricsConfiguration": MetricsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
+        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricsConfigurationUnionTypeDef = Union[
-    MetricsConfigurationTypeDef, MetricsConfigurationOutputTypeDef
-]
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "MetricsConfiguration": MetricsConfigurationTypeDef,
     },
@@ -6937,36 +6780,14 @@
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAnalyticsConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
-    },
-)
-_OptionalAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAnalyticsConfigurationOutputTypeDef",
-    {
-        "Filter": AnalyticsFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AnalyticsConfigurationOutputTypeDef(
-    _RequiredAnalyticsConfigurationOutputTypeDef, _OptionalAnalyticsConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredAnalyticsConfigurationTypeDef = TypedDict(
     "_RequiredAnalyticsConfigurationTypeDef",
     {
         "Id": str,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
 )
@@ -6985,50 +6806,39 @@
     pass
 
 
 PutBucketLifecycleRequestBucketLifecyclePutTypeDef = TypedDict(
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
+        "LifecycleConfiguration": LifecycleConfigurationBucketLifecycleTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-_RequiredPutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutBucketLifecycleRequestRequestTypeDef",
+NotificationConfigurationBucketNotificationTypeDef = TypedDict(
+    "NotificationConfigurationBucketNotificationTypeDef",
     {
-        "Bucket": str,
-    },
-)
-_OptionalPutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutBucketLifecycleRequestRequestTypeDef",
-    {
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
-        "ExpectedBucketOwner": str,
+        "TopicConfigurations": Sequence[TopicConfigurationBucketNotificationTypeDef],
+        "QueueConfigurations": Sequence[QueueConfigurationBucketNotificationTypeDef],
+        "LambdaFunctionConfigurations": Sequence[
+            LambdaFunctionConfigurationBucketNotificationTypeDef
+        ],
+        "EventBridgeConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
-
-class PutBucketLifecycleRequestRequestTypeDef(
-    _RequiredPutBucketLifecycleRequestRequestTypeDef,
-    _OptionalPutBucketLifecycleRequestRequestTypeDef,
-):
-    pass
-
-
 NotificationConfigurationResponseTypeDef = TypedDict(
     "NotificationConfigurationResponseTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
-        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
+        "TopicConfigurations": List[TopicConfigurationTypeDef],
+        "QueueConfigurations": List[QueueConfigurationTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
@@ -7054,15 +6864,15 @@
     },
     total=False,
 )
 
 _RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "_RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
-        "BucketLoggingStatus": BucketLoggingStatusTypeDef,
+        "BucketLoggingStatus": BucketLoggingStatusBucketLoggingTypeDef,
     },
 )
 _OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "_OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
@@ -7097,87 +6907,53 @@
 
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredInventoryConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInventoryConfigurationOutputTypeDef",
-    {
-        "Destination": InventoryDestinationOutputTypeDef,
-        "IsEnabled": bool,
-        "Id": str,
-        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
-        "Schedule": InventoryScheduleTypeDef,
-    },
-)
-_OptionalInventoryConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInventoryConfigurationOutputTypeDef",
-    {
-        "Filter": InventoryFilterTypeDef,
-        "OptionalFields": List[InventoryOptionalFieldType],
-    },
-    total=False,
-)
-
-
-class InventoryConfigurationOutputTypeDef(
-    _RequiredInventoryConfigurationOutputTypeDef, _OptionalInventoryConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredInventoryConfigurationTypeDef = TypedDict(
     "_RequiredInventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
     },
 )
 _OptionalInventoryConfigurationTypeDef = TypedDict(
     "_OptionalInventoryConfigurationTypeDef",
     {
         "Filter": InventoryFilterTypeDef,
-        "OptionalFields": Sequence[InventoryOptionalFieldType],
+        "OptionalFields": List[InventoryOptionalFieldType],
     },
     total=False,
 )
 
 
 class InventoryConfigurationTypeDef(
     _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
 ):
     pass
 
 
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
 
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": BucketLifecycleConfigurationTypeDef,
+        "LifecycleConfiguration": BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
 _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef",
@@ -7202,33 +6978,30 @@
 ):
     pass
 
 
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalyticsConfigurationUnionTypeDef = Union[
-    AnalyticsConfigurationTypeDef, AnalyticsConfigurationOutputTypeDef
-]
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
     },
@@ -7248,15 +7021,15 @@
 ):
     pass
 
 
 _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationBucketNotificationTypeDef,
     },
 )
 _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
@@ -7345,33 +7118,30 @@
 ):
     pass
 
 
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
+        "InventoryConfiguration": InventoryConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InventoryConfigurationUnionTypeDef = Union[
-    InventoryConfigurationTypeDef, InventoryConfigurationOutputTypeDef
-]
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "InventoryConfiguration": InventoryConfigurationTypeDef,
     },
@@ -7391,15 +7161,15 @@
 ):
     pass
 
 
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
@@ -7419,12 +7189,7 @@
 
 
 class PutBucketReplicationRequestRequestTypeDef(
     _RequiredPutBucketReplicationRequestRequestTypeDef,
     _OptionalPutBucketReplicationRequestRequestTypeDef,
 ):
     pass
-
-
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/type_defs.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -84,33 +84,31 @@
 
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
     "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
-    "OwnerTypeDef",
     "AccessControlTranslationTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "BlobTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "FileobjTypeDef",
     "BucketTypeDef",
     "BucketUploadFileRequestTypeDef",
+    "CORSRuleBucketCorsTypeDef",
     "CORSRuleTypeDef",
-    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "ChecksumTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
-    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "TimestampTypeDef",
     "CopyPartResultTypeDef",
@@ -177,15 +175,15 @@
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "ObjectLockRetentionOutputTypeDef",
+    "ObjectLockRetentionTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
@@ -194,33 +192,31 @@
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
-    "LifecycleExpirationOutputTypeDef",
+    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
-    "TransitionOutputTypeDef",
+    "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
-    "QueueConfigurationDeprecatedOutputTypeDef",
-    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "OwnershipControlsRuleTypeDef",
     "ProgressTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
@@ -252,38 +248,34 @@
     "GetBucketVersioningOutputTypeDef",
     "GetObjectOutputTypeDef",
     "GetObjectTorrentOutputTypeDef",
     "HeadObjectOutputTypeDef",
     "IndexDocumentResponseTypeDef",
     "InitiatorResponseTypeDef",
     "OwnerResponseTypeDef",
+    "OwnerTypeDef",
     "PutObjectAclOutputTypeDef",
     "PutObjectLegalHoldOutputTypeDef",
     "PutObjectLockConfigurationOutputTypeDef",
     "PutObjectOutputTypeDef",
     "PutObjectRetentionOutputTypeDef",
     "PutObjectTaggingOutputTypeDef",
     "RedirectAllRequestsToResponseTypeDef",
     "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseTypeDef",
+    "RestoreStatusTypeDef",
     "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
-    "DeleteMarkerEntryTypeDef",
-    "ObjectTypeDef",
-    "ObjectVersionTypeDef",
-    "AnalyticsAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
-    "IntelligentTieringAndOperatorOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
-    "LifecycleRuleAndOperatorOutputTypeDef",
+    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
-    "MetricsAndOperatorOutputTypeDef",
     "MetricsAndOperatorTypeDef",
-    "ReplicationRuleAndOperatorOutputTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
@@ -291,15 +283,15 @@
     "ObjectCopyRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "ListBucketsOutputTypeDef",
+    "CORSConfigurationBucketCorsTypeDef",
     "CORSConfigurationTypeDef",
     "GetBucketCorsOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
     "CopyObjectOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
@@ -307,200 +299,187 @@
     "CreateMultipartUploadRequestRequestTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "LifecycleExpirationTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
+    "LifecycleExpirationBucketLifecycleTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "TransitionTypeDef",
+    "TransitionBucketLifecycleConfigurationTypeDef",
+    "TransitionBucketLifecycleTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "UploadPartCopyOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
     "ObjectLockRuleTypeDef",
     "DeleteObjectsOutputTypeDef",
     "DeleteTypeDef",
-    "S3KeyFilterOutputTypeDef",
+    "S3KeyFilterBucketNotificationTypeDef",
     "S3KeyFilterTypeDef",
     "GetBucketPolicyStatusOutputTypeDef",
     "GetObjectAttributesPartsTypeDef",
     "GetObjectLegalHoldOutputTypeDef",
     "PutObjectLegalHoldRequestRequestTypeDef",
     "GetObjectRetentionOutputTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
-    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
-    "RuleOutputTypeDef",
+    "RuleTypeDef",
     "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
-    "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
-    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
     "ProgressEventTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "RoutingRuleTypeDef",
     "ServerSideEncryptionRuleTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "StatsEventTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListObjectsV2OutputTypeDef",
-    "ListObjectVersionsOutputTypeDef",
-    "AnalyticsFilterOutputTypeDef",
+    "DeleteMarkerEntryTypeDef",
+    "ListBucketsOutputTypeDef",
+    "ListPartsOutputTypeDef",
+    "MultipartUploadTypeDef",
+    "ObjectTypeDef",
+    "ObjectVersionTypeDef",
     "AnalyticsFilterTypeDef",
-    "IntelligentTieringFilterOutputTypeDef",
     "IntelligentTieringFilterTypeDef",
-    "LifecycleRuleFilterOutputTypeDef",
+    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleFilterTypeDef",
-    "MetricsFilterOutputTypeDef",
     "MetricsFilterTypeDef",
-    "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
-    "ObjectLockRetentionUnionTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
-    "RuleTypeDef",
+    "RuleBucketLifecycleTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
-    "NotificationConfigurationFilterOutputTypeDef",
+    "NotificationConfigurationFilterBucketNotificationTypeDef",
     "NotificationConfigurationFilterTypeDef",
     "GetObjectAttributesOutputTypeDef",
     "AccessControlPolicyTypeDef",
     "GetBucketAclOutputTypeDef",
     "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
-    "LoggingEnabledOutputTypeDef",
+    "LoggingEnabledBucketLoggingTypeDef",
+    "LoggingEnabledResponseTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputTypeDef",
-    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
     "GetBucketLifecycleOutputTypeDef",
+    "LifecycleConfigurationTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
     "GetBucketOwnershipControlsOutputTypeDef",
-    "OwnershipControlsUnionTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
     "GetBucketWebsiteOutputTypeDef",
     "WebsiteConfigurationTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "SelectObjectContentEventStreamTypeDef",
-    "IntelligentTieringConfigurationOutputTypeDef",
+    "ListMultipartUploadsOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListObjectsV2OutputTypeDef",
+    "ListObjectVersionsOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
-    "LifecycleRuleOutputTypeDef",
+    "LifecycleRuleBucketLifecycleConfigurationTypeDef",
     "LifecycleRuleTypeDef",
-    "MetricsConfigurationOutputTypeDef",
     "MetricsConfigurationTypeDef",
     "StorageClassAnalysisTypeDef",
-    "LifecycleConfigurationTypeDef",
+    "LifecycleConfigurationBucketLifecycleTypeDef",
     "GetObjectLockConfigurationOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
-    "LambdaFunctionConfigurationOutputTypeDef",
-    "QueueConfigurationOutputTypeDef",
-    "TopicConfigurationOutputTypeDef",
+    "LambdaFunctionConfigurationBucketNotificationTypeDef",
+    "QueueConfigurationBucketNotificationTypeDef",
+    "TopicConfigurationBucketNotificationTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
-    "GetBucketLoggingOutputTypeDef",
+    "BucketLoggingStatusBucketLoggingTypeDef",
     "BucketLoggingStatusTypeDef",
-    "InventoryDestinationOutputTypeDef",
+    "GetBucketLoggingOutputTypeDef",
     "InventoryDestinationTypeDef",
-    "ReplicationRuleOutputTypeDef",
+    "PutBucketLifecycleRequestRequestTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
     "GetBucketEncryptionOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationUnionTypeDef",
     "SelectObjectContentOutputTypeDef",
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
-    "IntelligentTieringConfigurationUnionTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
     "BucketLifecycleConfigurationTypeDef",
+    "GetBucketLifecycleConfigurationOutputTypeDef",
     "GetBucketMetricsConfigurationOutputTypeDef",
     "ListBucketMetricsConfigurationsOutputTypeDef",
-    "MetricsConfigurationUnionTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
-    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
-    "PutBucketLifecycleRequestRequestTypeDef",
+    "NotificationConfigurationBucketNotificationTypeDef",
     "NotificationConfigurationResponseTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
-    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
-    "AnalyticsConfigurationUnionTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
     "GetBucketInventoryConfigurationOutputTypeDef",
     "ListBucketInventoryConfigurationsOutputTypeDef",
-    "InventoryConfigurationUnionTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketReplicationOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
@@ -554,23 +533,14 @@
     "AccelerateConfigurationTypeDef",
     {
         "Status": BucketAccelerateStatusType,
     },
     total=False,
 )
 
-OwnerTypeDef = TypedDict(
-    "OwnerTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-    },
-    total=False,
-)
-
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
@@ -672,54 +642,56 @@
 )
 
 class BucketUploadFileRequestTypeDef(
     _RequiredBucketUploadFileRequestTypeDef, _OptionalBucketUploadFileRequestTypeDef
 ):
     pass
 
-_RequiredCORSRuleTypeDef = TypedDict(
-    "_RequiredCORSRuleTypeDef",
+_RequiredCORSRuleBucketCorsTypeDef = TypedDict(
+    "_RequiredCORSRuleBucketCorsTypeDef",
     {
         "AllowedMethods": Sequence[str],
         "AllowedOrigins": Sequence[str],
     },
 )
-_OptionalCORSRuleTypeDef = TypedDict(
-    "_OptionalCORSRuleTypeDef",
+_OptionalCORSRuleBucketCorsTypeDef = TypedDict(
+    "_OptionalCORSRuleBucketCorsTypeDef",
     {
         "ID": str,
         "AllowedHeaders": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAgeSeconds": int,
     },
     total=False,
 )
 
-class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
+class CORSRuleBucketCorsTypeDef(
+    _RequiredCORSRuleBucketCorsTypeDef, _OptionalCORSRuleBucketCorsTypeDef
+):
     pass
 
-_RequiredCORSRuleOutputTypeDef = TypedDict(
-    "_RequiredCORSRuleOutputTypeDef",
+_RequiredCORSRuleTypeDef = TypedDict(
+    "_RequiredCORSRuleTypeDef",
     {
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
     },
 )
-_OptionalCORSRuleOutputTypeDef = TypedDict(
-    "_OptionalCORSRuleOutputTypeDef",
+_OptionalCORSRuleTypeDef = TypedDict(
+    "_OptionalCORSRuleTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
     },
     total=False,
 )
 
-class CORSRuleOutputTypeDef(_RequiredCORSRuleOutputTypeDef, _OptionalCORSRuleOutputTypeDef):
+class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
     pass
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
@@ -820,32 +792,20 @@
 )
 
 class ClientUploadFileRequestTypeDef(
     _RequiredClientUploadFileRequestTypeDef, _OptionalClientUploadFileRequestTypeDef
 ):
     pass
 
-CloudFunctionConfigurationOutputTypeDef = TypedDict(
-    "CloudFunctionConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "Event": EventType,
-        "Events": List[EventType],
-        "CloudFunction": str,
-        "InvocationRole": str,
-    },
-    total=False,
-)
-
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
     total=False,
 )
 
 CommonPrefixTypeDef = TypedDict(
@@ -1975,16 +1935,16 @@
 
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-ObjectLockRetentionOutputTypeDef = TypedDict(
-    "ObjectLockRetentionOutputTypeDef",
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
     total=False,
 )
 
@@ -2190,16 +2150,16 @@
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": str,
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
@@ -2219,16 +2179,16 @@
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
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
@@ -2366,14 +2326,15 @@
         "EncodingType": Literal["url"],
         "KeyMarker": str,
         "MaxKeys": int,
         "Prefix": str,
         "VersionIdMarker": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
     _OptionalListObjectVersionsRequestRequestTypeDef,
@@ -2392,14 +2353,15 @@
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Marker": str,
         "MaxKeys": int,
         "Prefix": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
 ):
@@ -2419,14 +2381,15 @@
         "MaxKeys": int,
         "Prefix": str,
         "ContinuationToken": str,
         "FetchOwner": bool,
         "StartAfter": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
@@ -2487,52 +2450,30 @@
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
 
-QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "QueueConfigurationDeprecatedOutputTypeDef",
-    {
-        "Id": str,
-        "Event": EventType,
-        "Events": List[EventType],
-        "Queue": str,
-    },
-    total=False,
-)
-
-TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
-    "TopicConfigurationDeprecatedOutputTypeDef",
-    {
-        "Id": str,
-        "Events": List[EventType],
-        "Event": EventType,
-        "Topic": str,
-    },
-    total=False,
-)
-
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Queue": str,
     },
     total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
         "Event": EventType,
         "Topic": str,
     },
     total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
@@ -3001,14 +2942,23 @@
     {
         "DisplayName": str,
         "ID": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OwnerTypeDef = TypedDict(
+    "OwnerTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutObjectAclOutputTypeDef = TypedDict(
     "PutObjectAclOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3080,14 +3030,32 @@
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RestoreStatusResponseTypeDef = TypedDict(
+    "RestoreStatusResponseTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusTypeDef = TypedDict(
+    "RestoreStatusTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UploadPartOutputTypeDef = TypedDict(
     "UploadPartOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3120,70 +3088,19 @@
 
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DeleteMarkerEntryTypeDef = TypedDict(
-    "DeleteMarkerEntryTypeDef",
-    {
-        "Owner": OwnerTypeDef,
-        "Key": str,
-        "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
-    },
-    total=False,
-)
-
-ObjectTypeDef = TypedDict(
-    "ObjectTypeDef",
-    {
-        "Key": str,
-        "LastModified": datetime,
-        "ETag": str,
-        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
-        "Size": int,
-        "StorageClass": ObjectStorageClassType,
-        "Owner": OwnerTypeDef,
-    },
-    total=False,
-)
-
-ObjectVersionTypeDef = TypedDict(
-    "ObjectVersionTypeDef",
-    {
-        "ETag": str,
-        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
-        "Size": int,
-        "StorageClass": Literal["STANDARD"],
-        "Key": str,
-        "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
-        "Owner": OwnerTypeDef,
-    },
-    total=False,
-)
-
-AnalyticsAndOperatorOutputTypeDef = TypedDict(
-    "AnalyticsAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
@@ -3197,88 +3114,60 @@
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
-    "IntelligentTieringAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
-    "LifecycleRuleAndOperatorOutputTypeDef",
+LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
-MetricsAndOperatorOutputTypeDef = TypedDict(
-    "MetricsAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tags": List[TagTypeDef],
-        "AccessPointArn": str,
-    },
-    total=False,
-)
-
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
-        "AccessPointArn": str,
-    },
-    total=False,
-)
-
-ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
-    "ReplicationRuleAndOperatorOutputTypeDef",
-    {
-        "Prefix": str,
         "Tags": List[TagTypeDef],
+        "AccessPointArn": str,
     },
     total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
@@ -3545,34 +3434,32 @@
 )
 
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
-ListBucketsOutputTypeDef = TypedDict(
-    "ListBucketsOutputTypeDef",
+CORSConfigurationBucketCorsTypeDef = TypedDict(
+    "CORSConfigurationBucketCorsTypeDef",
     {
-        "Buckets": List[BucketTypeDef],
-        "Owner": OwnerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CORSRules": Sequence[CORSRuleBucketCorsTypeDef],
     },
 )
 
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleOutputTypeDef],
+        "CORSRules": List[CORSRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
@@ -3992,29 +3879,30 @@
 )
 
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
+LifecycleExpirationBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleExpirationBucketLifecycleConfigurationTypeDef",
     {
         "Date": TimestampTypeDef,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+LifecycleExpirationBucketLifecycleTypeDef = TypedDict(
+    "LifecycleExpirationBucketLifecycleTypeDef",
     {
-        "Mode": ObjectLockRetentionModeType,
-        "RetainUntilDate": TimestampTypeDef,
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
@@ -4202,16 +4090,26 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
+TransitionBucketLifecycleConfigurationTypeDef = TypedDict(
+    "TransitionBucketLifecycleConfigurationTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
+TransitionBucketLifecycleTypeDef = TypedDict(
+    "TransitionBucketLifecycleTypeDef",
     {
         "Date": TimestampTypeDef,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
@@ -4391,26 +4289,26 @@
     },
     total=False,
 )
 
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-S3KeyFilterOutputTypeDef = TypedDict(
-    "S3KeyFilterOutputTypeDef",
+S3KeyFilterBucketNotificationTypeDef = TypedDict(
+    "S3KeyFilterBucketNotificationTypeDef",
     {
-        "FilterRules": List[FilterRuleTypeDef],
+        "FilterRules": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": Sequence[FilterRuleTypeDef],
+        "FilterRules": List[FilterRuleTypeDef],
     },
     total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
@@ -4465,19 +4363,46 @@
     _OptionalPutObjectLegalHoldRequestRequestTypeDef,
 ):
     pass
 
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionOutputTypeDef,
+        "Retention": ObjectLockRetentionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Retention": ObjectLockRetentionTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "BypassGovernanceRetention": bool,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+class PutObjectRetentionRequestRequestTypeDef(
+    _RequiredPutObjectRetentionRequestRequestTypeDef,
+    _OptionalPutObjectRetentionRequestRequestTypeDef,
+):
+    pass
+
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4629,87 +4554,64 @@
 
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
-MultipartUploadTypeDef = TypedDict(
-    "MultipartUploadTypeDef",
-    {
-        "UploadId": str,
-        "Key": str,
-        "Initiated": datetime,
-        "StorageClass": StorageClassType,
-        "Owner": OwnerTypeDef,
-        "Initiator": InitiatorTypeDef,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-    },
-    total=False,
-)
-
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "CSV": CSVInputTypeDef,
         "CompressionType": CompressionTypeType,
         "JSON": JSONInputTypeDef,
         "Parquet": Mapping[str, Any],
     },
     total=False,
 )
 
-InventoryEncryptionOutputTypeDef = TypedDict(
-    "InventoryEncryptionOutputTypeDef",
-    {
-        "SSES3": Dict[str, Any],
-        "SSEKMS": SSEKMSTypeDef,
-    },
-    total=False,
-)
-
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": Mapping[str, Any],
+        "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
+_RequiredRuleTypeDef = TypedDict(
+    "_RequiredRuleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
     },
 )
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
+_OptionalRuleTypeDef = TypedDict(
+    "_OptionalRuleTypeDef",
     {
-        "Expiration": LifecycleExpirationOutputTypeDef,
+        "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
-        "Transition": TransitionOutputTypeDef,
+        "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
     {
         "Bucket": str,
     },
@@ -4743,14 +4645,15 @@
     "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     {
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
     _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
@@ -4768,14 +4671,15 @@
     "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
     {
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListObjectsRequestListObjectsPaginateTypeDef(
     _RequiredListObjectsRequestListObjectsPaginateTypeDef,
@@ -4795,14 +4699,15 @@
         "Delimiter": str,
         "EncodingType": Literal["url"],
         "Prefix": str,
         "FetchOwner": bool,
         "StartAfter": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
     _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
@@ -4833,36 +4738,14 @@
 
 class ListPartsRequestListPartsPaginateTypeDef(
     _RequiredListPartsRequestListPartsPaginateTypeDef,
     _OptionalListPartsRequestListPartsPaginateTypeDef,
 ):
     pass
 
-ListPartsOutputTypeDef = TypedDict(
-    "ListPartsOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "PartNumberMarker": int,
-        "NextPartNumberMarker": int,
-        "MaxParts": int,
-        "IsTruncated": bool,
-        "Parts": List[PartTypeDef],
-        "Initiator": InitiatorTypeDef,
-        "Owner": OwnerTypeDef,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
     },
 )
 _OptionalMetricsTypeDef = TypedDict(
@@ -4883,42 +4766,35 @@
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedResponseTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-OwnershipControlsOutputTypeDef = TypedDict(
-    "OwnershipControlsOutputTypeDef",
-    {
-        "Rules": List[OwnershipControlsRuleTypeDef],
-    },
-)
-
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": Sequence[OwnershipControlsRuleTypeDef],
+        "Rules": List[OwnershipControlsRuleTypeDef],
     },
 )
 
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": ProgressTypeDef,
@@ -5053,121 +4929,131 @@
     "StatsEventTypeDef",
     {
         "Details": StatsTypeDef,
     },
     total=False,
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+DeleteMarkerEntryTypeDef = TypedDict(
+    "DeleteMarkerEntryTypeDef",
     {
-        "IsTruncated": bool,
-        "Marker": str,
-        "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Owner": OwnerTypeDef,
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
     },
+    total=False,
 )
 
-ListObjectsV2OutputTypeDef = TypedDict(
-    "ListObjectsV2OutputTypeDef",
+ListBucketsOutputTypeDef = TypedDict(
+    "ListBucketsOutputTypeDef",
     {
-        "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "KeyCount": int,
-        "ContinuationToken": str,
-        "NextContinuationToken": str,
-        "StartAfter": str,
-        "RequestCharged": Literal["requester"],
+        "Buckets": List[BucketTypeDef],
+        "Owner": OwnerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectVersionsOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputTypeDef",
+ListPartsOutputTypeDef = TypedDict(
+    "ListPartsOutputTypeDef",
     {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "PartNumberMarker": int,
+        "NextPartNumberMarker": int,
+        "MaxParts": int,
         "IsTruncated": bool,
-        "KeyMarker": str,
-        "VersionIdMarker": str,
-        "NextKeyMarker": str,
-        "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
-        "Name": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
+        "Parts": List[PartTypeDef],
+        "Initiator": InitiatorTypeDef,
+        "Owner": OwnerTypeDef,
+        "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalyticsFilterOutputTypeDef = TypedDict(
-    "AnalyticsFilterOutputTypeDef",
+MultipartUploadTypeDef = TypedDict(
+    "MultipartUploadTypeDef",
     {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": AnalyticsAndOperatorOutputTypeDef,
+        "UploadId": str,
+        "Key": str,
+        "Initiated": datetime,
+        "StorageClass": StorageClassType,
+        "Owner": OwnerTypeDef,
+        "Initiator": InitiatorTypeDef,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-AnalyticsFilterTypeDef = TypedDict(
-    "AnalyticsFilterTypeDef",
+ObjectTypeDef = TypedDict(
+    "ObjectTypeDef",
     {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": AnalyticsAndOperatorTypeDef,
+        "Key": str,
+        "LastModified": datetime,
+        "ETag": str,
+        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
+        "Size": int,
+        "StorageClass": ObjectStorageClassType,
+        "Owner": OwnerTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
+    },
+    total=False,
+)
+
+ObjectVersionTypeDef = TypedDict(
+    "ObjectVersionTypeDef",
+    {
+        "ETag": str,
+        "ChecksumAlgorithm": List[ChecksumAlgorithmType],
+        "Size": int,
+        "StorageClass": Literal["STANDARD"],
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
+        "Owner": OwnerTypeDef,
+        "RestoreStatus": RestoreStatusTypeDef,
     },
     total=False,
 )
 
-IntelligentTieringFilterOutputTypeDef = TypedDict(
-    "IntelligentTieringFilterOutputTypeDef",
+AnalyticsFilterTypeDef = TypedDict(
+    "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
-        "And": IntelligentTieringAndOperatorOutputTypeDef,
+        "And": AnalyticsAndOperatorTypeDef,
     },
     total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
     total=False,
 )
 
-LifecycleRuleFilterOutputTypeDef = TypedDict(
-    "LifecycleRuleFilterOutputTypeDef",
+LifecycleRuleFilterBucketLifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleRuleFilterBucketLifecycleConfigurationTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
-        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "And": LifecycleRuleAndOperatorBucketLifecycleConfigurationTypeDef,
     },
     total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
@@ -5176,46 +5062,25 @@
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
     total=False,
 )
 
-MetricsFilterOutputTypeDef = TypedDict(
-    "MetricsFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "AccessPointArn": str,
-        "And": MetricsAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
     total=False,
 )
 
-ReplicationRuleFilterOutputTypeDef = TypedDict(
-    "ReplicationRuleFilterOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": TagTypeDef,
-        "And": ReplicationRuleAndOperatorOutputTypeDef,
-    },
-    total=False,
-)
-
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
@@ -5423,15 +5288,15 @@
     _RequiredUploadPartCopyRequestRequestTypeDef, _OptionalUploadPartCopyRequestRequestTypeDef
 ):
     pass
 
 _RequiredPutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "_RequiredPutBucketCorsRequestBucketCorsPutTypeDef",
     {
-        "CORSConfiguration": CORSConfigurationTypeDef,
+        "CORSConfiguration": CORSConfigurationBucketCorsTypeDef,
     },
 )
 _OptionalPutBucketCorsRequestBucketCorsPutTypeDef = TypedDict(
     "_OptionalPutBucketCorsRequestBucketCorsPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
@@ -5510,65 +5375,37 @@
 
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
-ObjectLockRetentionUnionTypeDef = Union[
-    ObjectLockRetentionTypeDef, ObjectLockRetentionOutputTypeDef
-]
-_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Retention": ObjectLockRetentionTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "BypassGovernanceRetention": bool,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-class PutObjectRetentionRequestRequestTypeDef(
-    _RequiredPutObjectRetentionRequestRequestTypeDef,
-    _OptionalPutObjectRetentionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
+_RequiredRuleBucketLifecycleTypeDef = TypedDict(
+    "_RequiredRuleBucketLifecycleTypeDef",
     {
         "Prefix": str,
         "Status": ExpirationStatusType,
     },
 )
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
+_OptionalRuleBucketLifecycleTypeDef = TypedDict(
+    "_OptionalRuleBucketLifecycleTypeDef",
     {
-        "Expiration": LifecycleExpirationTypeDef,
+        "Expiration": LifecycleExpirationBucketLifecycleTypeDef,
         "ID": str,
-        "Transition": TransitionTypeDef,
+        "Transition": TransitionBucketLifecycleTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+class RuleBucketLifecycleTypeDef(
+    _RequiredRuleBucketLifecycleTypeDef, _OptionalRuleBucketLifecycleTypeDef
+):
     pass
 
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
         "Rule": ObjectLockRuleTypeDef,
@@ -5620,18 +5457,18 @@
 )
 
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
-NotificationConfigurationFilterOutputTypeDef = TypedDict(
-    "NotificationConfigurationFilterOutputTypeDef",
+NotificationConfigurationFilterBucketNotificationTypeDef = TypedDict(
+    "NotificationConfigurationFilterBucketNotificationTypeDef",
     {
-        "Key": S3KeyFilterOutputTypeDef,
+        "Key": S3KeyFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
@@ -5703,85 +5540,60 @@
     },
     total=False,
 )
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-_RequiredLoggingEnabledOutputTypeDef = TypedDict(
-    "_RequiredLoggingEnabledOutputTypeDef",
+_RequiredLoggingEnabledBucketLoggingTypeDef = TypedDict(
+    "_RequiredLoggingEnabledBucketLoggingTypeDef",
     {
         "TargetBucket": str,
         "TargetPrefix": str,
     },
 )
-_OptionalLoggingEnabledOutputTypeDef = TypedDict(
-    "_OptionalLoggingEnabledOutputTypeDef",
+_OptionalLoggingEnabledBucketLoggingTypeDef = TypedDict(
+    "_OptionalLoggingEnabledBucketLoggingTypeDef",
     {
-        "TargetGrants": List[TargetGrantTypeDef],
+        "TargetGrants": Sequence[TargetGrantTypeDef],
     },
     total=False,
 )
 
-class LoggingEnabledOutputTypeDef(
-    _RequiredLoggingEnabledOutputTypeDef, _OptionalLoggingEnabledOutputTypeDef
+class LoggingEnabledBucketLoggingTypeDef(
+    _RequiredLoggingEnabledBucketLoggingTypeDef, _OptionalLoggingEnabledBucketLoggingTypeDef
 ):
     pass
 
-LoggingEnabledTypeDef = TypedDict(
-    "LoggingEnabledTypeDef",
+LoggingEnabledResponseTypeDef = TypedDict(
+    "LoggingEnabledResponseTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListMultipartUploadsOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputTypeDef",
+_RequiredLoggingEnabledTypeDef = TypedDict(
+    "_RequiredLoggingEnabledTypeDef",
     {
-        "Bucket": str,
-        "KeyMarker": str,
-        "UploadIdMarker": str,
-        "NextKeyMarker": str,
-        "Prefix": str,
-        "Delimiter": str,
-        "NextUploadIdMarker": str,
-        "MaxUploads": int,
-        "IsTruncated": bool,
-        "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
-        "EncodingType": Literal["url"],
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredInventoryS3BucketDestinationOutputTypeDef = TypedDict(
-    "_RequiredInventoryS3BucketDestinationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Format": InventoryFormatType,
+        "TargetBucket": str,
+        "TargetPrefix": str,
     },
 )
-_OptionalInventoryS3BucketDestinationOutputTypeDef = TypedDict(
-    "_OptionalInventoryS3BucketDestinationOutputTypeDef",
+_OptionalLoggingEnabledTypeDef = TypedDict(
+    "_OptionalLoggingEnabledTypeDef",
     {
-        "AccountId": str,
-        "Prefix": str,
-        "Encryption": InventoryEncryptionOutputTypeDef,
+        "TargetGrants": List[TargetGrantTypeDef],
     },
     total=False,
 )
 
-class InventoryS3BucketDestinationOutputTypeDef(
-    _RequiredInventoryS3BucketDestinationOutputTypeDef,
-    _OptionalInventoryS3BucketDestinationOutputTypeDef,
-):
+class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
     pass
 
 _RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
     "_RequiredInventoryS3BucketDestinationTypeDef",
     {
         "Bucket": str,
         "Format": InventoryFormatType,
@@ -5841,19 +5653,26 @@
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
+    {
+        "Rules": Sequence[RuleTypeDef],
+    },
+)
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -5893,20 +5712,19 @@
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsOutputTypeDef,
+        "OwnershipControls": OwnershipControlsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OwnershipControlsUnionTypeDef = Union[OwnershipControlsTypeDef, OwnershipControlsOutputTypeDef]
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
         "OwnershipControls": OwnershipControlsTypeDef,
     },
 )
@@ -5943,25 +5761,18 @@
         "IndexDocument": IndexDocumentTypeDef,
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "RoutingRules": Sequence[RoutingRuleTypeDef],
     },
     total=False,
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
-    },
-)
-
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
+        "Rules": List[ServerSideEncryptionRuleTypeDef],
     },
 )
 
 SelectObjectContentEventStreamTypeDef = TypedDict(
     "SelectObjectContentEventStreamTypeDef",
     {
         "Records": RecordsEventTypeDef,
@@ -5969,42 +5780,99 @@
         "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
     total=False,
 )
 
-_RequiredIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIntelligentTieringConfigurationOutputTypeDef",
+ListMultipartUploadsOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputTypeDef",
     {
-        "Id": str,
-        "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Bucket": str,
+        "KeyMarker": str,
+        "UploadIdMarker": str,
+        "NextKeyMarker": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "NextUploadIdMarker": str,
+        "MaxUploads": int,
+        "IsTruncated": bool,
+        "Uploads": List[MultipartUploadTypeDef],
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
+    {
+        "IsTruncated": bool,
+        "Marker": str,
+        "NextMarker": str,
+        "Contents": List[ObjectTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIntelligentTieringConfigurationOutputTypeDef",
+
+ListObjectsV2OutputTypeDef = TypedDict(
+    "ListObjectsV2OutputTypeDef",
     {
-        "Filter": IntelligentTieringFilterOutputTypeDef,
+        "IsTruncated": bool,
+        "Contents": List[ObjectTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "KeyCount": int,
+        "ContinuationToken": str,
+        "NextContinuationToken": str,
+        "StartAfter": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class IntelligentTieringConfigurationOutputTypeDef(
-    _RequiredIntelligentTieringConfigurationOutputTypeDef,
-    _OptionalIntelligentTieringConfigurationOutputTypeDef,
-):
-    pass
+ListObjectVersionsOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputTypeDef",
+    {
+        "IsTruncated": bool,
+        "KeyMarker": str,
+        "VersionIdMarker": str,
+        "NextKeyMarker": str,
+        "NextVersionIdMarker": str,
+        "Versions": List[ObjectVersionTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
+        "Name": str,
+        "Prefix": str,
+        "Delimiter": str,
+        "MaxKeys": int,
+        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "EncodingType": Literal["url"],
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
     "_RequiredIntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
         "Status": IntelligentTieringStatusType,
-        "Tierings": Sequence[TieringTypeDef],
+        "Tierings": List[TieringTypeDef],
     },
 )
 _OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
     "_OptionalIntelligentTieringConfigurationTypeDef",
     {
         "Filter": IntelligentTieringFilterTypeDef,
     },
@@ -6012,37 +5880,38 @@
 )
 
 class IntelligentTieringConfigurationTypeDef(
     _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
 ):
     pass
 
-_RequiredLifecycleRuleOutputTypeDef = TypedDict(
-    "_RequiredLifecycleRuleOutputTypeDef",
+_RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
+    "_RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef",
     {
         "Status": ExpirationStatusType,
     },
 )
-_OptionalLifecycleRuleOutputTypeDef = TypedDict(
-    "_OptionalLifecycleRuleOutputTypeDef",
+_OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef = TypedDict(
+    "_OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef",
     {
-        "Expiration": LifecycleExpirationOutputTypeDef,
+        "Expiration": LifecycleExpirationBucketLifecycleConfigurationTypeDef,
         "ID": str,
         "Prefix": str,
-        "Filter": LifecycleRuleFilterOutputTypeDef,
-        "Transitions": List[TransitionOutputTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Filter": LifecycleRuleFilterBucketLifecycleConfigurationTypeDef,
+        "Transitions": Sequence[TransitionBucketLifecycleConfigurationTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
-class LifecycleRuleOutputTypeDef(
-    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+class LifecycleRuleBucketLifecycleConfigurationTypeDef(
+    _RequiredLifecycleRuleBucketLifecycleConfigurationTypeDef,
+    _OptionalLifecycleRuleBucketLifecycleConfigurationTypeDef,
 ):
     pass
 
 _RequiredLifecycleRuleTypeDef = TypedDict(
     "_RequiredLifecycleRuleTypeDef",
     {
         "Status": ExpirationStatusType,
@@ -6051,44 +5920,25 @@
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
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
 
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
-_RequiredMetricsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMetricsConfigurationOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalMetricsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMetricsConfigurationOutputTypeDef",
-    {
-        "Filter": MetricsFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-class MetricsConfigurationOutputTypeDef(
-    _RequiredMetricsConfigurationOutputTypeDef, _OptionalMetricsConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredMetricsConfigurationTypeDef = TypedDict(
     "_RequiredMetricsConfigurationTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricsConfigurationTypeDef = TypedDict(
@@ -6108,18 +5958,18 @@
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
     total=False,
 )
 
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
+LifecycleConfigurationBucketLifecycleTypeDef = TypedDict(
+    "LifecycleConfigurationBucketLifecycleTypeDef",
     {
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleBucketLifecycleTypeDef],
     },
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
@@ -6148,83 +5998,85 @@
 
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLambdaFunctionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionConfigurationOutputTypeDef",
+_RequiredLambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredLambdaFunctionConfigurationBucketNotificationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalLambdaFunctionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionConfigurationOutputTypeDef",
+_OptionalLambdaFunctionConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalLambdaFunctionConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
-class LambdaFunctionConfigurationOutputTypeDef(
-    _RequiredLambdaFunctionConfigurationOutputTypeDef,
-    _OptionalLambdaFunctionConfigurationOutputTypeDef,
+class LambdaFunctionConfigurationBucketNotificationTypeDef(
+    _RequiredLambdaFunctionConfigurationBucketNotificationTypeDef,
+    _OptionalLambdaFunctionConfigurationBucketNotificationTypeDef,
 ):
     pass
 
-_RequiredQueueConfigurationOutputTypeDef = TypedDict(
-    "_RequiredQueueConfigurationOutputTypeDef",
+_RequiredQueueConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredQueueConfigurationBucketNotificationTypeDef",
     {
         "QueueArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalQueueConfigurationOutputTypeDef = TypedDict(
-    "_OptionalQueueConfigurationOutputTypeDef",
+_OptionalQueueConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalQueueConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
-class QueueConfigurationOutputTypeDef(
-    _RequiredQueueConfigurationOutputTypeDef, _OptionalQueueConfigurationOutputTypeDef
+class QueueConfigurationBucketNotificationTypeDef(
+    _RequiredQueueConfigurationBucketNotificationTypeDef,
+    _OptionalQueueConfigurationBucketNotificationTypeDef,
 ):
     pass
 
-_RequiredTopicConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTopicConfigurationOutputTypeDef",
+_RequiredTopicConfigurationBucketNotificationTypeDef = TypedDict(
+    "_RequiredTopicConfigurationBucketNotificationTypeDef",
     {
         "TopicArn": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
     },
 )
-_OptionalTopicConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTopicConfigurationOutputTypeDef",
+_OptionalTopicConfigurationBucketNotificationTypeDef = TypedDict(
+    "_OptionalTopicConfigurationBucketNotificationTypeDef",
     {
         "Id": str,
-        "Filter": NotificationConfigurationFilterOutputTypeDef,
+        "Filter": NotificationConfigurationFilterBucketNotificationTypeDef,
     },
     total=False,
 )
 
-class TopicConfigurationOutputTypeDef(
-    _RequiredTopicConfigurationOutputTypeDef, _OptionalTopicConfigurationOutputTypeDef
+class TopicConfigurationBucketNotificationTypeDef(
+    _RequiredTopicConfigurationBucketNotificationTypeDef,
+    _OptionalTopicConfigurationBucketNotificationTypeDef,
 ):
     pass
 
 _RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
     "_RequiredLambdaFunctionConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
     "_OptionalLambdaFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6237,15 +6089,15 @@
 ):
     pass
 
 _RequiredQueueConfigurationTypeDef = TypedDict(
     "_RequiredQueueConfigurationTypeDef",
     {
         "QueueArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalQueueConfigurationTypeDef = TypedDict(
     "_OptionalQueueConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6258,15 +6110,15 @@
 ):
     pass
 
 _RequiredTopicConfigurationTypeDef = TypedDict(
     "_RequiredTopicConfigurationTypeDef",
     {
         "TopicArn": str,
-        "Events": Sequence[EventType],
+        "Events": List[EventType],
     },
 )
 _OptionalTopicConfigurationTypeDef = TypedDict(
     "_OptionalTopicConfigurationTypeDef",
     {
         "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
@@ -6374,67 +6226,64 @@
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
     },
     total=False,
 )
 
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
+BucketLoggingStatusBucketLoggingTypeDef = TypedDict(
+    "BucketLoggingStatusBucketLoggingTypeDef",
     {
-        "LoggingEnabled": LoggingEnabledOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoggingEnabled": LoggingEnabledBucketLoggingTypeDef,
     },
+    total=False,
 )
 
 BucketLoggingStatusTypeDef = TypedDict(
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
     },
     total=False,
 )
 
-InventoryDestinationOutputTypeDef = TypedDict(
-    "InventoryDestinationOutputTypeDef",
+GetBucketLoggingOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputTypeDef",
     {
-        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
+        "LoggingEnabled": LoggingEnabledTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
     },
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
+_RequiredPutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "_RequiredPutBucketLifecycleRequestRequestTypeDef",
     {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
+        "Bucket": str,
     },
 )
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
+_OptionalPutBucketLifecycleRequestRequestTypeDef = TypedDict(
+    "_OptionalPutBucketLifecycleRequestRequestTypeDef",
     {
-        "ID": str,
-        "Priority": int,
-        "Prefix": str,
-        "Filter": ReplicationRuleFilterOutputTypeDef,
-        "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
-        "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
+        "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-class ReplicationRuleOutputTypeDef(
-    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+class PutBucketLifecycleRequestRequestTypeDef(
+    _RequiredPutBucketLifecycleRequestRequestTypeDef,
+    _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
@@ -6499,15 +6348,15 @@
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
@@ -6527,93 +6376,91 @@
 
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-ServerSideEncryptionConfigurationUnionTypeDef = Union[
-    ServerSideEncryptionConfigurationTypeDef, ServerSideEncryptionConfigurationOutputTypeDef
-]
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "AioEventStream[SelectObjectContentEventStreamTypeDef]",
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntelligentTieringConfigurationUnionTypeDef = Union[
-    IntelligentTieringConfigurationTypeDef, IntelligentTieringConfigurationOutputTypeDef
-]
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
 
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef = TypedDict(
+    "BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef",
     {
-        "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Rules": Sequence[LifecycleRuleBucketLifecycleConfigurationTypeDef],
     },
 )
 
 BucketLifecycleConfigurationTypeDef = TypedDict(
     "BucketLifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
 
+GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputTypeDef",
+    {
+        "Rules": List[LifecycleRuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "MetricsConfiguration": MetricsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
+        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricsConfigurationUnionTypeDef = Union[
-    MetricsConfigurationTypeDef, MetricsConfigurationOutputTypeDef
-]
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "MetricsConfiguration": MetricsConfigurationTypeDef,
     },
@@ -6628,34 +6475,14 @@
 
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAnalyticsConfigurationOutputTypeDef",
-    {
-        "Id": str,
-        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
-    },
-)
-_OptionalAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAnalyticsConfigurationOutputTypeDef",
-    {
-        "Filter": AnalyticsFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-class AnalyticsConfigurationOutputTypeDef(
-    _RequiredAnalyticsConfigurationOutputTypeDef, _OptionalAnalyticsConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredAnalyticsConfigurationTypeDef = TypedDict(
     "_RequiredAnalyticsConfigurationTypeDef",
     {
         "Id": str,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
 )
@@ -6672,48 +6499,39 @@
 ):
     pass
 
 PutBucketLifecycleRequestBucketLifecyclePutTypeDef = TypedDict(
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
+        "LifecycleConfiguration": LifecycleConfigurationBucketLifecycleTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-_RequiredPutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "_RequiredPutBucketLifecycleRequestRequestTypeDef",
+NotificationConfigurationBucketNotificationTypeDef = TypedDict(
+    "NotificationConfigurationBucketNotificationTypeDef",
     {
-        "Bucket": str,
-    },
-)
-_OptionalPutBucketLifecycleRequestRequestTypeDef = TypedDict(
-    "_OptionalPutBucketLifecycleRequestRequestTypeDef",
-    {
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": LifecycleConfigurationTypeDef,
-        "ExpectedBucketOwner": str,
+        "TopicConfigurations": Sequence[TopicConfigurationBucketNotificationTypeDef],
+        "QueueConfigurations": Sequence[QueueConfigurationBucketNotificationTypeDef],
+        "LambdaFunctionConfigurations": Sequence[
+            LambdaFunctionConfigurationBucketNotificationTypeDef
+        ],
+        "EventBridgeConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
-class PutBucketLifecycleRequestRequestTypeDef(
-    _RequiredPutBucketLifecycleRequestRequestTypeDef,
-    _OptionalPutBucketLifecycleRequestRequestTypeDef,
-):
-    pass
-
 NotificationConfigurationResponseTypeDef = TypedDict(
     "NotificationConfigurationResponseTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
-        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
+        "TopicConfigurations": List[TopicConfigurationTypeDef],
+        "QueueConfigurations": List[QueueConfigurationTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
@@ -6739,15 +6557,15 @@
     },
     total=False,
 )
 
 _RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "_RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
-        "BucketLoggingStatus": BucketLoggingStatusTypeDef,
+        "BucketLoggingStatus": BucketLoggingStatusBucketLoggingTypeDef,
     },
 )
 _OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef = TypedDict(
     "_OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
@@ -6778,83 +6596,51 @@
 )
 
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
-_RequiredInventoryConfigurationOutputTypeDef = TypedDict(
-    "_RequiredInventoryConfigurationOutputTypeDef",
-    {
-        "Destination": InventoryDestinationOutputTypeDef,
-        "IsEnabled": bool,
-        "Id": str,
-        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
-        "Schedule": InventoryScheduleTypeDef,
-    },
-)
-_OptionalInventoryConfigurationOutputTypeDef = TypedDict(
-    "_OptionalInventoryConfigurationOutputTypeDef",
-    {
-        "Filter": InventoryFilterTypeDef,
-        "OptionalFields": List[InventoryOptionalFieldType],
-    },
-    total=False,
-)
-
-class InventoryConfigurationOutputTypeDef(
-    _RequiredInventoryConfigurationOutputTypeDef, _OptionalInventoryConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredInventoryConfigurationTypeDef = TypedDict(
     "_RequiredInventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
     },
 )
 _OptionalInventoryConfigurationTypeDef = TypedDict(
     "_OptionalInventoryConfigurationTypeDef",
     {
         "Filter": InventoryFilterTypeDef,
-        "OptionalFields": Sequence[InventoryOptionalFieldType],
+        "OptionalFields": List[InventoryOptionalFieldType],
     },
     total=False,
 )
 
 class InventoryConfigurationTypeDef(
     _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
 ):
     pass
 
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
 
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "LifecycleConfiguration": BucketLifecycleConfigurationTypeDef,
+        "LifecycleConfiguration": BucketLifecycleConfigurationBucketLifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
 _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef",
@@ -6877,33 +6663,30 @@
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalyticsConfigurationUnionTypeDef = Union[
-    AnalyticsConfigurationTypeDef, AnalyticsConfigurationOutputTypeDef
-]
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
     },
@@ -6921,15 +6704,15 @@
     _OptionalPutBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
 _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationBucketNotificationTypeDef,
     },
 )
 _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
@@ -7012,33 +6795,30 @@
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
+        "InventoryConfiguration": InventoryConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InventoryConfigurationUnionTypeDef = Union[
-    InventoryConfigurationTypeDef, InventoryConfigurationOutputTypeDef
-]
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
         "InventoryConfiguration": InventoryConfigurationTypeDef,
     },
@@ -7056,15 +6836,15 @@
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
@@ -7083,11 +6863,7 @@
 )
 
 class PutBucketReplicationRequestRequestTypeDef(
     _RequiredPutBucketReplicationRequestRequestTypeDef,
     _OptionalPutBucketReplicationRequestRequestTypeDef,
 ):
     pass
-
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
```

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/waiter.py` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3/waiter.pyi` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post1/types_aiobotocore_s3.egg-info/SOURCES.txt` & `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

